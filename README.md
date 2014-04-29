ddclient-SMCD3GNV
=================

Script to get WAN ip address from Comcast SMCD3GNV router for use with ddclient.

My router software version:  eMTA & DOCSIS Software Version: 3.1.5.3.3_NCS 

Clone repository and copy script to `/etc/ddclient/get_wan_ip` (or wherever.)

Edit script and config as necessary (password and router ip address.)

Test script - no need to run as root and you should see your WAN ip address.

ddclient example setup using freedns.afraid.org:
```
use=cmd, cmd=/etc/ddclient/get_wan_ip
protocol=freedns
server=freedns.afraid.org
login=<your_login>
password=<your_password>
<your_ddns_hostname>
```
