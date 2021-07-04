# kubernetes-the-not-so-hard-way

Disable SWAP
```
# /sbin/swapoff -a
# vim /etc/fstab
```

Add a # in front of the swap entry to disable it at the next boot
```
...
UUID=b90e4cce-635d-4975-9c2e-xyzxyzxyzxyzxyz /               ext4    errors=remount-ro 0       1
...
# UUID=43a18e27-5142-4674-9bbd-xyzxyzxyzxyzxyz none            swap    sw              0       0
...

```

