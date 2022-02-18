# Zabbix: QNAP Template (SNMPv2)

This template allows you to quickly get up and running with monitoring of QNAP line of devices (NAS). It allows for auto-discovering of hard drives, LUNs, pools, volumes, system HW and automatically applies appropriate triggers for the discovered items.

# 📃 Different QNAP firmwares and templates - read this very carefully!

QNAP has released new firmwares which means new SNMP OIDs and in turn this mean some devices may be incompatible with the new Zabbix templates unless their firmwares
are updated to **QTS 4.5.2 or higher**. For now, the older templates are NOT compatible with the new QTS 4.5.2 or higher SNMP OIDs!

## ⚙️ Installation (**Zabbix 5.x or higher**)

1. Download the appropriate template from [Releases](https://github.com/albinbatman/zabbix-qnap-template/releases/new) for your Zabbix version.
2. Import the template file to Zabbix (Configuration -> Templates -> Import)
3. Add the template *Template SNMP QNAP* to your host and configure 
   1. Adjust *{$SNMP_COMMUNITY}* in host's macros and configure it. (Under Macros -> Inherited and template macros if different from default *public* community)
4. Enable the *SNMP* agent on your QNAP device.
   1. Set *SNMP community* to the same value as your macro or the other way around.

## ⚙️ Installation (**Zabbix 5.x or lower**)

1. Download the appropriate template from [Releases](https://github.com/albinbatman/zabbix-qnap-template/releases/new) for your Zabbix version.
2. Import the template file to Zabbix (Configuration -> Templates -> Import)
   1. Add *{$SNMP_COMMUNITY}* to your host's macros and configure it. (default is usually public)
3. Enable the *SNMP* agent on your QNAP device.
   1. Set *SNMP community* to the same value as your macro or the other way around.

## 🏷️ Features
- ✔️ Auto discovering of hard drives, LUNs, pools, volumes and network interfaces
- ✔️  Triggers for discovered items
- ✔️ Monitoring  state of RAID(s)

## Supported models
Updated as of 2022-02-18.
- TS-432XU-RP
- TS-X32U
- TS-X63U
- TS-H886

## License
[MIT](https://choosealicense.com/licenses/mit/)