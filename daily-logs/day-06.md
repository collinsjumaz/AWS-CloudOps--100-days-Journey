# Day 6 – 20th April 2026 – AWS Monitoring & Management

## Skills Learned:
- **Amazon CloudWatch**: Monitoring and observability service for collecting metrics, tracking logs, setting alarms, and automating responses
- **EC2 Metrics**: CPU utilization, disk operations, network traffic, and status checks with 5-minute (default) or 1-minute (detailed) intervals
- **CloudWatch Alarms**: Setting thresholds and triggering automated actions (SNS, Auto Scaling, EC2 control)
- **Log Analysis**: Using metric filters to extract numerical metrics from logs for real-time analysis
- **Amazon EventBridge**: Event-driven service for routing real-time system events to targets like Lambda, SNS, SQS
- **AWS Systems Manager (SSM)**: Comprehensive service for viewing, managing, and operating infrastructure at scale
- **SSM Core Components**: Automation Documents, Parameter Store, Patch Manager, Session Manager, Inventory, State Manager, OpsCenter
- **Hybrid & Multicloud Management**: Managing EC2, on-premises servers, and VMs with unified dashboard

## Labs/Exercises Completed:
- Studied CloudWatch metrics collection and analysis for EC2 instances
- Reviewed alarm configuration and automation workflows
- Explored EventBridge routing and event-driven architecture
- Analyzed SSM capabilities for infrastructure automation
- Compared CloudWatch vs Systems Manager functionality and use cases

## Key Takeaways:
- **CloudWatch** is the monitoring backbone: metrics, logs, alarms, and events for AWS resources
- **Systems Manager** is the management toolkit: automation, compliance, secure access, and operational control
- **Detailed monitoring** should be enabled for production workloads (1-minute granularity)
- **SSM Agent** is required for Systems Manager to function across resources
- **Session Manager** provides secure, auditable remote access without SSH/RDP
- Together, CloudWatch + Systems Manager provide a complete operational toolkit for cloud environments
- Both services integrate with IAM for security and can work across hybrid/multicloud environments

## Notes:
- CloudWatch focuses on observability (what's happening)
- Systems Manager focuses on management (what to do about it)
- For incident response, combine OpsCenter (issue visibility) with Automation Runbooks (response execution)
- Consider Parameter Store for managing configuration and secrets securely
- Patch Manager can automate critical security updates across infrastructure at scale
- Next: Study AWS logging services, application insights, and container monitoring
