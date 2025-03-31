# Installing vib file
```
esxcli software component apply -d /tmp/CPxxxxxx_VMw.zip
```

# Executing the binary
```
cd /opt/Smart_Component/CPxxxxxx
./Execute_Component
```

# Removing vib file
```
esxcli software component remove –n Smart-Component-CPxxxxxx
```

# Manually remove the folders
```
rm –rf /opt/Smart_Component/CPxxxxxx
```
