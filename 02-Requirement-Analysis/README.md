# Phase 2: Requirement Analysis

## Project Title
Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Requirement Overview
The project requires an automated process in ServiceNow for handling Standard Laptop orders. The solution uses ServiceNow Flow Designer to automatically generate a Catalog Task for the Hardware team after the laptop request is approved.

## Functional Requirements

### 1. Standard Laptop Request
- Users should be able to request a Standard Laptop through the Service Catalog.
- The request should generate a Requested Item (RITM).

### 2. Approval Process
- The Standard Laptop request should go through an approval process.
- The automation should continue after the request is approved.

### 3. Flow Designer Automation
- A flow named `Standard laptop task` should be created.
- The flow should use the `Service Catalog` trigger.
- The application should be `Global`.
- The flow should run as `System User`.

### 4. Catalog Task Creation
After approval, the flow should automatically create a Catalog Task.

The Catalog Task should contain the following values:

| Field | Value |
|---|---|
| Table Name | Catalog Task [sc_task] |
| Requested Item | Trigger → Requested Item Record |
| Short Description | Laptop need to Configured |
| Description | Laptop need to Configured |
| Assignment Group | Hardware |
| Approval | Approved |

### 5. Flow Assignment
- The created flow should be assigned to the `Standard Laptop` catalog item.
- The flow should be configured through the Process Engine section.

## Non-Functional Requirements
- The process should reduce manual intervention.
- The automation should reduce delays in laptop configuration.
- The process should be reliable and consistent.
- The solution should improve IT procurement efficiency.
- The workflow should be easy to manage using ServiceNow Flow Designer.

## Software Requirements
- ServiceNow Instance
- ServiceNow Flow Designer
- Service Catalog
- Web Browser
- GitHub

## User Roles

### Requester
Places the Standard Laptop request through the Service Catalog.

### Approver
Reviews and approves the Standard Laptop request.

### Hardware Team
Receives the automatically generated Catalog Task and handles laptop configuration.

### Administrator
Creates and manages the Flow Designer automation and Service Catalog configuration.

## Expected Output
After the Standard Laptop request is approved, the ServiceNow Flow Designer automation should automatically create a Catalog Task.

The generated task should:
- Be linked to the requested item.
- Have the required short description and description.
- Be assigned to the `Hardware` group.
- Have the approval value set to `Approved`.

## Conclusion
The requirement analysis defines the functional and technical requirements needed to automate the Standard Laptop procurement process using ServiceNow Flow Designer.
