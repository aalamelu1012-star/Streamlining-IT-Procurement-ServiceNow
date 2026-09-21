# Phase 5: Project Development

## Project Title
Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Development Overview
The project was developed using ServiceNow Flow Designer to automate the Standard Laptop procurement process.

The implementation automatically creates a Catalog Task and assigns it to the Hardware group after the Standard Laptop request is approved.

## Step 1: Create Flow

A new flow was created in ServiceNow Flow Designer.

### Flow Configuration

| Field | Value |
|---|---|
| Flow Name | Standard laptop task |
| Application | Global |
| Run As | System User |

## Step 2: Configure Trigger

The trigger was configured as:

`Service Catalog`

This trigger allows the flow to work with the Requested Item Record generated from the Service Catalog.

## Step 3: Add Create Catalog Task Action

The `Create Catalog Task` action was added to the flow.

### Action Configuration

| Field | Value |
|---|---|
| Table Name | Catalog Task [sc_task] |
| Requested Item | Trigger → Requested Item Record |
| Short Description | Laptop need to Configured |
| Description | Laptop need to Configured |
| Assignment Group | Hardware |
| Approval | Approved |
| Wait | Enabled |

## Step 4: Activate Flow

After completing the trigger and action configuration, the flow was saved and activated.

Flow Name:

`Standard laptop task`

## Step 5: Assign Flow to Standard Laptop

The Standard Laptop Catalog Item was opened.

Navigation:

`Maintain Items → Standard Laptop → Process Engine`

The existing Flow configuration was replaced with:

`Standard laptop task`

The catalog item was then updated.

## Step 6: Place Standard Laptop Order

The Standard Laptop item was opened through the Service Catalog and an order was placed.

This generated:

- Request (REQ)
- Requested Item (RITM)
- Approval Record

## Step 7: Approve Request

The generated request was opened and the pending approval was approved.

After approval, the Requested Item moved to the approved stage.

## Step 8: Automatic Catalog Task Creation

After approval, the Flow Designer automation automatically generated a Catalog Task.

The generated task contained:

- Short Description: `Laptop need to Configured`
- Description: `Laptop need to Configured`
- Assignment Group: `Hardware`
- Approval: `Approved`

## Development Result

The implementation successfully automated the Standard Laptop procurement workflow.

The completed process is:

Standard Laptop Request  
→ Approval  
→ Request Approved  
→ Flow Designer Execution  
→ Catalog Task Created  
→ Hardware Group Assigned  
→ Laptop Configuration

## Development Status

Development Completed Successfully.
