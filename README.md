## Release Information

- Solution Pack Version: 1.0.0
- Minimum Compatible FortiSOAR™ Version: 7.2.0
- Authored By: Fortinet
- Certified: No

## Overview

### Introduction

*Impossible Traveller Threat Response Solution Pack* is designed to provide a set of investigation and utility playbooks to respond to Concurrent Successful Authentications To the Same Account From Multiple Countries. SIEM usually picks up and reports these events.

Configure SIEM ingestion using connectors such as Fortinet FortiSIEM. The ingestion process creates an alert of type 'Concurrent Login' and manually triggers the response workflow.

Refer to Simulation Scenario - **Concurrent Successful Authentications** to experience the use case without a SIEM configuration.

### Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/solution-pack-guide.md) to understand how to Simulate and Reset scenarios.

This Solution Pack ships with the following simulation scenarios. 

**Concurrent Successful Authentications**

The scenario generates a demo alert of Type **Concurrent Login**.

Navigate to generated alert and observe that the destination IP address is present to analyze the case.

**Investigate Concurrent Login from Different Geo Location:**

Launch the **Investigate Concurrent Login from Different Geo Location** playbook and observe various investigation activities such as

- Identify the geolocation from where concurrent login was observed
- Get the user's details, who is attempting concurrent login, from Microsoft's Active Directory
- Check login activity of the user for the last 4 hours
- Disable the user for an hour with the IT team's approval
- If the user attempts to log in again, reset the user's password

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

2. Global Variable(s)

    - Default_Email
    - Demo_mode

3. Record Set(s)

    - Scenario: Concurrent Successful Authentications

4. Playbook Collection(s)
    - 02 - Use Case - Impossible Traveller Threat Response(2):

    |**Playbook Name**|**Description**|
    | :- | :- |
    |Generate Alert for Concurrent Successful Authentication | Generates a demo record for the event - Concurrent Successful Authentications To Same Account From Multiple Countries|
    |Investigate Concurrent Login from Different Geo Location | Investigates alerts of type 'Concurrent Login' by checking if the source IP address is in the specified CIDR range and then performs remediation tasks based on the result.|

     **Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.

