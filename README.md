# LFS162

DevOps and Site Reliability Engineering

# DevOps Tools

## Version Control

- **Git** – Widely used for version control; tracks changes in source code during development.
- **Subversion (SVN)** – Centralized version control system; tracks changes to files and directories. Preferred for linear workflows.
- **Bitbucket** – Cloud-based Git platform; offers code hosting, pull requests, issue tracking, and CI/CD tools.
- **GitHub** – Popular cloud platform for version control, social coding, and project management.

## Continuous Integration / Continuous Deployment (CI/CD)

- **Jenkins** – Open source automation server for building, testing, and deploying code.
- **Travis CI** – CI/CD service integrated with GitHub for automated testing and deployment.
- **CircleCI** – Cloud-based CI/CD platform supporting automation and parallel testing.

## Configuration Management

- **Ansible** – Open source automation tool for configuration management, deployment, and task automation.
- **Chef** – Infrastructure automation using reusable scripts called recipes.
- **Puppet** – Automates provisioning and management of infrastructure.

## Containerization and Orchestration

- **Docker** – Platform for developing, shipping, and running applications in containers.
- **Podman** – Open source container engine, Docker-compatible CLI, image creation, and deployment.
- **LXC (Linux Containers)** – Lightweight containerization built into the Linux kernel; efficient and portable.
- **Kubernetes** – Container orchestration platform for deployment, scaling, and management of containers.
- **OpenShift** – Red Hat container platform extending Kubernetes with enterprise features and developer tools.
- **Apache Mesos** – Cluster management and orchestration platform for distributed applications.

## Infrastructure as Code (IaC)

- **Terraform** – Tool for building, changing, and versioning infrastructure efficiently.
- **AWS CloudFormation** – Amazon’s IaC service for provisioning and managing AWS resources using templates.
- **OpenTofu** – Open source, community-driven fork of Terraform, managed by the Linux Foundation.

## Continuous Monitoring

- **Prometheus** – Open source monitoring and alerting toolkit.
- **Zabbix** – Monitoring for servers, networks, applications; supports alerting and reporting.
- **Nagios** – Server and network monitoring tool with plugin support and alerting.
- **OpenNMS** – Network management system with monitoring, discovery, and visualization.
- **Grafana** – Visualization platform for interactive dashboards; integrates with Prometheus and other data sources.

## Collaboration and Communication

- **Slack** – Team collaboration and communication tool.
- **Microsoft Teams** – Communication and collaboration platform integrated with Microsoft tools.

## Logging

- **ELK Stack (Elasticsearch, Logstash, Kibana)** – Log management, search, analysis, and visualization.
- **Fluentd** – Lightweight log collector and forwarder; integrates with various logging platforms.
- **Splunk** – Comprehensive logging platform with real-time analytics and AI-driven insights.
- **Datadog** – Monitoring platform with log management, metrics collection, and application performance monitoring.

## Source Code Management (SCM)

- **Bitbucket** – Git repository management with code collaboration and CI/CD features.
- **GitLab** – Web-based Git repository manager with CI/CD, code review, and collaboration.
- **GitHub** – Web-based platform for storing, tracking, and collaborating on code.

# Types of Clouds

## Infrastructure as a Service (IaaS)

**What it is:**  
Imagine you're building a house. IaaS is like renting the land and the basic utilities (electricity, water, etc.). You have the freedom to design and build your house the way you want.

**For developers:**  
With IaaS in the cloud, developers get the basic tools (servers, storage, and networking) to create and manage their own digital 'houses' (applications). It's like having your own digital construction site.

---

## Platform as a Service (PaaS)

**What it is:**  
Think of PaaS as hiring a construction company to build your house. You don't worry about the details of buying land or managing construction workers; you just tell the company what you want, and they take care of the rest.

**For developers:**  
In the cloud, PaaS lets developers focus only on building and improving their applications. They don't need to handle 'construction' details such as servers; they just focus on creating a great 'house' (application).

---

## Software as a Service (SaaS)

**What it is:**  
SaaS is like renting a fully furnished house instead of building one. You move in, and everything you need is already there – furniture, appliances, everything.

**For developers:**  
In the cloud, SaaS provides fully developed applications that developers and users can use immediately without worrying about building or maintaining anything. It's like moving into a ready-made 'digital house.'

---

## Function as a Service (FaaS)

