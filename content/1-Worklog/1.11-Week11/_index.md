---
title: "Week 11 Worklog"
date: 2025-11-16
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

- Setup CloudWatch monitoring and alarms
- Implement Notification system
- Attend AWS Cloud Mastery Series #2 (DevOps)
- Optimize Lambda performance

### Tasks to Execute This Week:

| **Date**          | **Task**                                                                                                                                                                                                                                               | **Start**  | **Finish** | **References**        |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | ---------- | --------------------- |
| Monday (17/11)    | **AWS Cloud Mastery Series #2 – DevOps on AWS**<br>_Time: 08:30 – 17:00_<br>- Full-day workshop<br>- Learn CodePipeline, CodeBuild, CodeDeploy<br>- Hands-on labs for CI/CD<br>- Plan CI/CD for the project                                            | 17/11/2025 | 17/11/2025 | -                     |
| Tuesday (18/11)   | - **Setup CloudWatch Monitoring:**<br>&emsp;+ Verify Lambda log groups<br>&emsp;+ Create custom metrics<br>&emsp;+ Setup CloudWatch Insights queries<br>&emsp;+ Create monitoring dashboard                                                            | 18/11/2025 | 18/11/2025 | CloudWatch Guide      |
| Wednesday (19/11) | - **Configure CloudWatch Alarms:**<br>&emsp;+ Lambda error alarm (threshold > 5)<br>&emsp;+ Lambda duration alarm<br>&emsp;+ API Gateway 5xx alarm<br>&emsp;+ DynamoDB throttle alarm<br>- Setup SNS notifications                                     | 19/11/2025 | 19/11/2025 |                       |
| Thursday (20/11)  | - **Implement Notifications APIs:**<br>&emsp;+ POST /notifications (create)<br>&emsp;+ GET /notifications (list)<br>&emsp;+ GET /notifications/{id}<br>&emsp;+ PUT /notifications/{id}/read (mark as read)<br>- Integrate with DynamoDB table          | 20/11/2025 | 20/11/2025 | -                     |
| Friday (21/11)    | - **Lambda Performance Optimization:**<br>&emsp;+ Analyze cold start metrics<br>&emsp;+ Optimize dependencies<br>&emsp;+ Implement connection pooling for DynamoDB<br>&emsp;+ Consider Provisioned Concurrency<br>- Benchmark performance improvements | 21/11/2025 | 21/11/2025 | Lambda Best Practices |

### Week 11 Achievements:

- Completed AWS DevOps workshop, strengthened CI/CD knowledge
- Configured CloudWatch dashboards, metrics, alarms
- Implemented Notifications APIs with improved DynamoDB efficiency
- Optimized Lambda performance, reduced cold starts
- System ready for real-world load testing with monitoring enabled

---
