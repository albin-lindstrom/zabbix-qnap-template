# Zabbix: QNAP Template (SNMPv2)

This template allows you to quickly get up and running with monitoring of QNAP line of devices (NAS). It allows for auto-discovering of hard drives, LUNs, pools, volumes, system HW and automatically applies appropriate triggers for the discovered items.

## ⚙️ Installation

1. Import *zbx_snmp_qnap.xml* to Zabbix (Configuration -> Templates -> Import)
2. Add the template *Template SNMP QNAP* to your host and configure 
   1. Add *{$SNMP_COMMUNITY}* to your host's macros and configure it. (default is usually public)
3. Enable the *SNMP* agent on your QNAP device.
   1. Set *SNMP community* to the same value as your macro or the other way around.

## 🏷️ Features
- ✔️ Auto discovering of  hard drives, LUNs, pools and volumes
- ✔️  Triggers for discovered items
- ✔️ Monitoring  state of RAID(s)
- 🔶 Linked with **Template Module Generic SNMPv2**

## Supported models
Updated as of 2020-08-17.
- TS-432XU-RP

## Issues
- none so far?
## License
[MIT](https://choosealicense.com/licenses/mit/)