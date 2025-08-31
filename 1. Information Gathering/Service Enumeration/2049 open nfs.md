# 2049/tcp nfs = network file system
```
mount -t nfs 172.30.217.107:/srv/nfs /mnt/dev
```

## view shares
- to view the shares

```
showmount -e $target
```

## one liner
```
sudo mkdir NFS && sudo mount -t nfs $target:/<sharename> ./NFS
```