**What it is:**  
FaaS is like the concept of co-working spaces, where freelancers, entrepreneurs, and small teams access a fully-equipped office on an as-needed basis without committing to a long-term lease. You simply show up, use a desk or office, and all maintenance, utilities, and internet services are taken care of. This setup allows you to focus on work without managing office space.

**For developers:**  
In the cloud, FaaS allows developers to deploy applications without managing the servers. The cloud provider dynamically manages resource allocation. This model allows developers to focus on application functionality, scale based on usage, and pay only for the resources consumed during execution.

# Introduction to Terraform

Imagine this: you're a software developer building an amazing new app. But then comes the dreaded task — setting up the infrastructure. Manually provisioning servers, configuring networks, and managing databases sounds like a nightmare, right?

That’s where **Infrastructure as Code (IaC)** tools like Terraform come in.

Think of Terraform as your personal infrastructure chef — handling all the tedious setup and management tasks efficiently and automatically.

---

## What is Terraform?

Terraform is a powerful **open-source Infrastructure as Code (IaC) tool** that allows you to define infrastructure using human-readable configuration files.

Instead of manually clicking through cloud dashboards, you write code that describes the infrastructure you need.

This code becomes a **blueprint for your infrastructure**, allowing you to:

- Provision infrastructure automatically
- Manage infrastructure consistently
- Version control infrastructure changes
- Reuse infrastructure configurations
- Scale resources easily
- Maintain infrastructure across multiple cloud providers

---

## Real-World Examples of Using Terraform

### 1. Startup Launching a Web Application

A startup wants to launch a web application with:

- A database
- A load balancer
- Application servers

Using Terraform, they can:

- Define the entire infrastructure in a single configuration file
- Provision everything automatically
- Scale resources up or down as needed

---

### 2. Large Organization Managing Multi-Cloud Infrastructure

A large enterprise manages infrastructure across multiple cloud providers.

With Terraform, they can:

- Manage all infrastructure from a single platform
- Maintain consistency across environments
- Enforce compliance and governance standards

---

### 3. Microservices Deployment

A development team wants to deploy a microservices architecture.

Using Terraform:

- Each microservice can be defined as a Terraform module
- Infrastructure becomes reusable and modular
- Deployment and management become simplified
- Teams can scale services independently

---

## Why Terraform Matters

Terraform helps you:

- Automate infrastructure provisioning
- Reduce manual errors
- Improve consistency
- Enable collaboration through version control
- Treat infrastructure like software

In short, Terraform turns infrastructure management into a programmable, repeatable, and scalable process.

# 🌱 Introduction to OpenTofu

In the space of Infrastructure as Code (IaC), Terraform has long been the reigning champion. However, concerns about its future under HashiCorp's Business Source License (BSL) sparked the creation of OpenTofu — a fork that aims to reclaim the open source spirit and provide developers and DevOps engineers with greater flexibility and control.

---

# ❓ What is OpenTofu?

OpenTofu is an open source IaC tool forked from Terraform version 1.5.

It inherits the familiar syntax and functionality of Terraform, making it easy for existing Terraform users to adopt. However, OpenTofu goes beyond simply replicating Terraform. It introduces key enhancements and features that support the open source community and address limitations introduced by the BSL license.

---

# ✅ Advantages of OpenTofu

## 🔓 Open Source and Community-Driven

OpenTofu is fully committed to open source principles.

- Development is led by a dedicated community of contributors
- Transparent roadmap and governance
- Anyone can participate in shaping the future of the project
- Encourages collaboration and innovation

This approach leads to a more robust and feature-rich tool.

---

## ⚙️ Flexibility and Control

OpenTofu offers greater flexibility compared to Terraform under the BSL.

Users can:

- Modify the core code
- Contribute extensions
- Customize the tool for specific needs
- Avoid proprietary licensing restrictions

---

## 🔮 Future-Proof

OpenTofu ensures the future of Terraform-style IaC remains open.

By providing a fully open source alternative, it guarantees:

- Long-term availability
- No vendor lock-in concerns
- Stability regardless of future licensing changes

---

## 🚀 Continuous Development and Improvement

The active OpenTofu community ensures:

- Regular feature releases
- Bug fixes
- Performance improvements
- Security updates

---

## 🔄 Familiarity for Terraform Users

OpenTofu maintains nearly identical syntax and structure to Terraform.

