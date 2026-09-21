# Phase 2: Requirement Analysis

## Project Title
Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Requirement Overview
The project requires an automated process in ServiceNow for handling Standard Laptop orders. The solution should use Flow Designer to automatically generate a Catalog Task for the Hardware team after the laptop request is approved.

## Functional Requirements

### 1. Standard Laptop Request
- Users should be able to request a Standard Laptop through the Service Catalog.
- The request should create a Requested Item (RITM).

### 2. Approval Process
- The Standard Laptop request should go through an approval process.
- The automation should proceed after the request is approved.

### 3. Flow Designer Automation
- A flow named `Standard laptop task` should be created.
- The flow should use the `Service Catalog` trigger.
- The flow should run as `System User`.

### 4. Catalog Task Creation
After approval, the flow should automatically create a Catalog Task.

The task should contain:
- Short Description: `Laptop need to Configured`
- Description: `Laptop need to Configured`
- Assignment Group: `Hardware`
- Approval: `Approved`

## Non-Functional Requirements
- The automation should reduce manual intervention.
- The process should be reliable and consistent.
- The solution should reduce delays in laptop configuration.
- The workflow should be easy to maintain using ServiceNow Flow Designer.

## Software Requirements
- ServiceNow Instance
- ServiceNow Flow Designer
- Service Catalog
- Web Browser
- GitHub for project documentation

## User Roles
- Requester – Places the Standard Laptop order.
- Approver – Approves the laptop request.
- Hardware Team – Handles the generated laptop configuration task.
- Administrator – Configures and manages the ServiceNow flow.

## Expected Output
After the Standard Laptop request is approved, a Catalog Task should be automatically generated and assigned to the Hardware group for laptop configuration.
