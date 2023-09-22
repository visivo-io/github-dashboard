# Visivo Github Dashboard

# Usage

This dashboard uses a Fivetran Webhook to Snowflake pipeline.  Fivetran has a great way to consume webhooks and store them in a database.

## Prequesites

1. Snowflake database
2. Fivetran account
3. Github repository

## Setup

### Fivetran

1. Create connector
2. Choose Webhook
3. Add schema and table names
4. Select `unpacked`  
5. Click `Save and test`
6. Copy the webhook URL

### Github

1. Click `Settings` > `Webhooks`
1. Set the url from the connector above
2. Create a new webhook and choose "everything"

### Back in Fivetran

1. Trigger the webhook connector to start its initial sync.

## Installation

1. Include the repo in your project's `includes`
2. Set the needed environment variables:
   1. DB
   2. DB_USERNAME