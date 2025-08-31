# 2049/tcp nfs = network file system


mount -t nfs 172.30.217.107:/srv/nfs /mnt/dev

## view shares
showmount -e (IP address)
	to view the shares

## one liner 
sudo mkdir NFS && sudo mount -t nfs $target:/<sharename> ./NFS