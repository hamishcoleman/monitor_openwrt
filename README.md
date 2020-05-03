OpenWRT has a well specified jsonrpc interface, which can be used to collect
a number of interesting stats.  Many of these stats can be easily exported
via SNMP or other existing packages, however some cannot.

Initially, DSL stats are the target.


Example Usage:

    ./monitor_openwrt --username=root --password=hunter9 log $logfile

Flags:
<dl>
 <dt>--hostname -h</dt> <dd>The host to connect to, defaults to 192.168.1.1</dd>
 <dt>--username -u<dt>  <dd>Username to login as, defaults to 'root'</dd>
 <dt>--password -p<dt>  <dd>Password to use - required</dd>
 <dt>--debug<dt>        <dd>Various debug output (mostly just dumping the whole recieved data structure)</dd>
</dl>
