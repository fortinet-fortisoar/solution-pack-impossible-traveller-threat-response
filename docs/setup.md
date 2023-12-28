[Home](../README.md) |
|--------------------------------------------|

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.
2. From the list of solution pack that appears, search for **Impossible Traveler Threat Response**.
3. Click the **Impossible Traveler Threat Response** solution pack card.
4. Click **Install** on the lower part of the screen to begin installation.

## Prerequisites

| Solution Pack Name | Version | Purpose                                                  |
|:-------------------|:--------|:---------------------------------------------------------|
| SOAR Framework     | v2.2.1  | Required for Incident Response modules                   |
| SOC Simulator      | v1.0.1  | Required for Scenario Module and SOC Simulator connector |

# Configuration

For optimal performance of **Impossible Traveler Threat Response** solution pack, you can install and configure the following connectors:

- **Fortinet FortiSIEM** - FortiSIEM provides integrations that allow you to query and make changes to the CMDB, query events, and send incident notifications.
    - To configure and use the Fortinet FortiSIEM connector as a source of data ingestion, refer to [Configuring Fortinet FortiSIEM](https://docs.fortinet.com/document/fortisoar/4.3.2/fortinet-fortisiem/278/fortinet-fortisiem-v4-3-2)
- **Microsoft Active Directory** - Helps directly query AD to retrieve information about users, groups, and computers, in an organization, by using the Lightweight Directory Access Protocol (LDAP)
    - To configure and use Microsoft's Active Directory connector, refer to [Configuring Microsoft's Active Directory](https://docs.fortinet.com/document/fortisoar/2.2.0/active-directory/154/active-directory-v2-2-0#Configuration_parameters)
- **Fortinet FortiGate** - FortiGate is an enterprise firewall provide high performance, consolidated advanced security and granular visibility for broad protection across the entire digital attack surface.
    - To configure and use the Fortinet FortiGate connector, refer to [Configuring Fortinet FortiGate](https://docs.fortinet.com/fortisoar/connectors/fortigate_firewall)

# Next Steps

| [Usage](./usage.md) | [Contents](./contents.md) |
|---------------------|---------------------------|
