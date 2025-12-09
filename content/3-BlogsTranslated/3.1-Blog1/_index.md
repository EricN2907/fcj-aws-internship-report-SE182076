---
title: "Blog 1"
date: 2025-09-09
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---

# Simplify your canary by batching multiple URLs in Amazon CloudWatch Synthetics

*by Shree Chinnasamy on 20 SEP 2021*

You can use Amazon CloudWatch Synthetics to create canaries, configurable scripts that run on a schedule, to monitor your endpoints and API operations. Canaries follow the same routes and perform the same actions as a customer, which makes it possible to continuously verify your customer experience even when you don’t have any customer traffic on your applications. By using canaries, you can discover issues before your customers do.

If your canary uses `syn-nodejs-puppeteer-3.1` or later runtime version, you can use the Heartbeat monitoring blueprint and batch multiple URLs in a single canary versus using multiple canaries to monitor a single URL. You can then see the status, duration, associated screenshots, and failure reason for each URL in the step summary of the canary run report. As CloudWatch Synthetics is priced on canary runs, batching multiple URLs in a single canary also reduces your costs. Check Pricing section of this blog post for additional details.

## Walkthrough

In this blog post, I present the value proposition for batching multiple URLs in a single canary. For the purposes of this blog post, my canaries monitor multiple URLs as shown in Figure 2.

Figure 1 shows the Create canary page in the CloudWatch console. To use Heartbeat monitoring blueprint to monitor multiple URLs, complete the fields as shown in the Figure 1. Once you fill the necessary fields in the page, click on Create canary button in the bottom of the page.

On the Create canary page, the **Use a blueprint** option is selected. Under Blueprints, **Heartbeat monitoring** is selected. In Canary builder, you can add up to five endpoints. You can add even more by modifying the script.

<div align="center">
  <img src="/images/3-Translates%20Blog/Blog%201/Figure1_Monitoring_multiple_URLs_in_heartbeat_monitoring_blueprint.png" width="70%" alt="Figure 1: Create canary page">
</div>

> **Figure 1: Create canary page**

Select the canary from the canaries list page and navigate to the canary details page. You should see that the canary is in Running state. Click on Availability tab to view information about the recent runs of this canary. Figure 2 shows the step summary of the canary run report in the CloudWatch console.

On the details page for `shreetest-canary-1`, five steps were run. All have a status of Passed.

<div align="center">
  <img src="/images/3-Translates%20Blog/Blog%201/Figure2_Step_summary_-of_the_canary_run_report.png" width="80%" alt="Figure 2: Step summary of the canary run report">
</div>

> **Figure 2: Step summary of the canary run report**

If you’re monitoring multiple URLs in Heartbeat monitoring blueprint:

1. Canaries that use either the `executeStep()` or `executeHttpStep()` methods from the Synthetics library also publish SuccessPercent and Duration metrics with the dimensions CanaryName and StepName for each step.
2. For canaries that use `syn-nodejs-pupeteer-3.1` or later, the (options) for `setConfig` support multiple Boolean parameters that determine which metrics are published by the canary. For more information, check Library functions available for Node.js canary scripts and SyntheticsConfiguration class in the Amazon CloudWatch User Guide. As you see fit, disable relevant parameters in the (options) for `setConfig` to save costs.

In the following example, `setConfig` allows all steps to run even if some fail. It disables taking screenshot on step start.

```javascript
syntheticsConfiguration.setConfig 
({
    continueOnStepFailure : true,
    screenshotOnStepStart : false
});
```

## Pricing

Your monthly bill varies depending on number of canary runs, AWS Lambda charges, monitoring and storage configuration of the canary. Note that CloudWatch Synthetics publishes SuccessPercent and Duration metrics for the overall AWS account, each canary, and each step. Each canary run also runs Lambda function and writes logs and results to CloudWatch Logs and to the designated Amazon Simple Storage Service (Amazon S3) bucket. For more information, check the Lambda, Amazon S3, and CloudWatch Logs pricing pages.

## Cleanup

To avoid charges to your account, remove the resources you created.

1. In the Amazon CloudWatch console, choose the canary you created and from Actions, choose **Stop**.
2. Choose the canary again and from Actions, choose **Delete**.

When you delete a canary, the resources used and created by the canary are not deleted automatically. Also delete the following:

* (optional) In the Amazon CloudWatch console, delete the CloudWatch alarms created for this canary. These alarms have a name of `Synthetics-Alarm-MyCanaryName`.
* In the Amazon CloudWatch console, delete the CloudWatch log groups created for the canary. These logs groups have the name `aws/lambda/cwsyn-MyCanaryName`.
* In the AWS Lambda console, delete the Lambda function used by this canary. These have the prefix `cwsyn-MyCanaryName`.
* In the Amazon S3 console, delete the Amazon S3 objects and buckets created for this canary, such as the canary’s artifact location.
* In the AWS Identity and Access Management console, delete the IAM roles created for the canary. If they were created in the console, these roles have the name `role/service-role/CloudWatchSyntheticsRole-MyCanaryName`.


**About the Author**

| |
| :--- |
| **Shree Chinnasamy** <br><br> <img src="/images/3-Translates%20Blog/Blog%201/Shree-Chinnasamy-Profile.jpg" align="left" width="200px" style="margin-right: 25px; border-radius: 50%;"> <span style="font-size: 25px;">Shree Chinnasamy is a Senior Specialist Solutions Architect in the Cloud Operations team at AWS. He primarily focuses on AWS monitoring and observability services such as Amazon CloudWatch, AWS X-Ray, Amazon Managed Service for Prometheus and Amazon Managed Grafana. He graduated with a Master of Science degree in Telecommunication Systems Management from Northeastern University, Boston. An avid reader and a marathon finisher, Shree is based out of Washington in the Pacific Northwest. LinkedIn profile: www.linkedin.com/in/shreekarthic</span> |

