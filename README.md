# spacewalk-rundeck-import

Script for importing a Spacewalk Systemgroup as a Rundeck project file in yaml format via Frontier::Client
This software in "works for me" status, tested on Fedora 23 and Centos 7 against Spacewalk 2.4
Use at your own risk!

Pulls the hostlist from Spacewalk API and saves in a file <systemgroup>.yaml for furter usage in Rundeck
Config file support (command line options beat config file)

Install:

# cp usr/bin/spacewalk-rundeck-import /usr/local/bin/.
# mkdir  /etc/spacewalk-rundeck-import
# cp etc/spacewalk-rundeck-import/config /etc/spacewalk-rundeck-import/.

Usage:
# spacewalk-rundeck-import [--spacewalk_server FQDN] [--spacewalk_user USER] [--systemgroup GROUP] [--resource_path PATH] [--spacewalk_password PASS]


Shortcomings:
Frontier::client via plain HTTP, no help, no manpage.

Todo v1.1:
lock file support for proper cron.hourly execution

License: GPLv2
