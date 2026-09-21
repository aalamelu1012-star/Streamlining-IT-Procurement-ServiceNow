# Phase 3: Project Design

## Project Title
Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Design Overview
The project is designed to automate the Standard Laptop procurement process using ServiceNow Flow Designer.

The solution connects the Standard Laptop Service Catalog item with a Flow Designer flow. After the laptop request is approved, a Catalog Task is automatically created and assigned to the Hardware group.

## System Architecture

The project consists of the following major components:

1. ServiceNow Service Catalog
2. Standard Laptop Catalog Item
3. Request and Requested Item
4. Approval Process
5. ServiceNow Flow Designer
6. Catalog Task
7. Hardware Assignment Group

## Process Flow

User Requests Standard Laptop  
↓  
Service Catalog  
↓  
Request Created (REQ)  
↓  
Requested Item Created (RITM)  
↓  
Approval Requested  
↓  
Request Approved  
↓  
Flow Designer Triggered  
↓  
Create Catalog Task  
↓  
Task Assigned to Hardware Group  
↓  
Laptop Configuration

## Flow Designer Configuration

### Flow Details

| Configuration | Value |
|---|---|
| Flow Name | Standard laptop task |
| Application | Global |
| Run As | System User |
| Trigger | Service Catalog |

## Trigger Design

The flow uses the `Service Catalog` trigger.

The trigger provides the Requested Item Record that is used while creating the Catalog Task.

## Action Design

The flow contains the `Create Catalog Task` action.

### Catalog Task Configuration

| Field | Value |
|---|---|
| Table Name | Catalog Task [sc_task] |
| Requested Item | Trigger → Requested Item Record |
| Short Description | Laptop need to Configured |
| Description | Laptop need to Configured |
| Assignment Group | Hardware |
| Approval | Approved |
| Wait | Enabled |

## Process Engine Configuration

The `Standard laptop task` flow is assigned to the `Standard Laptop` Catalog Item through the Process Engine.

This connects the catalog item with the Flow Designer automation.

## Input

The main input to the system is a user request for a Standard Laptop through the ServiceNow Service Catalog.

## Processing

The system performs the following operations:

1. Accepts the Standard Laptop request.
2. Creates a Request and Requested Item.
3. Sends the request for approval.
4. Processes the approved request.
5. Executes the Flow Designer automation.
6. Creates a Catalog Task.
7. Assigns the Catalog Task to the Hardware group.

## Output

The expected output is an automatically generated Catalog Task associated with the Standard Laptop Requested Item.

The task contains:

- Short Description: `Laptop need to Configured`
- Description: `Laptop need to Configured`
- Assignment Group: `Hardware`
- Approval: `Approved`

## Design Benefits

- Reduces manual task creation.
- Automates task assignment.
- Improves procurement workflow efficiency.
- Reduces delays in laptop configuration.
- Provides a consistent process for Standard Laptop requests.

## Final Design

The final design provides an automated connection between the Service Catalog and the Hardware team using ServiceNow Flow Designer. Once the required approval is completed, the Catalog Task is generated automatically for laptop configuration.