This means:

- Easy migration
- Minimal learning curve
- Compatibility with existing Terraform workflows
- Reusable infrastructure configurations

---

# 🏁 Summary

OpenTofu is a powerful, open source Infrastructure as Code tool that:

- Preserves Terraform’s familiar experience
- Restores full open source freedom
- Encourages community-driven innovation
- Provides long-term flexibility and sustainability

It is an excellent alternative for teams who value openness, control, and future-proof infrastructure automation.

# 🔄 Continuous Integration / Continuous Delivery (CI/CD)

CI/CD includes deployment strategies that help release software safely, efficiently, and with minimal risk.

---

# 🔵🟢 Blue-Green Deployment

In a Blue-Green deployment, two identical environments are maintained:

- **Blue** → Current production environment
- **Green** → New version environment (staging/testing)

Traffic is switched from Blue to Green once the new version is verified.

## ✅ Characteristics

- **Zero Downtime**  
  Deployment and testing happen without affecting live users.

- **Quick Rollback**  
  If issues are detected, simply switch traffic back to the previous environment.

## 🎯 Use Cases

- Web applications where downtime is unacceptable
- Mission-critical systems requiring safe transitions
- Systems needing instant rollback capability

---

# 🐤 Canary Release

A Canary release deploys a new version to a small subset of users (the "canaries") before rolling it out to everyone.

This allows real-world testing under limited exposure.

## ✅ Characteristics

- **Gradual Rollout**  
  Starts with a small percentage of users.

- **Real-Time Monitoring**  
  Performance, logs, and user feedback are closely monitored.

- **Risk Mitigation**  
  Issues are identified before full deployment.

## 🎯 Use Cases

- Web and mobile applications
- Feature experimentation
- User behavior testing
- High-risk feature deployments

---

# 📈 Phased (Staged) Rollout

In a phased rollout, the new version is released to groups of users in predefined stages.

Each stage expands the release scope after monitoring and validation.

## ✅ Characteristics

- **Controlled Progression**  
  Rollout happens in structured stages.

- **Feedback and Monitoring**  
  Each stage allows for validation before expanding.

- **Risk Mitigation**  
  Issues can be fixed before reaching all users.

## 🎯 Use Cases

- Large-scale applications
- Global platforms with diverse users
- Enterprise software rollouts
- Compliance-sensitive environments

---

# 🏁 Summary Comparison

| Strategy       | Deployment Style                 | Risk Level | Rollback Speed | Best For              |
| -------------- | -------------------------------- | ---------- | -------------- | --------------------- |
| Blue-Green     | Full switch between environments | Low        | Instant        | Zero-downtime systems |
| Canary         | Small user subset first          | Very Low   | Moderate       | Real-world testing    |
| Phased Rollout | Gradual staged release           | Low        | Moderate       | Large-scale systems   |

---

# 🚀 Final Thought

Choosing the right deployment strategy depends on:

- Application criticality
- User base size
- Infrastructure maturity
- Monitoring capabilities
- Risk tolerance

All three strategies aim to **reduce deployment risk while maintaining reliability and user experience.**

# 🚀 GitOps as a Deployment Tool

GitOps is a deployment methodology that uses **Git as the single source of truth** for infrastructure and application configuration.

With GitOps:

- Infrastructure and application configurations are stored in Git repositories.
- Changes are made through pull requests.
- Deployments are automated using Git workflows.
- Systems continuously reconcile the actual state with the desired state defined in Git.

This approach enables teams to manage applications and infrastructure in a **declarative, version-controlled, and automated way**.

---

# 🔧 Popular GitOps Tools

## 🌊 Argo CD

Argo CD is an open source GitOps continuous delivery tool that:

- Supports multiple platforms and environments
- Integrates tightly with Kubernetes
- Provides a UI dashboard for deployment visibility
- Automatically syncs cluster state with Git repositories

---

## 🔁 Flux CD

Flux CD is an open source GitOps continuous delivery tool designed specifically for:

- Kubernetes deployments
- Automated synchronization of cluster state
- Continuous monitoring of Git repositories for changes

It is lightweight and highly Kubernetes-focused.

---

## 🔨 Tekton CD

Tekton CD is an open source continuous delivery platform built on Kubernetes.

- Kubernetes-native pipelines
- Designed for cloud-native environments
- Supports GitOps-style workflows

