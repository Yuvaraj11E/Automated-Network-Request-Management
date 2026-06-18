# Automated Network Request Management (ANRM)

## Project Overview

Automated Network Request Management (ANRM) is a ServiceNow-based workflow automation solution designed to streamline the lifecycle of network-related service requests within an organization.

The system replaces manual email-based processes with a centralized self-service portal that automates request submission, approvals, task assignment, SLA tracking, notifications, and reporting.

The project enables employees to request network services while allowing administrators and IT teams to efficiently manage, monitor, and fulfill those requests.

---

## Features

### User Features

* Submit network-related requests through a self-service portal
* Dynamic request forms based on request type
* Real-time request status tracking
* Receive email notifications for request updates

### Administrator Features

* Review and manage submitted requests
* Approve or reject requests
* Automatically assign tasks to network teams
* Monitor SLA compliance
* Generate reports and dashboards

### Automation Features

* Automated approval workflows
* Catalog task generation
* SLA tracking
* Email notifications
* Dashboard analytics

---

## Supported Request Types

The application currently supports six network request categories:

1. VPN Access Request
2. Firewall Rule Change Request
3. Network Drive Access Request
4. Wi-Fi Access Request
5. Network Device Configuration Request
6. IP Address Allocation Request

---

## Project Workflow

```text
User

↓

Service Portal

↓

Record Producer

↓

Network Request Table

↓

Flow Designer

↓

Approval Process

↓

Catalog Task Creation

↓

SLA Tracking

↓

Notifications

↓

Reports & Dashboards
```

---

## System Architecture

```text
                   +----------------+
                   | Service Portal |
                   +--------+-------+
                            |
                            |
                   +--------v--------+
                   | Record Producer |
                   +--------+--------+
                            |
                            |
                   +--------v--------+
                   | Network Request |
                   | (Custom Table)  |
                   +--------+--------+
                            |
                  -------------------------
                  |           |           |
                  |           |           |
         +--------v--+ +------v-----+ +---v--------+
         | Approval  | | Catalog    | | Notification|
         | Workflow  | | Tasks      | | System      |
         +--------+--+ +------+-----+ +------+------+
                  |           |              |
                  |           |              |
                  +-----------+--------------+
                              |
                      +-------v-------+
                      | SLA Tracking  |
                      +-------+-------+
                              |
                      +-------v-------+
                      | Reports &     |
                      | Dashboards    |
                      +---------------+
```

---

## Technology Stack

| Component       | Technology                 |
| --------------- | -------------------------- |
| Platform        | ServiceNow                 |
| User Interface  | Service Portal             |
| Workflow Engine | Flow Designer              |
| Database        | ServiceNow Tables          |
| Approvals       | ServiceNow Approval Engine |
| Notifications   | Email Notifications        |
| SLA Management  | Task SLA                   |
| Reporting       | Reports & Dashboards       |

---

## Project Structure

```text
Automated-Network-Request-Management/

├── README.md

├── Documentation/
│   ├── Project_Report.pdf
│   ├── Architecture_Diagram.png
│   ├── Data_Model_Diagram.png
│   └── Screenshots/

├── ServiceNow/
│   ├── Record_Producers/
│   ├── Catalog_Client_Scripts/
│   ├── UI_Policies/
│   ├── Flow_Designer/
│   ├── Notifications/
│   ├── SLAs/
│   ├── Reports/
│   └── Dashboards/

└── Demo/
    └── Project_Demo.mp4
```

---

## Functional Modules

### Service Portal

Provides a user-friendly interface for employees to submit requests.

### Record Producer

Captures network request information and creates records automatically.

### Approval Workflow

Routes requests to managers or administrators for approval.

### Catalog Tasks

Creates implementation tasks for network teams.

### SLA Management

Tracks request completion time and SLA compliance.

### Notifications

Sends automated email updates.

### Reports & Dashboards

Provides insights into requests, approvals, task performance, and SLA metrics.

---

## Data Model

### Main Entities

* User
* Network Request
* Approval
* Catalog Task
* SLA
* Notifications
* Reports

Relationships:

```text
User

↓

Network Request

↓

Approval

↓

Catalog Task

↓

SLA

↓

Notifications

↓

Reports
```

---

## Testing

The following functionalities were tested successfully:

* Request submission
* Approval and rejection flow
* Task generation
* SLA tracking
* Notification delivery
* Dashboard updates

---

## Advantages

* Reduces manual work
* Faster approval process
* Centralized request management
* Improved visibility
* Better SLA compliance
* Automated notifications
* Enhanced reporting

---

## Future Enhancements

* AI-based request prioritization
* Predictive SLA analysis
* Virtual Agent integration
* Mobile application support
* Multi-level dynamic approvals
* Advanced analytics

---

## Screenshots

Add screenshots for:

* Service Portal
* Record Producer
* Approval Screen
* Flow Designer
* Catalog Tasks
* SLA Tracking
* Notifications
* Reports
* Dashboards

---

## Project Demonstration

Add your project demo video link here.

Example:

`https://drive.google.com/your-demo-link`

---

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

