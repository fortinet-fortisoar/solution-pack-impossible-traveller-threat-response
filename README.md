# Impossible Traveller Threat Response Solution Pack

## Release Information

- Solution Pack Version: 1.0.0
- Minimum Compatible FortiSOAR™ Version: 7.2.0
- Authored By: Fortinet
- Certified: Yes

## Overview

### Introduction

*Impossible Traveller Threat Response Solution Pack* is designed to provide a set of investigation and utility playbooks to respond to Concurrent Successful Authentications To the Same Account From Multiple Countries. These events are typically picked up by SIEM.

Configure SIEM ingestion using connectors such as Fortinet FortiSIEM. The ingestion process creates an alert of type 'Concurrent Login' and manually triggers the response workflow.

Refer to Simulation Scenario - 'Concurrent Successful Authentications' to experience the use case without any SIEM configuration.

### Usage

This Solution Pack ships with the following simulation scenarios. [Refer](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/solution-pack-guide.md/?target=_blank) to Simulate Scenario documentation to understand how to Simulate and Reset Scenario.

#### 1. Scenario: Concurrent Successful Authentications

The scenario generates a demo alert of Type 'Concurrent Login'.

Goto generated an alert and observe the following:

- Destination IP Address is presented to analyze the case

**Investigate Concurrent Login from Different Geo Location:**

Launch the "Investigate Concurrent Login from Different Geo Location" playbook and observe various investigation activities such as

- Identify the Geolocation from where concurrent login observed
- Get user's details from Microsoft Active Directory that involved in concurrent login
- Check login activity for the user for the last 4 hours
- Disable the user for an hour with the IT team's approval
- If login is attempted then reset the user password

## Prerequisites

|**Solution Pack Name**|**Purpose**|**Doc Link**|
| :- | :- | :- |
|SOAR Framework 1.0.0|Require for Incident Response modules|[Click here](https://github.com/fortinet-fortisoar/solution-pack-soar-framework/blob/develop/README.md)|
|SOC Simulator 1.0.1|Require for Scenario Module and SOC Simulator connector| [Click here](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/README.md)|

## Contents

1. Connector(s)

    |**Sr. No**|**Connector**|
    | :- | :- |
    |1|Microsoft Active Directory|
    |2|Fortinet FortiSIEM|

     **Warning:** After deployment, this Solution Pack will install or upgrade the stated connectors list.

2. Record Set(s)

    - Scenario: Concurrent Successful Authentications

3. Global Variable(s)

    - Default_Email
    - Demo_mode

4. Playbook Collection(s)
    - 02 - Use Case - Impossible Traveller Threat Response(2):

|**Playbook Name**|**Description**|
| :- | :- |
|Generate Alert for Concurrent Successful Authentication | Generates a demo record for the event - Concurrent Successful Authentications To Same Account From Multiple Countries|
|Investigate Concurrent Login from Different Geo Location | Investigates alerts of type 'Concurrent Login' by checking if the source IP address is in the specified CIDR range, and then performs remediation tasks based on the result.|
