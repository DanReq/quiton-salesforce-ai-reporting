# Quiton – Salesforce AI Sales Reporting Automation

Quiton is a Salesforce-based project focused on automating sales reports through Salesforce Flows, Apex Invocable Actions, Agentforce-oriented prompt design, and an external REST API built with FastAPI and Python.

## Status

This repository presents a sanitized case study version of the Quiton project.

The full implementation is currently private due to hackathon participation and security considerations. A public version with selected non-sensitive implementation details will be released after the hackathon concludes.

## Overview

The solution integrates Salesforce with an external REST API to generate automated sales reports, process business metrics, and support Agentforce-based interactions.

The project automates the generation of closed-sales reports by sending report parameters from Salesforce to an external FastAPI service, processing sales data in Python, and returning business indicators such as total closed sales, average ticket size, and top categories.

## Tech Stack

- Salesforce
- Agentforce
- Apex
- Salesforce Flows
- Named Credentials
- External Credentials
- FastAPI
- Python
- Pandas
- REST APIs
- Render

## Architecture

User request → Agentforce → Salesforce Flow → Apex Invocable Action → FastAPI REST API → Python data processing → Salesforce result object → Agentforce response

## Main Features

- Automated sales report requests from Salesforce
- Salesforce Flow automation
- Apex Invocable Action integration
- External REST API integration with FastAPI
- Python-based data cleaning and business metric calculation
- Salesforce custom objects for report storage
- Agentforce-oriented prompt design
- Integration testing and workflow debugging

## Salesforce Components

- Flow: `Quiton_Sales_Report_Flow`
- Apex Invocable Action: `QuitonClosedSalesAnalysisAction`
- Custom Objects:
  - `Quiton_Report_Request__c`
  - `Quiton_Report_Result__c`
  - `Quiton_Audit_Event__c`

## API Endpoints

- `GET /health`
- `POST /reports/closed-sales-month`

## Project Documentation

- [Architecture](docs/architecture.md)
- [API Contract](docs/api_contract.md)
- [Salesforce Flow Overview](docs/salesforce_flow.md)
- [Apex Overview](salesforce/apex_overview.md)
- [Custom Objects](salesforce/custom_objects.md)

## Security Notice

This repository does not include credentials, tokens, private Salesforce configuration, production data, or confidential hackathon materials.

All examples, screenshots, and documentation are sanitized for portfolio and recruitment purposes.