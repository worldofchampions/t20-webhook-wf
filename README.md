# t20-webhook-wf

T20 Cricket League Webhook Azure Logic App (Standard) Workflows

## Configuration

The following application settings have to be set to run the function app

| Setting Name                 				      |     Setting Type    | Description                                     |
|-------------------------------------------|:-------------------:|-------------------------------------------------|
| CosmosDBConnectionString                  |  Connection String  | Cosmos Database connection                      |

These settings should be set inside `local.settings.json` file when running locally.

{
  "IsEncrypted": false,
  "Values": {
    "AzureWebJobsStorage": "UseDevelopmentStorage=true",
    "FUNCTIONS_WORKER_RUNTIME": "node",
    "WORKFLOWS_TENANT_ID": "",
    "WORKFLOWS_SUBSCRIPTION_ID": "",
    "WORKFLOWS_RESOURCE_GROUP_NAME": "t20-rg-webhook-dev",
    "WORKFLOWS_LOCATION_NAME": "northeurope",
    "WORKFLOWS_MANAGEMENT_BASE_URI": "https://management.azure.com/",
    "azureLogicWorkflow_workflowSig": ""
    }
}

There setting can also be download via vs code command palette, press F1 and paste:
Azure Functions: Download Remote Settings....
