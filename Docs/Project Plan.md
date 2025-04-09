## Index

- [Project Plan](#project-plan)
  - [1. Project Overview](#1-project-overview)
  - [2. Project Objectives](#2-project-objectives)
  - [3. Project Scope](#3-project-scope)
    - [**In Scope**](#in-scope)
    - [**Out of Scope**](#out-of-scope)
  - [4. Project Milestones \& Deliverables](#4-project-milestones--deliverables)
  - [5. Project Schedule](#5-project-schedule)
    - [5.1 WBS Structure](#51-wbs-structure)
    - [5.2 Gantt Chart or Timeline](#52-gantt-chart-or-timeline)
  - [6. Risk, Assumptions and Dependency Management](#6-risk-assumptions-and-dependency-management)
  - [7. Roles and Responsibilities](#7-roles-and-responsibilities)
  - [8. Project Methodology](#10-project-methodology)


# Project Plan

## 1. Project Overview

**Project Name:** Tazama Fraud Management System  

**Client:** Comesa Business Council  

**Project Manager:** Usama Abdul Mannan  

**Start Date:** March 01, 2025

**End Date:** December 31, 2025

**Key Stakeholders:** Linux Foundation, CBC, Tazama, Mojaloop Implementation Partner & Paysys Labs



## 2. Project Objectives
- Develop and deliver the Tazama Fraud Management System integrated with the Mojaloop Retail Banking System.
- Enhance fraud detection and prevention for the Comesa Business Council.
- Ensure secure and reliable financial transactions within retail banking operations.

## 3. Project Scope

### **In Scope:** 

- Data integration SDK
- Relay Service Enhancement
- Case and Investigation Management

    - Triage Module

    - Case Management Module

    - Investigation Module
- Data Warehouse
- Business Intelligence, Analytics and Reporting

    - Detection performance reporting

    - Anomaly detection

- Model Management

    - Rule development and deployment SDK

- Simulation sandbox
- Non-Functional Requirements
    - Auditability
    - Identity and Access Management
    - Protection of Personally Identifiable Information
    - Data security
    - Multi-Tenancy
    - ISO27001 Compliance

- A Joint Application Development (JAD) workshop with Mojaloop to define the integration between Mojaloop and Tazama – Assignment of development responsibilities to follow the JAD workshop.

### **Out of Scope:** 

- Model Management - Configuration Module
- Calibration service, including the use of AI/ML to fine-tune typologies
- Implementation
- Requirements elicitation and documentation for COMESA implementation
- Elicitation of COMESA compliance and regulatory stakeholder requirements
- Mediating agreement between sovereign stakeholders on regulations and policy
    - Data integration via SDK
    - Integration from Tazama to Mojaloop via Kafka
    - Modification of Mojaloop to handle Tazama blocking instructions
    - Identification of COMESA-specific rules and typologies
    - COMESA-specific rules development via SDK
    - Implementation of COMESA-specific compliance requirements
    - Configuration of COMESA-specific case management workflows
    - Implementation-specific regulatory reporting
    - Implementation-specific administrative reporting
    - Deployment of Tazama onto COMESA infrastructure
    - User setup
- Non-core enhancements
    - AI/ML fraud detection in real-time
- Operationalization
    - Definition and implementation of the COMESA operating environment
    - Ongoing maintenance and support of COMESA implementation
    - Ongoing production operation of Tazama and related applications
    - Onboarding of new participants/DFSPs

## 4. Project Milestones & Deliverables

- **Milestone 1: Project Kickoff & JAD Workshop**
    - **Deliverables:**
        - Project plan, Resource Allocations, Risk Management Plan  
        - Outcomes from JAD workshop (who’s responsible for Mojaloop integration steps, if any)  
        - Initial agreement on how Paysys will hand off deliverables to Tazama

-  **Milestone 2: System Architecture and Design**

    - **Deliverables:**
        - Signed-off architecture & design documentation (including data models, integration points, workflow diagrams)  
        - Security design approach finalized (authentication, encryption, PII handling, ISO27001 alignment)

- **Milestone 3: Development Phase 1 - Data Integration SDK**
    - **Deliverables:**
      - Working Data Integration SDK featuring the functionality in Section 2.1  
      - Documentation for how Tazama can integrate historical or real-time data sources

- **Milestone 4: Development Phase 2 - Relay Service**
  - **Deliverables:**
    - Configured Relay Service with Kafka + REST capabilities (as per Section 2.2)  
    - Demonstration of tested message flow, including security context (Keycloak)

- **Milestone 5: Development Phase 3 - Triage Module**
  - **Deliverables:**
    -	Triage Module for receiving alerts via REST + NATS, grouping/classifying them
    - Auto-association of alerts with active/resolved cases, auto-complete logic for low-priority alerts

- **Milestone 6: Development Phase 4 - Case Management System**
  - **Deliverables:**
    - Case Management System aligned with Section 2.3.2  
    - Documented workflows for standard use; user roles & privileges, notifications, auditing
 
- **Milestone 7: Development Phase 5 - Investigation Module**
  - **Deliverables:**
    - Investigation Module as described in Section 2.3.3  
    - Secure file storage, chain-of-custody tracking, and in-system collaboration (internal or with regulators)

- **Milestone 8: Development Phase 6 - Data Warehouse & BI/Analytics**
  - **Deliverables:**    
    - Data warehouse with replication from Tazama operational data (2.4)  
    - Basic dashboards or reports for detection performance & anomaly analysis (2.5.1 & 2.5.2)

- **Milestone 9: Development Phase 7 - Model Management, Sandbox, Multi-Tenancy**
  - **Deliverables:**
    - Rule Dev & Deployment toolkit plus Sandbox (2.6 & 2.7)  
    - Multi-tenant environment setup (2.8), data security & compliance checks (2.9)

- **Milestone 10: Final Acceptance - Turnover to Tazama**
  - **Deliverables:**    
    - Final acceptance by Tazama (covering all SOW scope)  
    - Delivery of all code, documentation, and any remaining BRDs  
    - UAT or E2E validation from Tazama and sign-off.  
    - Closure sign-off to confirm Paysys fulfilled the development scope

## 5. Project Schedule

### 5.1 WBS Structure:

All the deliverables are outlined in the **Project Deliverables and Milestones** section. The WBS structure provides a high-level breakdown of work required to achieve these milestones.  

For a detailed breakdown of development tasks, refer to the **GitHub Project Board**, where all task-level activities, dependencies, and progress tracking are available:  

🔗 **GitHub Project Board:** [https://github.com/orgs/frmscoe/projects/44/views/2](https://github.com/orgs/frmscoe/projects/44/views/2)

### 5.2 Gantt Chart or Timeline:
- A detailed visual representation of the schedule in the form of Gantt Chart is available on Github Project Board:
    - Link: https://github.com/orgs/frmscoe/projects/44/views/11?sortedBy%5Bdirection%5D=asc&sortedBy%5BcolumnId%5D=Milestone


## 6. Risk, Assumptions and Dependency Management

- All risks, assumptions & dependencies must be logged in **Asana** for immediate team review. 
  - **RAID LOG COMESA PROJECT** (https://app.asana.com/1/9283783873717/project/1209497261723580/dashboard/1209497280037571) will be followed, as prescribed by the **Linux Foundation**
- A detailed **Risk Management Plan** is developed separately and can be seen here: https://github.com/frmscoe/pmo/issues/13


## 7. Roles and Responsibilities

The list of resources with details including their Name, Email, Role & Organization can be seen on [Governance Plan](https://github.com/frmscoe/pmo/issues/11). 

## 8. Project Methodology
- Please refer to [Project Governance Plan](https://github.com/frmscoe/pmo/issues/11) for further details.
