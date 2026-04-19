# Day 05 – April 19, 2026 – AWS Databases

## Skills Learned:
- Amazon RDS: A managed relational database service supporting MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, and Aurora with automated backups, easy scaling, CloudWatch monitoring, and security features.
- RDS Read Replicas: Asynchronous read-only database copies for scaling read-heavy workloads; can improve performance and disaster recovery but are not substitutes for Multi-AZ high availability.
- RDS Multi-AZ Deployments: High availability through synchronous replication to a standby instance in another AZ with automatic failover and transparent application updates.
- RDS Events Notification: SNS-integrated alerts for database events (failover, maintenance, backup completion) enabling automated workflows and proactive monitoring.
- RDS Proxy: Fully managed database proxy offering connection pooling, automatic failover, and IAM authentication to improve scalability for serverless and unpredictable-traffic workloads.
- Amazon Aurora: Cloud-native relational database (MySQL/PostgreSQL-compatible) with 5x faster performance, auto-scaling storage (up to 128 TB), multi-AZ replication, and global databases for cross-region disaster recovery.
- Amazon DynamoDB: Fully managed NoSQL database with key-value and document models, single-digit millisecond latency, automatic scaling, global tables, streams for event processing, and flexible capacity modes.
- DynamoDB Core Components: Tables (data containers), items (records), attributes (fields), primary keys (partition key mandatory, sort key optional), indexes (GSI, LSI), and streams for event-driven architectures.
- DynamoDB Design Best Practices: Efficient key design for access patterns, GSI usage for flexible queries, and capacity/throughput monitoring and optimization.

## Labs/Exercises Completed:
- N/A (recorded notes and studied AWS database service capabilities).

## Key Takeaways:
- RDS is ideal for structured data and ACID compliance; choose Multi-AZ for production workloads requiring high availability and Read Replicas for scaling read-heavy workloads.
- Aurora provides higher performance and cost-efficiency than standard RDS engines while maintaining MySQL/PostgreSQL compatibility; consider for mission-critical applications.
- DynamoDB excels at massive scale, low latency access, and flexible schema; use for gaming, IoT, mobile apps, and event-driven architectures requiring global replication.
- RDS Proxy reduces connection overhead and supports serverless applications; consider for workloads with variable or unpredictable traffic patterns.
- Relational databases (RDS/Aurora) suit transaction processing; NoSQL (DynamoDB) suits high-throughput, distributed, and flexible-schema scenarios.
- Layer database resilience with backups, replication, multi-AZ deployments, and Read Replicas based on RPO/RTO requirements.

## Notes:
- Next: Explore caching strategies with ElastiCache and data warehouse solutions like Amazon Redshift.
- Consider building a proof-of-concept using Aurora for structured data and DynamoDB for session/profile data in the same application.
