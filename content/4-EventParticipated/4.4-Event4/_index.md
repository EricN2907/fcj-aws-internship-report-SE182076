---
title: "Event 4"
date: 2025-09-09
weight: 4
chapter: false
pre: " <b> 4.4. </b> "
---


# Summary Report: AWS Cloud Mastery Series #2 – DevOps on AWS

## 1. Attendance Objectives
By attending this event, I set key objectives to enhance my technical capabilities:
- Master the core DevOps mindset and how to measure effectiveness through DORA metrics.
- Master the process of building end-to-end CI/CD pipelines on the AWS ecosystem.
- Analyze and select the optimal Infrastructure as Code (IaC) tool: CloudFormation or AWS CDK?
- Learn containerization strategies with Amazon ECS, EKS, and App Runner.
- Implement in-depth Observability solutions with CloudWatch and AWS X-Ray.

## 2. Event Information
- **Time:** 08:30 – 17:00, Monday, November 17, 2025.
- **Location:** 26th Floor, Bitexco Financial Tower, District 1, Ho Chi Minh City.
- **Speakers:** Experts from AWS Community Builders (Truong Quang Tinh, Kha Van, Bao Huynh, Thinh Nguyen, Vi Tran).

## 3. Technical Content

### DevOps Mindset & Performance Measurement
- **Unified Culture:** Breaking down barriers between Dev and Ops, moving towards a shared responsibility model.
- **DORA Metrics:** 4 "golden" measures for project health: Deployment Frequency (DF), Lead Time for Changes (LT), Mean Time to Recovery (MTTR), and Change Failure Rate (CFR).

### CI/CD Ecosystem on AWS
- **Source Control:** Managing source code with AWS CodeCommit, comparing GitFlow and Trunk-based models.
- **Orchestration:** Automating software release processes with **AWS CodePipeline**.
- **Deployment Strategies:**
    - *Blue/Green:* Running two environments in parallel to reduce risk and downtime.
    - *Canary:* Releasing experimental versions to a small group of users.
    - *Rolling:* Gradually updating infrastructure in portions.

### Infrastructure as Code (IaC)
- **AWS CloudFormation:** Declarative approach with JSON/YAML, strong in state management (drift detection).
- **AWS CDK:** Imperative approach, allowing the use of programming languages (Java, TypeScript...) to define infrastructure, enabling more effective code reuse.

### Containers & Observability
- **Compute Selection:** Weighing between detailed control (Amazon ECS), Kubernetes standardization (EKS), or simplicity and speed (App Runner).
- **Comprehensive Monitoring:** Combining CloudWatch (Logs/Metrics) and AWS X-Ray for tracing errors in complex Microservices architectures.

## 4. Key Takeaways

### System Design Thinking
- **Automate Everything:** From testing to infrastructure deployment, everything must be automated to eliminate human errors.
- **Shift-Left Security:** Security must be integrated from the coding phase, not as a final step.
- **Data-Driven:** Using DORA metrics as a compass to improve processes.

### Architecture & Modernization
- **Immutable Infrastructure:** Don't fix running servers; completely replace them with new servers when changes occur.
- **Pipeline Orchestration:** Establishing strict approval gates before going to Production.
- **Right-sizing:** Choosing the right tool for the purpose (e.g., using App Runner for simple web apps to save operational costs).

## 5. Action Plan

After the workshop, I will apply the knowledge to real projects:
1.  **Git Workflow:** Switching to **Trunk-based Development** model to reduce code conflicts when working in teams.
2.  **CI/CD Pipeline:** Setting up **AWS CodePipeline** for the student management project, ensuring code is automatically deployed upon merge.
3.  **Infrastructure Refactoring:** Rewriting current DynamoDB and Lambda configurations using **AWS CDK** instead of manual operations, making maintenance and scaling easier.
4.  **Monitoring:** Setting up **CloudWatch Alarms** to alert immediately when APIs return 5xx errors.

## 6. Experience & Reflections

The "DevOps on AWS" event was truly an important piece that helped me connect Development (Dev) and Operations (Ops) thinking. Not just stopping at theory, I witnessed the real power of automation:
- **Learning from Experts:** Understanding the real "pitfalls" when implementing DevOps and the Shared Responsibility model.
- **Impressive Live Demo:** Seeing firsthand how AWS CDK deployed an entire VPC and ECS cluster with very concise code, as well as AWS X-Ray's ability to instantly "diagnose" system issues.
- **Networking:** Getting clearer guidance on the path to conquering the **AWS Certified DevOps Engineer – Professional** certification.

> **Conclusion:** "Infrastructure as Code" and "Observability" are no longer optional, but mandatory standards. The event equipped me with the necessary mindset to build Production-ready systems: Reliable, Secure, and Scalable.

![](/images/4-EventParticipated/4.4-Event4/Image_4.1.jpg)
![Warm-up with speaker Tinh Truong](/images/4-EventParticipated/4.4-Event4/Image_4.2.jpg)
![Infrastructure as Code (IaC)](/images/4-EventParticipated/4.4-Event4/Image_4.3.jpg)
