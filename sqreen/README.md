# Sqreen Integration

## Overview

The Sqreen integration enables you and your team to monitor your service security activity right from Datadog.

It provides you with dashboards, security rules, log facets and saved views.

In order to use it you must be a Sqreen Design Partner, and have the Sqreen microagent deployed into your web applications.

TODO: Add a screenshot of the final Dashboard.

### Security Rules

This integration contains 2 security rules: 
* Security Incident detected by Sqreen
* User logged in from a new country

Once setup, you'll be able to review their full definition from the [Security Rules list](https://app.datadoghq.com/security/configuration/rules?sort=rule&query=source%3Asqreen).

## Setup

### Configure the Sqreen -> Datadog data pipeline

Sqreen streams your services security activity to Datadog as logs.

Here's the steps to follow to set it up:

1. Go to the [Sqreen Dashboard > Organization settings > Integrations](https://my.sqreen.com/profile/organization/integrations),
2. Add a new "Push API" integration and select "datadog" as the destination,
3. In the "url" field, input the Datadog ingestion server URL. For Datadog US: http-intake.logs.datadoghq.com. For Datadog EU: http-intake.logs.datadoghq.eu,
4. In the "dd_api_key", provide the Datadog API key to use to stream the Sqreen data as logs. [Datadog API keys management page](https://app.datadoghq.com/account/settings#api).

After a few seconds, the first logs with `source:sqreen` should be flowing in. 

The assets bundled in this integration will be deployed into your Datadog account.

### Troubleshooting

In case you face any issues using this integration, please reach out to [support@sqreen.com](mailto:support@sqreen.com).