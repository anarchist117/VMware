# Modify the boot.cfg file

### 1.Add the following line
prefix=http://ipxe.domain.com/ESXi-8.x.x-XXXXXX
where http://ipxe.domain.com/ESXi-8.x.x-XXXXXX is the location of the installer files on the HTTP server.

### 2. Delete (/)
If the filenames in the kernel= and modules= lines begin with a forward slash (/) character, delete that character.

### 3. Delete cdromBoot
If the kernelopt= line contains the string cdromBoot, remove the string only.

# Documentation
[Boot the ESXi Installer by Using iPXE and HTTP](https://techdocs.broadcom.com/us/en/vmware-cis/vsphere/vsphere/8-0/esxi-upgrade-8-0/upgrading-esxi-hosts-upgrade/how-to-boot-an-esxi-host-from-a-network-device-upgrade/boot-the-esxi-installer-by-using-ipxe-and-http-upgrade.html)
