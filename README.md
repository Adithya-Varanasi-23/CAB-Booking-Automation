# CAB Booking Automation

A ServiceNow-based application designed to streamline Change Advisory Board (CAB) meeting scheduling, approval management, and booking lifecycle automation.

## Overview

Managing CAB meetings involves coordinating schedules, checking meeting availability, collecting approvals, and tracking booking requests associated with Change Requests.

The **CAB Booking Automation** application simplifies this process by providing a centralized platform where users can submit meeting requests, CAB Coordinators can review and approve requests, and the booking lifecycle can be managed through automated workflows.

This project demonstrates the practical application of ServiceNow capabilities within the **IT Service Management (ITSM)** domain, particularly Change Enablement.

## Key Features

- **CAB Meeting Requests:** Submit meeting requests linked to existing Change Requests.
- **Availability Validation:** Validate meeting dates and prevent overlapping bookings.
- **Approval Management:** Route booking requests to CAB Coordinators for approval or rejection.
- **Booking Dashboard:** View booking statistics, recent requests, and booking statuses.
- **My Bookings:** Search, filter, and manage submitted booking requests.
- **Cancellation Management:** Allow users to cancel confirmed bookings.
- **Rescheduling:** Submit rescheduling requests through an approval process.
- **Coordinator Dashboard:** Provide coordinators with visibility into assigned booking requests.
- **Lifecycle Notifications:** Support communication for important booking status changes.

## ServiceNow Technologies Used

| Technology | Purpose |
|---|---|
| Service Portal | Created a custom user interface for booking management. |
| Service Portal Widgets | Developed custom application components using HTML, CSS, and AngularJS. |
| Flow Designer | Automated booking approvals and lifecycle workflows. |
| Business Rules | Implemented server-side validations and scheduling conflict checks. |
| Custom Tables | Stored and managed CAB booking information. |
| Access Control Lists (ACLs) | Controlled access to application records and operations. |
| User Roles and Groups | Managed requester and CAB Coordinator access. |
| Notifications | Supported booking-related communication. |

## Application Workflow

1. **Request Submission:** A user selects a Change Request and enters the proposed meeting schedule, agenda, and location.
2. **Schedule Validation:** Business Rules validate the meeting dates and check for scheduling conflicts.
3. **Approval Routing:** Flow Designer routes the booking request to the CAB Coordinators.
4. **Approval Decision:** The coordinator reviews the request and approves or rejects it.
5. **Status Management:** The booking status is updated based on the approval outcome.
6. **Booking Lifecycle:** Users can cancel confirmed bookings or submit rescheduling requests for approval.

## Architecture

The application follows a ServiceNow platform-based architecture:

```text
              Users
                |
                v
       Service Portal UI
                |
                v
       Custom Portal Widgets
                |
                v
       ServiceNow Server Logic
          /           \
         v             v
   Business Rules   Custom Tables
         |             |
         v             v
  Availability      CAB Booking
   Validation         Records
                         |
                         v
                    Flow Designer
                         |
                         v
                  CAB Coordinator
                         |
                         v
                 Approval Decision
                         |
                         v
                 Booking Status
```

## ITSM Relevance

This project is aligned with the **IT Service Management (ITSM)** domain and supports Change Enablement processes.

CAB meetings play an important role in reviewing proposed changes, evaluating risks, discussing implementation plans, and making approval decisions before changes are implemented.

The application helps organize this process by connecting CAB meeting requests with Change Requests and automating the associated scheduling and approval activities.

## Screenshots

Add screenshots of your actual application in this section.

Suggested screenshots:

1. Dashboard Overview
2. New CAB Booking Form
3. My Bookings Page
4. Coordinator Dashboard
5. Approval Workflow
6. Booking Status After Approval

Store the screenshots in a folder named `screenshots` in this repository.

Example:

```text
CAB-Booking-Automation/
│
├── screenshots/
│   ├── dashboard.png
│   ├── new-booking.png
│   ├── my-bookings.png
│   ├── coordinator-dashboard.png
│   └── approval-workflow.png
│
└── README.md
```

## Learning Outcomes

Developing this application provided practical experience in:

- Building scoped applications on the ServiceNow platform.
- Developing custom Service Portal widgets.
- Implementing server-side validation using Business Rules.
- Designing complex Flow Designer approval workflows.
- Managing application access through roles and ACLs.
- Understanding ITSM processes and Change Enablement.
- Handling booking lifecycle scenarios, including cancellation and rescheduling.

One of the most valuable aspects of this project was working deeply with complex Flow Designer workflows, particularly approval routing, conditional outcomes, and lifecycle automation.

## Future Enhancements

- Improve responsive design for mobile devices.
- Add advanced reporting and booking analytics.
- Enhance concurrent booking validation.
- Expand automated notifications and audit visibility.

## Project Information

**Project:** CAB Booking Automation  
**Platform:** ServiceNow  
**Domain:** IT Service Management (ITSM)  
**Focus:** Change Enablement and Workflow Automation  
**Developer:** Adithya

---

*This is my second ServiceNow project, built to gain hands-on experience with ServiceNow application development, ITSM processes, and complex workflow automation.*
