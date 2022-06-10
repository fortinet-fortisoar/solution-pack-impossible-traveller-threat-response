| [Home](https://github.com/fortinet-fortisoar/solution-pack-impossible-traveller-threat-response/blob/develop/README.md) |
|--------------------------------------------|

# Contents

## Connectors

|Connector|Description|
| :- | :- |
|Microsoft Active Directory| Helps directly query AD to retrieve information about users, groups, and computers, in an organization, by using the Lightweight Directory Access Protocol (LDAP)|
|Fortinet FortiSIEM| FortiSIEM provides integrations that allow you to query and make changes to the CMDB, query events, and send incident notifications.|

>**Warning:** After deployment, this Solution Pack will install or upgrade the stated connectors list.

## Global Variables

|Global Variable|Description|
| :- | :- |
|`Default_Email`| This global variable contains the email address which sends acknowledgement and other emails to the reporter. |
|`Demo_mode`| Enables playbook to execute a mock output |

## Record Set

|Record Set|Description|
| :- | :- |
|Scenario| Concurrent Successful Authentications|

## Playbook Collection
|02 - Use Case - Impossible Traveller Threat Response|
|:-                                                  |

|Playbook Name|Description|
| :- | :- |
|Generate Alert for Concurrent Successful Authentication | Generates a demo record for the event - Concurrent Successful Authentications To Same Account From Multiple Countries|
|Investigate Concurrent Login from Different Geo Location | Investigates alerts of type 'Concurrent Login' by checking if the source IP address is in the specified CIDR range and then performs remediation tasks based on the result.|

>**Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.

