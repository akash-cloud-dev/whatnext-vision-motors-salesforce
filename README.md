# WhatNext Vision Motors – Salesforce CRM

## Project Overview
WhatNext Vision Motors is a Salesforce CRM project designed to manage vehicle sales, dealers, customers, vehicle orders, test drives, and service requests.
The project demonstrates Salesforce data modeling, Lightning App development, automation using Flow, Apex Triggers, Batch Apex, and Scheduled Apex.

## Objectives
- Manage vehicle information and inventory
- Manage authorized vehicle dealers
- Manage customer information
- Track vehicle orders
- Manage test drive bookings
- Track vehicle service requests
- Validate vehicle stock before processing orders
- Automatically update vehicle stock after confirmed orders
- Process pending orders when stock becomes available
- Automate scheduled processing using Batch Apex and Scheduled Apex

## Salesforce Custom Objects
- Vehicle
- Vehicle Dealer
- Vehicle Customer
- Vehicle Order
- Vehicle Test Drive
- Vehicle Service Request

## Relationships
- Vehicle → Vehicle Dealer
- Vehicle Order → Vehicle
- Vehicle Order → Vehicle Customer
- Vehicle Test Drive → Vehicle
- Vehicle Test Drive → Vehicle Customer
- Vehicle Service Request → Vehicle
- Vehicle Service Request → Vehicle Customer

## Automation
The project uses Salesforce Flow to automate business processes, including scheduled test-drive related activities and notifications.

## Apex Implementation
### VehicleOrderTriggerHandler
The trigger handler contains the vehicle stock validation and order-processing logic.

### VehicleOrderTrigger
The trigger invokes the handler during relevant Vehicle Order insert and update operations.

### VehicleOrderBatch
The Batch Apex class processes pending vehicle orders when vehicle stock becomes available.

### VehicleOrderBatchScheduler
The scheduler executes the vehicle order batch automatically according to the configured schedule.

## Technologies Used
- Salesforce CRM
- Lightning App
- Custom Objects
- Custom Fields
- Lookup Relationships
- Salesforce Flow
- Apex
- Apex Trigger
- Trigger Handler
- Batch Apex
- Scheduled Apex

## Project Demo
Demo video: [Add YouTube Demo Link Here]

## Project Repository
This repository contains documentation and Salesforce project implementation files for WhatNext Vision Motors.

## Author
Vankudoth Akash
