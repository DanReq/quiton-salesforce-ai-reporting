# Architecture

The Quiton project connects Salesforce with an external FastAPI service to automate sales reporting.

## High-Level Flow

1. A user requests a sales report through Agentforce or Salesforce.
2. Salesforce Flow captures the request parameters.
3. An Apex Invocable Action sends the request to an external REST API.
4. The FastAPI backend processes the data using Python and Pandas.
5. The API returns business metrics.
6. Salesforce stores the result in custom objects.
7. Agentforce uses the stored result to generate a business-oriented response.

## Architecture Diagram

User request → Agentforce → Salesforce Flow → Apex Invocable Action → FastAPI REST API → Python/Pandas processing → Salesforce custom object → Agentforce response