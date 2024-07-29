# Overview

[Calibre](https://calibre-ebook.com/) is a powerful and easy to use e-book manager.

# Storage
## Persistent Volume Claims
| name    | Claim   | Storage Class   | Storage |
|---------|---------|-----------------|---------|
| config  | calibre | ceph-filesystem | 15Gi    |

## NFS
`books` is still pointing to my filesystem on the vhost3 docker host

| name    | Type    | Server       | Path                                       |
|---------|---------|--------------|--------------------------------------------|
| books   | NFS     | 192.168.0.53 | /mnt/data/containers/rdp-calibre/config    |
