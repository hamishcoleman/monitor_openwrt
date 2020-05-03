OpenWRT has a well specified jsonrpc interface, which can be used to collect
a number of interesting stats.  Many of these stats can be easily exported
via SNMP or other existing packages, however some cannot.

Initially, DSL stats are the target.


Example Usage:

    ./monitor_openwrt --username=root --password=hunter9 log $logfile

Flags:
    --hostname -h   Set the host to connect to, defaults to 192.168.1.1
    --username -u   Username to login as, defaults to 'root'
    --password -p   Password to use
    --debug         Various debug output (mostly just dumping the whole
                    recieved data structure)
