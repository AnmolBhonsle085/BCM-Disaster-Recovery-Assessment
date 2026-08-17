**BCM & Disaster Recovery Assessment**
**Project Overview**

This project demonstrates a Business Continuity Management (BCM) and Disaster Recovery (DR) assessment for a simulated SaaS organization.

The assessment focuses on identifying critical business services, analyzing the impact of disruptions, defining recovery objectives, assessing disaster scenarios, and developing recovery strategies.

Note: The organization and IT environment used in this project are simulated for educational and portfolio purposes. This is not a real client assessment, external audit, or certification engagement.

**Objectives**

Identify critical business services and IT assets
Perform a Business Impact Analysis (BIA)
Define Recovery Time Objective (RTO) and Recovery Point Objective (RPO)
Identify potential disaster scenarios
Assess business and IT risks
Develop backup and recovery strategies
Create a Disaster Recovery Plan
Perform a controlled recovery test
Document findings and recommendations

**Simulated Organization**

Organization: SecureTech Solutions Pvt. Ltd.
Industry: Software as a Service (SaaS)
Employees: 100
Customers: 5,000
Location: Pune, India

The organization provides an online SaaS application that customers depend on for accessing business services.

**IT Environment**

The simulated environment consists of:

Customer Web Application
Database Server
File Storage
Employee Laptops
Email Service
Network Connectivity
Security/System Monitoring
Backup Storage
High-Level Architecture
                    INTERNET
                        |
                        ↓
                Web Application
                        |
                        ↓
                    Database
                        |
                ┌───────┴───────┐
                ↓               ↓
          File Storage       Monitoring
                                |
                           Security Logs
                           
**Business Impact Analysis**

The Business Impact Analysis identifies the effect of an IT service becoming unavailable.

Critical services include:

Service	Criticality	Maximum Tolerable Downtime
Database	Critical	1 hour
Customer Web Application	Critical	2 hours
File Storage	High	4 hours
Email	High	8 hours
Employee Laptops	High	1 business day

The database and customer-facing application receive the highest recovery priority because their unavailability directly affects customers and business operations.

**RTO & RPO**

RTO (Recovery Time Objective) defines how quickly a service should be restored.

RPO (Recovery Point Objective) defines the maximum acceptable amount of data loss.

Example targets:

Service	RTO	RPO
Database	1 hour	15 minutes
Web Application	2 hours	30 minutes
File Storage	4 hours	1 hour
Email	8 hours	4 hours

These targets are simulated requirements for the project.

**Disaster Scenarios**

The following scenarios were assessed:

Database Server Failure
Database becomes unavailable or corrupted.
Recovery involves restarting/failing over the service or restoring a clean backup.
Ransomware Attack
Systems or files become encrypted.
Recovery involves isolating affected systems and restoring from clean backups.
Accidental Data Deletion
Important files or database records are accidentally deleted.
Recovery involves restoring from an appropriate backup or version.
Cloud Service Outage
Cloud-hosted services become unavailable.
Recovery involves activating an alternate recovery environment or provider-supported recovery process.
Network Outage
Network connectivity becomes unavailable.
Recovery involves alternate connectivity and network-provider escalation.
Power Outage
Local infrastructure loses power.
Recovery involves backup power and alternate working arrangements.

**Risk Assessment**

Each disaster scenario is evaluated based on:

Likelihood
Business impact
Risk rating
Existing/proposed controls
Risk treatment
Recovery strategy

Example:

Risk: Database failure
Likelihood: Medium
Impact: High
Risk Rating: High
Treatment: Backup and recovery testing

**Backup & Recovery Strategy**

The project proposes:

Scheduled database backups
Incremental/frequent backups where supported
Separate recovery copies
Restricted access to backups
Backup monitoring
Periodic restoration testing
Isolated or immutable backup copies where feasible

A backup is not considered reliable simply because it exists. Restoration must be tested to verify that the data can actually be recovered.

**Disaster Recovery Plan**

The DR plan defines the recovery process for critical failures.

Example: Database Failure
Detect Failure
      ↓
Investigate
      ↓
Confirm Database Unavailable
      ↓
Activate DR Procedure
      ↓
Identify Latest Clean Backup
      ↓
Restore Database
      ↓
Validate Database
      ↓
Reconnect Application
      ↓
Test Application
      ↓
Resume Service
      ↓
Document Recovery

The plan also defines recovery responsibilities, escalation, validation, and post-recovery documentation.

**Recovery Test**

A controlled recovery test should be performed using non-production sample data.

Test Scenario

Accidental deletion of sample data

Test Process
Create Sample Data
       ↓
Create Backup
       ↓
Simulate Data Deletion
       ↓
Detect Failure
       ↓
Restore Backup
       ↓
Verify Data
       ↓
Record Recovery Time

The following should be recorded:

Failure/simulation time
Detection time
Recovery start time
Recovery completion time
Actual recovery duration
Latest recoverable backup
Data recovered
Data lost, if any
Whether RTO/RPO targets were achieved

Actual test results and screenshots should be added after performing the test. No fabricated evidence should be used.

**Project Structure**

BCM-DR-Assessment/
│
├── README.md
│
├── 01_Project_Scope.docx
├── 02_Organization_Profile.xlsx
├── 03_IT_Environment.xlsx
├── 04_Business_Impact_Analysis.xlsx
├── 05_RTO_RPO_Matrix.xlsx
├── 06_Disaster_Scenarios.xlsx
├── 07_Risk_Register.xlsx
├── 08_Backup_Strategy.docx
├── 09_Disaster_Recovery_Plan.docx
├── 10_DR_Test_Report.docx
│
├── Evidence/
│   ├── backup-created.png
│   ├── simulated-failure.png
│   ├── restore-process.png
│   └── recovery-success.png
│
└── BCM_DR_Assessment_Report.pdf

**Key Findings & Recommendations**

Based on the assessment, the organization should:

Maintain regular backups of critical data
Store recovery copies separately from production
Restrict access to backup systems
Regularly test backup restoration
Document recovery responsibilities
Maintain disaster recovery procedures
Periodically review RTO/RPO requirements
Test recovery procedures through controlled exercises
Update the DR plan based on lessons learned

**Skills Demonstrated**

Business Continuity Management (BCM)
Disaster Recovery (DR)
Business Impact Analysis (BIA)
Risk Assessment
Risk Register
RTO & RPO
Backup & Recovery
Disaster Scenario Analysis
Recovery Planning
Documentation
GRC Concepts

**Disclaimer**

This project is a simulated educational portfolio project. The organization, business requirements, IT environment, RTO/RPO values, and scenarios are illustrative. The project does not represent an assessment, audit, or consulting engagement performed for a real organization.
