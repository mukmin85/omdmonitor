# omdmonitor
Automated build of OMD (Open Monitoring Distribution) for CentOS v6.7

Docker OMD Monitor

Operating System : CentOS6.7
Environment : Production
Automated Build : Dockerfile
Process Management Tool : Supervisor
OMD repository : https://labs.consol.de/repo/stable/

2 Way Access OMD Web Interfaces

Mode : Detached Mode with bind a service TCP Port
Command Run: docker run -d -p 80:80 mukmin85/omdmonitor
Web Interfaces : http://localhost/monitor
Web Interfaces : http://<actual_ip_address_host>/monitor

Mode : Foreground Mode
Command Run: docker run -i -t mukmin85/omdmonitor bash
Command Run in Bash : service httpd start; service omd start
Web Interfaces : http://<ip_address_dhcp_docker_container>/monitor
