# Phase 7: Project Documentation

## Project Title
Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Project Overview
This project automates the Standard Laptop procurement process using ServiceNow Flow Designer.

The automation creates a Catalog Task and assigns it to the Hardware team after the Standard Laptop request is approved.

## Problem Statement
The existing IT procurement process involves manual activities that can cause delays and additional workload while handling Standard Laptop orders.

The project addresses this problem by automating Catalog Task creation and task assignment using ServiceNow Flow Designer.

## Project Objective
The main objectives of the project are:

- Automate the Standard Laptop procurement workflow.
- Reduce manual intervention.
- Reduce delays in laptop configuration.
- Automatically create Catalog Tasks.
- Assign configuration tasks to the Hardware team.
- Improve overall IT procurement efficiency.

## Technology Used
- ServiceNow
- ServiceNow Flow Designer
- Service Catalog
- Catalog Tasks
- GitHub

## Flow Configuration

| Configuration | Value |
|---|---|
| Flow Name | Standard laptop task |
| Application | Global |
| Run As | System User |
| Trigger | Service Catalog |
| Action | Create Catalog Task |

## Catalog Task Configuration

| Field | Value |
|---|---|
| Table Name | Catalog Task [sc_task] |
| Requested Item | Trigger → Requested Item Record |
| Short Description | Laptop need to Configured |
| Description | Laptop need to Configured |
| Assignment Group | Hardware |
| Approval | Approved |

## Implementation Process

1. Created a new Flow in ServiceNow Flow Designer.
2. Configured the Service Catalog trigger.
3. Added the Create Catalog Task action.
4. Configured the Catalog Task fields.
5. Saved and activated the flow.
6. Assigned the flow to the Standard Laptop Catalog Item.
7. Placed a Standard Laptop order through the Service Catalog.
8. Approved the generated request.
9. Verified the automatically generated Catalog Task.
10. Confirmed that the task was assigned to the Hardware group.

## Project Workflow

Standard Laptop Request  
→ Request Created  
→ Approval Process  
→ Request Approved  
→ Flow Designer Triggered  
→ Catalog Task Created  
→ Hardware Group Assigned  
→ Laptop Configuration

## Testing

The project was tested by placing a Standard Laptop request and completing the approval process.

The automation successfully created a Catalog Task after approval.

### Verified Output

- Request: `REQ0010001`
- Requested Item: `RITM0010001`
- Catalog Task: `SCTASK0010001`
- Assignment Group: `Hardware`
- Short Description: `Laptop need to Configured`
- Approval: `Approved`

## Result
The Standard Laptop procurement automation was successfully implemented and tested.

The Flow Designer automation reduced manual task creation by automatically generating a Catalog Task and assigning it to the Hardware team.

## Benefits
- Reduced manual effort.
- Faster task generation.
- Improved task allocation.
- Reduced delays in laptop configuration.
- Improved IT procurement efficiency.
- Consistent and automated workflow.

## Conclusion
The project successfully demonstrates the use of ServiceNow Flow Designer to automate the Standard Laptop procurement process.

By automatically creating and assigning Catalog Tasks after approval, the solution reduces manual intervention and improves the overall efficiency of IT procurement operations.

## Project Status
Successfully Completed.
