# Data Architectures

Understanding data architecture is fundamental in designing systems that are scalable, efficient, and reliable for managing data across an organization.

---

## 📘 What is Data Architecture?

Data Architecture defines how data is collected, stored, processed, and accessed within a system. It includes the models, policies, rules, and standards that govern which data is collected, how it is stored, arranged, integrated, and used.

---

## 🏗️ Common Data Architecture Types

### 1. Data Warehouse

- **Purpose**: Centralized repository for structured data used in analytics and reporting.
- **Examples**: Amazon Redshift, Google BigQuery, Snowflake
- **Characteristics**:
  - Schema-on-write
  - Optimized for complex queries (OLAP)
  - Batch data loading
- **Use Cases**:
  - Business Intelligence
  - Dashboards and KPIs

---

### 2. Data Lake

- **Purpose**: Centralized storage for raw, unstructured, semi-structured, and structured data.
- **Examples**: AWS S3, Azure Data Lake, Hadoop HDFS
- **Characteristics**:
  - Schema-on-read
  - Cost-effective and scalable
  - Supports big data processing
- **Use Cases**:
  - Machine Learning
  - Data Exploration
  - Historical data storage

---

### 3. Lakehouse

- **Purpose**: Combines the best of Data Lakes and Data Warehouses.
- **Examples**: Databricks Lakehouse, Delta Lake, Apache Iceberg
- **Characteristics**:
  - Supports ACID transactions
  - Handles both structured and unstructured data
  - Unified platform for BI + ML
- **Use Cases**:
  - Real-time analytics and AI on the same platform

---

### 4. Data Mesh

- **Purpose**: Decentralized architecture that treats data as a product and distributes ownership to domain teams.
- **Characteristics**:
  - Domain-oriented data ownership
  - Self-serve data infrastructure
  - Strong data governance
- **Use Cases**:
  - Large organizations with multiple data domains
  - Scalable data operations

---

### 5. Data Fabric

- **Purpose**: Abstracted architecture to manage and integrate data across environments, platforms, and locations.
- **Characteristics**:
  - Metadata-driven
  - Automation and AI-enabled data integration
  - Works across hybrid/multi-cloud setups
- **Use Cases**:
  - Enterprise-wide data integration
  - Real-time insights from distributed sources

---

## 🧭 Choosing the Right Architecture

| Criteria                | Warehouse | Lake | Lakehouse | Mesh | Fabric |
|------------------------|-----------|------|-----------|------|--------|
| Structured Data        | ✅        | ✅   | ✅        | ✅   | ✅     |
| Unstructured Data      | ❌        | ✅   | ✅        | ✅   | ✅     |
| Real-time Processing   | ⚠️        | ✅   | ✅        | ✅   | ✅     |
| Decentralized Ownership| ❌        | ❌   | ⚠️        | ✅   | ⚠️     |
| Governance Focus       | ✅        | ⚠️   | ✅        | ✅   | ✅     |

⚠️ = possible depending on implementation.

---

## 📚 References

- [What is a Data Warehouse?](https://en.wikipedia.org/wiki/Data_warehouse)  
- [Data Lake vs Data Warehouse](https://databricks.com/glossary/data-lake-vs-data-warehouse)  
- [The Rise of the Lakehouse Architecture](https://databricks.com/blog/2020/01/30/what-is-a-data-lakehouse.html)  
- [Data Mesh Principles](https://martinfowler.com/articles/data-mesh-principles.html)  
- [Data Fabric: An Architecture for Modern Data Management](https://www.gartner.com/en/articles/data-fabric-is-the-future-of-data-management)
