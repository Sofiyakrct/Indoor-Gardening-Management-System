# Indoor Gardening Management System (IGMS)

## Project Overview

The Indoor Gardening Management System (IGMS) is a custom ServiceNow application designed to manage indoor gardening requests and support requesters, technicians, and managers.

The application was developed using ServiceNow's scoped application development and low-code capabilities.

## Application Details

| Property | Details |
|---|---|
| Application Name | Indoor Gardening Management System |
| Application Type | Custom |
| Platform | ServiceNow |
| Application Scope | `x_1989080_indoor_0` |
| Created | August 19, 2026 |

## Main Components

### 1. Indoor Gardening Requests

A custom table named **Indoor Gardening Requests** was created for managing indoor gardening service requests.

The table extends the **Task** table.

### 2. Request Fields

The table contains fields including:

- Number
- Priority
- Assigned To
- State
- Configuration Item
- Requested For
- Customer
- Requested Date
- Plant Type
- Indoor Plant Category
- Service Type
- Active
- Short Description
- Description
- Work Notes

### 3. Application Roles

Five application roles were created:

- `x_1989080_indoor_0.admin`
- `x_1989080_indoor_0.user`
- `x_1989080_indoor_0.x_1834345_igsm_manager_role`
- `x_1989080_indoor_0.x_1834346_igsm_technician_role`
- `x_1989080_indoor_0.x_1834347_igsm_requester_role`

### 4. Garden Record Producer

A **Garden Record Producer** was created and mapped to the **Indoor Gardening Requests** table.

Variables were created and mapped to the relevant fields.

### 5. Flow Designer

A flow named **Indoor Gardening Request Management** was created.

**Trigger:**

`Indoor Gardening Requests Created or Updated`

**Actions:**

1. Create or Update Record
2. Ask For Approval on Indoor Gardening Requests

The flow was tested successfully using the ServiceNow test functionality.

### 6. Approval Relationship

A relationship was created to attach the Approval table to the Indoor Gardening Requests form.

## Technologies and Platform

- ServiceNow
- ServiceNow Studio
- Table Builder
- Flow Designer
- Record Producer
- Scoped Application Development

## Project Purpose

The purpose of IGMS is to provide a structured ServiceNow application for managing indoor gardening service requests and supporting the users involved in the request management process.

## Project Status

The core application, custom request table, application roles, Garden Record Producer, request management flow, and approval relationship have been implemented and tested.

## Screenshots

Screenshots demonstrating the implemented ServiceNow components will be added to this repository.

## Application Scope

```text
x_1989080_indoor_0