---

## ⚙️ Jenkins X

Jenkins X combines GitOps principles with Jenkins for continuous delivery.

- Kubernetes-native CI/CD
- Automated environment promotion
- Git-based workflow management
- Preview environments per pull request

---

# 📋 GitOps Adoption Considerations

## 🏗 Infrastructure as Code (IaC) Adoption

GitOps relies heavily on existing IaC practices.

- Infrastructure must be defined declaratively.
- Tools like Terraform or Kubernetes manifests are typically required.
- Configuration files must be stored and versioned in Git.

---

## 🛠 Tool Selection

Choosing the right GitOps tool depends on:

- Target platform (e.g., Kubernetes)
- Team expertise
- Scalability requirements
- Observability needs
- Integration with existing CI/CD tools

---

## 🔐 Security Considerations

Since Git is the source of truth, securing repositories is critical.

Best practices include:

- Role-based access control (RBAC)
- Branch protection rules
- Signed commits
- Secret management solutions
- Audit logging and monitoring

---

# 🏁 Benefits of GitOps

- ✅ Version-controlled infrastructure
- ✅ Improved auditability
- ✅ Faster recovery and rollbacks
- ✅ Reduced configuration drift
- ✅ Enhanced collaboration via Git workflows

---

# 🎯 Summary

GitOps transforms deployment into a **Git-driven, automated, and declarative process**.

By treating Git as the single source of truth, organizations can:

- Increase reliability
- Improve security
- Enhance visibility
- Accelerate delivery cycles

# 🔎 The Three Pillars of Observability

Observability helps teams understand what is happening inside complex systems.  
It is built on three foundational pillars:

- Logs
- Metrics
- Traces

---

## 📝 Logs

**Logs are digital records of events that have occurred within a system.**

### 🔹 Application Logs

Application logs record events happening within the application layer, such as:

- User actions
- System errors
- Transactions
- Debug information

These logs help teams understand real-world application behavior and troubleshoot application-level issues.

---

### 🔹 System Logs

System logs document operating system-level events, including:

- System calls
- Scheduled tasks
- Kernel messages
- Hardware-related events

They are useful for diagnosing hardware or OS-level problems that impact application performance.

---

### 🔹 Audit Logs

Audit logs focus on security-related events, such as:

- User login attempts
- Permission changes
- Configuration updates
- Administrative actions

They are essential for:

- Security monitoring
- Compliance requirements
- Forensic investigations

---

## 📊 Metrics

Metrics provide numerical data about system and application performance over time.

### 🔹 System Metrics

System metrics measure infrastructure health, including:

- CPU usage
- Memory consumption
- Disk I/O
- Network bandwidth

They help monitor infrastructure stability and capacity.

---

### 🔹 Application Metrics

Application metrics focus on software performance, such as:

- Request latency
- Throughput
- Error rates
- Transaction volumes

These metrics help identify bottlenecks and performance degradation.

---

### 🔹 Business Metrics

Business metrics measure business impact, including:

- Daily active users (DAU)
- Conversion rates
- Revenue metrics
- Customer engagement

Although not purely technical, they connect system performance to business outcomes.

---

## 🔗 Traces

Traces show the journey of a request as it moves through different services in a distributed system.

### 🔹 Span

A **span** represents a single operation within a trace.

It typically includes:

- Start time
- End time
- Duration (latency)
- Operation name

---

### 🔹 Trace Context

Trace context carries the trace identity across:

- Services
- Processes
- Network boundaries

This ensures all spans belonging to the same request are properly linked.

---

### 🔹 Annotations and Metadata

Additional data attached to spans, such as:

- User IDs
- Error messages
- Service names
- Custom tags

This enriches traces and improves debugging capabilities.

---

# 📈 The Importance of SLA, SLO, and SLI in Observability

## 📌 Service Level Indicator (SLI)

An **SLI** is a measurable metric that quantifies system performance.

Examples:

- Latency
- Error rate
- Availability

It answers:  
**"What are we measuring?"**

---

## 🎯 Service Level Objective (SLO)

An **SLO** defines the target or acceptable range for an SLI.

Example:

- "99.9% uptime per month"

It answers:  
**"What is our performance goal?"**

---

## 📜 Service Level Agreement (SLA)

An **SLA** is a formal agreement with customers.

It often includes:

