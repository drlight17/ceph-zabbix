# ceph-zabbix

A zabbix probe to get performance counters of ceph (Luminous 12.2+)


Installation
============

Install jq:
      sudo apt install jq zabbix-sender

Copy the scripts, zabbix_agentd.conf.d into /etc/zabbix/

Check arguments: Server, Hostname, ListenIP and UnsafeUserParameters=1 in zabbix_agentd.conf

Check permission for read user zabbix /etc/ceph/<{$CLUSTER_NAME}>.client.admin.keyring

Finally in zabbix setup the discovery rule and related items you need.# ceph-zabbix
