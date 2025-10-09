# Topics covered in the document...

1. [What is Databricks and its architecture?](#1-what-is-databricks-and-its-architecture?)
2. [Accounts and workspace architecture](#2-accounts-and-workspace-architecture)
3. [Databricks workspace navigation](#3-databricks-workspace-navigation)
4. [Clusters: creation, configuration, and management](#4-clusters-creation-configuration-and-management)
5. [Notebooks: creating, organizing, and sharing](#5-notebooks-creating-organizing-and-sharing)
6. [Databricks Runtime and Unity Catalog overview](#6-databricks-runtime-and-unity-catalog-overview)



## 1. What is Databricks and its architecture?

### Answer
Databricks is a unified data analytics platform built on top of Apache Spark. It's a cloud-based platform that provides a collaborative environment for data engineers, data scientists, and analysts to work together on big data and machine learning projects.

Key Purpose: Databricks simplifies big data processing and makes it easier to build data pipelines, perform analytics, and create machine learning models at scale.

### Architecture

The Databricks architecture consists of two main planes:

#### 1. Control Plane (Managed by Databricks)
- Web Application/UI: The interface where you interact with Databricks.
- Cluster Manager: Manages cluster lifecycle (creation, termination, scaling)
- Notebook Server: Hosts collaborative notebooks
- Jobs scheduler: Orchestrates and schedules workflows
- Security & Access Control: Manages authentication and authorization
- Metadata Store: Stores information about databases, tables, and configurations

#### 2. Data Plane (Runs in Your Cloud Account)
- Compute Clusters: Apache Spark clusters that executes your code
  - Driver node (coordinates work)
  - Worker nodes (execute tasks)
- Cloud Storage: Where your actual data lives (S3, ADLS, GCS)
- Delta Lake Storage: Optimized storage layer with ACID transactions
###
![1.1. Databricks Architecture](image.png)

### Key Architectural Components
Workspaces: Isolated environments for organizing notebooks, libraries, and dashboards.

#### Clusters:
        - All-Purpose Clusters: Interactive work, development
        - Job Clusters: Automated production workloads (cost-effective)

- Notebooks: Interactive documents supporting Python, Scala, SQL, and R
- Delta Lake: Storage layer that brings reliability to data lakes (ACID transactions, time travel, schema enforcement)
- Unity Catalog: Centralized governance and metadata management across all workspaces
- DBFS (Databricks File System): Abstraction layer over cloud storage

## 2. Accounts and Workspace Architecture

### Answer
Account: 
The Databricks account represents the top-level management entity that is linked with a cloud provider account — such as an Azure subscription, AWS account, or GCP project.
It defines where billing, governance, and workspace management are handled.
In Azure, this means your Databricks setup is tied to your Azure subscription, and all Databricks resources are billed through Azure.

Workspace:
A Databricks workspace is a dedicated environment within your cloud account where teams can collaborate, write code, build data pipelines, and run machine learning models.
- Each workspace provides access to:
- Notebooks and repos for development
- Compute resources (clusters, jobs)
- Access control via Azure Active Directory or IAM

Workspaces are typically created per team, project, or environment (e.g., dev, test, prod) and allow users like Data Engineers, Data Scientists, and Analysts to work securely within their defined roles.


## 3. Databricks Workspace Navigation

### Answer


## 4. Clusters: Creation, Configuration, and Management

### Answer


## 5. Notebooks: Creating, Organizing, and Sharing

### Answer


## 6. Databricks Runtime and Unity Catalog Overview

### Answer