- Performance commitments
- Financial penalties
- Compensation terms if SLOs are not met

It answers:  
**"What have we promised externally?"**

---

# 🏁 Summary

Observability enables teams to:

- Detect issues quickly
- Understand system behavior
- Improve reliability
- Align technical performance with business goals

Logs, Metrics, and Traces provide visibility, while SLIs, SLOs, and SLAs define measurable reliability standards.

Let’s take a look at an example. Imagine a cloud storage service where an SLI tracks the success rate of file uploads. The SLO might specify that 99.95% of uploads must succeed within 5 seconds, while the SLA could promise enterprise customers a refund if this performance drops below that threshold. Observability tools then provide real-time insights into these metrics, helping engineers ensure compliance and maintain trust.


# 🔎 Observability Tools

Observability tools help organizations monitor, analyze, and troubleshoot systems using metrics, logs, traces, and performance data.

---

# 📊 Monitoring and Metrics

## Prometheus
Prometheus is an open source monitoring and alerting toolkit designed for reliability and scalability.

- Pull-based metrics collection
- Powerful query language (PromQL)
- Built-in alerting
- Strong Kubernetes integration

---

## Grafana
Grafana is a visualization platform used to create interactive dashboards.

- Integrates with multiple data sources (Prometheus, InfluxDB, etc.)
- Real-time monitoring dashboards
- Alerting capabilities
- Customizable visualizations

---

## InfluxDB
InfluxDB is a time-series database optimized for storing and querying time-stamped data.

- High-performance writes
- Efficient time-series queries
- Often used for metrics storage

---

## Datadog
Datadog is a cloud-based monitoring platform.

- Infrastructure monitoring
- Application monitoring
- Log management
- Real-time dashboards
- SaaS-based solution

---

# 📝 Logging

## ELK Stack

ELK stands for:

- **Elasticsearch** → Distributed search and analytics engine  
- **Logstash** → Log collection and pipeline processing tool  
- **Kibana** → Visualization and dashboard platform  

Together, they form a powerful centralized log management solution.

---

## Splunk

Splunk is a widely used platform for searching, monitoring, and analyzing machine-generated data.

- Advanced search capabilities
- Real-time log analysis
- Powerful dashboards
- Enterprise security features

---

# 🔗 Tracing

## Jaeger

Jaeger is an open source, end-to-end distributed tracing system.

- Monitors request latency
- Supports microservices architectures
- Helps identify performance bottlenecks
- Root cause analysis for distributed systems

---

## Zipkin

Zipkin is an open source distributed tracing system.

- Tracks requests across services
- Visualizes service dependencies
- Measures latency in distributed systems

---

# ⚡ Application Performance Monitoring (APM)

## New Relic

New Relic is a cloud-based APM tool that provides deep insights into application performance.

- Transaction tracing
- Error tracking
- Infrastructure monitoring
- Real-time performance analytics

---

## AppDynamics

AppDynamics is a comprehensive APM solution.

- Real-time application monitoring
- User experience tracking
- Infrastructure visibility
- Performance bottleneck detection

---

# 🏗 Infrastructure Monitoring

## Nagios

Nagios is a widely used open source infrastructure monitoring tool.

- Monitors hosts and services
- Network device monitoring
- Alerting and notification system
- Plugin-based extensibility

---

## Zabbix

Zabbix is an open source monitoring solution.

- Server and network monitoring
- Application monitoring
- Data visualization dashboards
- Customizable alerting

---

# ☁️ Cloud-Native Observability

## AWS CloudWatch

AWS CloudWatch is Amazon’s monitoring and observability service for AWS resources.

- Metrics collection
- Log monitoring
- Distributed tracing
- Alarm and notification system
- Deep integration with AWS services

---

## Azure Monitor

Azure Monitor is Microsoft Azure’s observability platform.

- Application monitoring
- Infrastructure health insights
- Metrics and log analysis
- Integration with Azure services

---

# 🏁 Summary

Observability tools can be categorized into:

- 📊 Metrics Monitoring
- 📝 Log Management
- 🔗 Distributed Tracing
- ⚡ Application Performance Monitoring
- 🏗 Infrastructure Monitoring
- ☁️ Cloud-Native Monitoring

Choosing the right tools depends on:

- Infrastructure type (cloud/on-prem)
- Application architecture (monolith/microservices)
- Scale requirements
- Budget and operational complexity
