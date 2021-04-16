list all block devices

```
lsblk
```   
zero the block device

```
sudo dd if=/dev/zero of=/dev/sdX status=progress bs=32M && sync
```
