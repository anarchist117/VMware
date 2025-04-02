# 1. Disable firewall
```
esxcli network firewall set --enabled false
```

# 2. Change the enforcement level
```
localcli system secpolicy domain list | grep appDom
localcli system secpolicy domain set -n appDom -l disabled
```

# 3. Run iperf
```
cd /usr/lib/vmware/vsan/bin
./iperf3 -s -B 10.11.12.13
./iperf3 -c 10.11.12.13
```

# Default
```
esxcli network firewall set --enabled true
```
```
localcli system secpolicy domain set -n appDom -l enforcing
```

# Documentation
[iperf3 error - unable to start listener for connections: Operation not permitted](https://www.dell.com/support/kbdoc/en-us/000212752/vxrail-iperf3-error-unable-to-start-listener-for-connections-operation-not-permitted)
