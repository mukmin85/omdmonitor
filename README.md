# Docker OMD Monitor
Automated build of OMD (Open Monitoring Distribution) for CentOS v6.7

# Description

Operating System : CentOS6.7

Environment : Production

Automated Build : Dockerfile

Process Management Tool : Supervisor

OMD repository : https://labs.consol.de/repo/stable/

# 2 Way Access OMD Web Interfaces

**Mode : Detached Mode with bind a service TCP Port**

Command Run: docker run -d -p 80:80 mukmin85/omdmonitor

Web Interfaces : http://localhost/monitor

Web Interfaces : http://xxx.xxx.xxx.xxx/monitor (Actual IP Address Host)


**Mode : Foreground Mode**

Command Run: docker run -i -t mukmin85/omdmonitor bash

Command Run in Bash : service httpd start; service omd start

Web Interfaces : http://xxx.xxx.xxx.xxx/monitor (IP Address DHCP Docker Container)
