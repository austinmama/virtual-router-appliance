---

copyright:
  years: 2017
lastupdated: "20189-11-14"

keywords: configure, service, NAT

subcollection: virtual-router-appliance

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank_"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:download: .download}
{:note: .note}
{:important: .important}
{:help: data-hd-content-type='help'}
{:support: data-reuse='support'}

# Configuring Services
{: #configuring-your-services}
{: help}
{: support}

There are a variety of services running on the {{site.data.keyword.vra_full}} (VRA) that can be configured.
{: shortdesc}

They include:

`vyatta@vrouter# set service`

Possible completions include:

```
 > connsync        Connection tracking synchronization (conn-sync) service
 > dhcp-relay      Dynamic Host Configuration Protocol (DHCP) relay agent
 > dhcp-server     Dynamic Host Configuration Protocol (DHCP) for DHCP server
 > dhcpv6-relay    DHCPv6 Relay Agent parameters
 > dhcpv6-server   DHCP for IPv6 (DHCPv6) server
 > dns             Domain Name Server (DNS) parameters
 > flow-monitoring Flow-Monitoring traffic monitoring configuration
 > https           Enable/disable the Web server
 > lldp            LLDP settings
 > nat             Network Address Translation (NAT)
 > netconf         NETCONF (RFC 6241)
 > portmonitor     Portmonitor configuration
 > sflow           sflow configuration for dataplane
 > snmp            Simple Network Management Protocol (SNMP)
 > ssh             Secure Shell (SSH) protocol
 > telnet          Enable/disable Network Virtual Terminal Protocol (TELNET) protocol
 > twamp           Two-Way Active Measurement Protocol
```

`nat` is configured as part of the service, and `https` controls access to the Web GUI and the APIs. `connsync` defines how two VRAs can share connection tracking synchronization for things like stateful firewall failover.
