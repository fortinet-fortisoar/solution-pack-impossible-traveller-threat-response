[Home](../README.md) |
|--------------------------------------------|

# Contents

## Connectors

| Connector                  | Description                                                                                                                                                                            |
|:---------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Microsoft Active Directory | Helps directly query AD to retrieve information about users, groups, and computers, in an organization, by using the Lightweight Directory Access Protocol (LDAP)                      |
| Fortinet FortiSIEM         | FortiSIEM provides integrations that allow you to query and make changes to the CMDB, query events, and send incident notifications.                                                   |
| Fortinet FortiGate         | Fortinet FortiGate enterprise firewall provide high performance, consolidated advanced security and granular visibility for broad protection across the entire digital attack surface. |

>**Warning:** After deployment, this Solution Pack will install or upgrade the stated connectors list.

## Record Set

| Record Set | Description                           |
|:-----------|:--------------------------------------|
| Scenario   | Concurrent Successful Authentications |

## Playbook Collection

| 02 - Use Case - Impossible Traveler Threat Response |
|:-----------------------------------------------------|


| Playbook Name                                            | Description                                                                                                                                                                 |
|:---------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Generate Alert for Concurrent Successful Authentication  | Generates a demo record for the event - Concurrent Successful Authentications To Same Account From Multiple Countries                                                       |
| Investigate Concurrent Login from Different Geo Location | Investigates alerts of type 'Concurrent Login' by checking if the source IP address is in the specified CIDR range and then performs remediation tasks based on the result. |
| IP Address - Fortinet FortiGate - Block                  | Blocks indicators of type *IP Address* on the Fortinet FortiGate and marks the indicators as **Blocked** based on their block status.                                         |

>**Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.

# Next Steps

| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) | [Usage](./usage.md) |
|-----------------------------------------|-------------------------------------------|---------------------|
