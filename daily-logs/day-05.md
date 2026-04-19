# AWS Databases - Study Notes

## 1. Amazon RDS Overview
- **Definition**: Amazon Relational Database Service (RDS) is a managed service for relational databases.
- **Supported Engines**: MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, Amazon Aurora.
- **Key Features**:
  - Automated backups and snapshots
  - Easy scaling (vertical and horizontal)
  - Monitoring via CloudWatch
  - Security with IAM, VPC, and encryption
- **Use Cases**: Simplifies database setup, operation, and scaling without manual administration.

---

## 2. Amazon RDS Read Replica
- **Purpose**: Provides read-only copies of a database for scaling read-heavy workloads.
- **Characteristics**:
  - Asynchronous replication from the primary DB
  - Multiple replicas supported
  - Can promote a replica to a standalone DB
- **Benefits**:
  - Improves performance by offloading read queries
  - Enhances availability and disaster recovery
- **Limitations**:
  - Replication lag possible
  - Not a substitute for Multi-AZ (which is for high availability)

---

## 3. Amazon RDS Multi-AZ Deployments
- **Definition**: Provides high availability by automatically replicating data to a standby instance in another Availability Zone.
- **Features**:
  - Synchronous replication
  - Automatic failover in case of primary DB failure
  - Transparent to applications
- **Benefits**:
  - Increased fault tolerance
  - Business continuity during outages
- **Best Practice**: Use for production workloads requiring high availability.

---

## 4. Amazon RDS Events Notification
- **Purpose**: Provides alerts for database events (e.g., failover, maintenance, backup completion).
- **Integration**:
  - Amazon SNS for notifications
  - Can trigger automated workflows
- **Examples of Events**:
  - Instance restart
  - Backup completion
  - Failover occurrence
- **Benefit**: Improves monitoring and proactive response to DB changes.

---

## 5. Amazon RDS Proxy
- **Definition**: A fully managed, highly available database proxy for RDS.
- **Features**:
  - Connection pooling
  - Automatic failover
  - IAM authentication
- **Benefits**:
  - Improves application scalability
  - Reduces connection overhead
  - Enhances security with IAM integration
- **Use Case**: Ideal for serverless applications or workloads with unpredictable traffic.

---

## 6. Amazon Aurora Overview
- **Definition**: A MySQL and PostgreSQL-compatible relational database built for the cloud.
- **Key Features**:
  - High performance (up to 5x faster than MySQL)
  - Auto-scaling storage (up to 128 TB)
  - Replication across multiple AZs
  - Global databases for cross-region replication
- **Benefits**:
  - Enterprise-grade performance at lower cost
  - Fault-tolerant and self-healing storage
- **Use Cases**: Mission-critical applications needing high throughput and resilience.

---

## 7. Amazon DynamoDB Overview
- **Definition**: A fully managed NoSQL database service.
- **Characteristics**:
  - Key-value and document data models
  - Single-digit millisecond latency
  - Scales automatically
- **Features**:
  - Global tables for multi-region replication
  - Streams for real-time event processing
  - On-demand and provisioned capacity modes
- **Use Cases**:
  - Gaming, IoT, mobile apps
  - Applications requiring massive scale and low latency

---

## 8. Amazon DynamoDB Core Components
- **Tables**: Primary container for data.
- **Items**: Individual records in a table.
- **Attributes**: Data fields within items.
- **Primary Key**:
  - Partition key (mandatory)
  - Sort key (optional, for composite keys)
- **Indexes**:
  - Global Secondary Index (GSI)
  - Local Secondary Index (LSI)
- **Streams**: Capture changes for event-driven architectures.
- **Best Practices**:
  - Design keys for efficient access patterns
  - Use GSIs for flexible queries
  - Monitor capacity and optimize throughput

---

# Summary
- **Amazon RDS**: Managed relational DB with features like Read Replicas, Multi-AZ, Proxy, and event notifications.
- **Amazon Aurora**: High-performance, cloud-native relational DB compatible with MySQL/PostgreSQL.
- **Amazon DynamoDB**: Fully managed NoSQL DB with scalability, low latency, and flexible data models.
