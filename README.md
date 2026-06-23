# Automated Network Request Management (ANRM)

## Overview

Automated Network Request Management (ANRM) is a ServiceNow-based workflow automation project developed to streamline the process of requesting, approving, assigning, and fulfilling network-related service requests within an organization.

The system replaces manual email-based processes with a centralized, automated workflow that allows employees to submit network requests, department heads to approve them, and network engineers to execute and track assigned tasks.

The solution improves visibility, accountability, and operational efficiency by integrating Record Producers, Flow Designer, Service Catalog, approvals, task assignment, notifications, reports, and dashboards.

---

## Problem Statement

Organizations often manage network access requests manually through emails, spreadsheets, and phone calls. This process leads to:

* Delays in approval cycles
* Lack of request tracking
* Duplicate requests
* Poor visibility into request status
* Increased administrative workload
* Difficulty in monitoring SLA compliance

ANRM addresses these issues by automating the complete request lifecycle.

---

## Objectives

* Automate network service request handling.
* Implement approval workflows.
* Route approved requests to network engineers.
* Track request fulfillment activities.
* Generate reports and dashboards.
* Improve transparency and accountability.

---

## Features

### Request Submission

Employees can submit network service requests using a Record Producer.

Supported request types:

* VPN Access
* Firewall Change
* WiFi Access
* Internet Access
* LAN Port Activation
* Network Troubleshooting

### Dynamic Form Behaviour

The form dynamically displays fields based on the selected Request Type.

Examples:

#### VPN Access

Fields displayed:

* Access Level
* Device Type
* Device Name
* Start Date
* End Date

#### Firewall Change

Fields displayed:

* IP Address
* Port Number

#### WiFi Access

Fields displayed:

* Device Type
* Device Name

#### Internet Access

Fields displayed:

* Website URL

#### LAN Port Activation

Fields displayed:

* Building
* Floor
* Desk Number
* Port Number

#### Network Troubleshooting

Fields displayed:

* Device Type
* Device Name
* Issue Description

---

## Workflow

### Step 1: Employee submits request

User submits a Network Request through Service Portal.

↓

### Step 2: Head approval

Request is sent to the department head for approval.

Actions:

* Approve
* Reject

↓

### Step 3: Network engineer assignment

Approved requests are assigned to the Network Team.

↓

### Step 4: Engineer fulfillment

The Network Engineer:

* Views assigned requests
* Updates work notes
* Changes request state
* Marks work as completed

↓

### Step 5: Notifications

Email notifications are sent during:

* Approval request
* Approval success
* Approval rejection
* Work completion

---

## System Architecture

```text
Employee
   ↓
Record Producer
   ↓
Head Approval
   ↓
sc_request
   ↓
Network Request (NREQ)
   ↓
Network Engineer
   ↓
Completion Notification
```

---

## Modules Implemented

### Employee

* Submit Network Request
* View Submitted Requests

### Department Head

* Pending Approvals
* Approval Actions

### Network Engineer

* My Assigned Requests
* Update Work Notes
* Update State

### Administrator

* All Network Requests
* Reports
* Dashboards

---

## ServiceNow Components Used

### Catalog Management

* Record Producer

### Flow Designer

* Approval Flow
* Assignment Flow
* Notification Flow

### Service Catalog

* Request Management

### User Management

* Users
* Groups
* Roles

### Automation

* Client Scripts
* UI Policies

### Reporting

* Reports
* Dashboards

---

## Roles

### Employee

Responsibilities:

* Submit requests
* Track requests

### Department Head

Responsibilities:

* Approve or reject requests

### Network Engineer

Responsibilities:

* Fulfill assigned requests
* Update work notes
* Complete tasks

### Administrator

Responsibilities:

* Configure workflows
* Monitor performance
* Generate reports

---

## Technologies Used

### Platform

* ServiceNow Personal Developer Instance (PDI)

### ServiceNow Modules

* Service Catalog
* Flow Designer
* Service Portal(Record Producers)
* User Administration
* Reports
* Dashboards

### Scripting

* JavaScript
* Glide API

---

## Project Structure

```text
ANRM
│
├── Record Producer
├── Approval Flow
├── Engineer Fulfillment Flow
├── Client Scripts
├── UI Policies
├── Email Notifications
├── Reports
├── Dashboards
└── Documentation
```

---

## Future Enhancements

* SLA monitoring
* Automatic escalation
* Mobile support
* Knowledge base integration
* Performance analytics
* Multi-level approvals
* Virtual Agent integration

---

## Benefits

* Reduced manual effort
* Faster approvals
* Improved accountability
* Better tracking
* Centralized management
* Enhanced visibility
* Increased operational efficiency

---

## Project Demonstration

Drive Link:

`https://drive.google.com/your-demo-link`


## GitHub Repository

Repository Name:

`Automated-Network-Request-Management`

---

## Author

**Yuvaraj Ethiraj**

ServiceNow Developer | Electronics and Communication Engineering Student

---

## License

This project is developed for academic and educational purposes.

