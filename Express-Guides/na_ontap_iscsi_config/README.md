# na_ontap_iscsi_config

## Steps 

* Install Iscsi utilities
```shell
yum install iscsi-initiator-utils
```
* Discover the target
```shell
iscsiadm -m discovery -t st -p xxx.xxx.xxx.xxx (iscsi LIF IP)
```
* Login to the target
```shell
iscsiadm -m node
```
```shell
iscsiadm -m node --login xxx.xxx.xxx.xxx (iscsi LIF IP)
```
* Partition, format and mount the iSCSI target by fdisk, mkfs.ext3, and mount command.
```shell
fdisk -l
```
```shell
fdisk /dev/sdb
```
* Make the filesystem
```shell
mkfs.ext3 /dev/sdb1
```
* Mount the iSCSI target
```shell
mount /dev/sdb1 /mnt
```
* Verify by checking permissions 
```shell
ls -l
```
* Unmount
```shell
umount /dev/sdb1 /mnt
```
