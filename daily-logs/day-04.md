# Day 04 – March 15, 2026 – AWS Application Integration & Security Services

## Skills Learned:
- AWS messaging for decoupling systems (SQS/SNS, Step Functions, EventBridge, AppSync, AppFlow).
- SQS: difference between Standard queues (high throughput, at-least-once, possible duplicates) and FIFO queues (ordered, exactly-once, lower throughput); how queue depth/age can drive Auto Scaling.
- SNS: pub/sub notification service with topics that can fan out to SQS, email, SMS, etc., with message filtering so subscribers only receive relevant messages.
- Step Functions: orchestration of Lambda (and other services) into visual state machines for complex workflows.
- Amazon MQ: managed ActiveMQ broker for protocol-compatible messaging (JMS, NMS, AMQP, MQTT, WebSockets) when standard AWS services aren’t a fit.
- Event-driven and data-integration services (EventBridge, AppSync, AppFlow).
- AWS security services:
  - Protecting applications and against DDoS (WAF, Firewall Manager, Shield).
  - Threat detection, investigation, and vulnerability management (GuardDuty, Inspector, Detective).
  - Keys, secrets, and sensitive data protection (CloudHSM, KMS, Secrets Manager, Macie, ACM).
- AWS management and governance services:
  - Day-to-day control via the Management Console, CLI, Mobile App, and Systems Manager (patching/configuration/automation).
  - Resource sharing and centralization with Resource Access Manager (RAM) across accounts.
  - Governance and compliance at scale with Config, Organizations, Service Catalog, and Control Tower.

## Labs/Exercises Completed:
- N/A (recorded notes and compared AWS integration/security service capabilities).

## Key Takeaways:
- Decoupling with messaging (SQS/SNS) improves scalability and resilience, and enables Auto Scaling based on queue metrics.
- Choose FIFO queues when ordering and exactly-once processing matter; choose Standard for throughput and loose ordering.
- EventBridge is the central serverless event bus for connecting AWS services and SaaS apps in an event-driven architecture.
- AppSync and AppFlow offer managed ways to integrate and query data across services and external apps.
- AWS security is layered: web/app protection (WAF/Shield), threat detection (GuardDuty/Inspector/Detective), and strong key/secret management (KMS/CloudHSM/Secrets Manager/Macie/ACM).
- Effective governance and operations require centralized tools (Systems Manager, Control Tower, Organizations, Config) and shared resources (RAM) to avoid configuration drift and reduce duplication.

## Notes:
- Next: Build a small event-driven prototype using SNS -> SQS -> Lambda, and optionally integrate Step Functions for orchestration.
- Explore a simple EventBridge rule that routes AWS service events to a Lambda target.
