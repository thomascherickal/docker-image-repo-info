## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:58ba41cd2ca0529523c249e9f5ef69d8faeef0fd0f71c592d304894cc0531bbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:4be85997a519cebf79fa9d03d35e7e08dc992d9dfc1fe200ff83b319d0708da6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87119409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25e9fc246aabe1bccbccd2946e034f0d43a901666875fcbaf17c26520c5ecb90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 14 Feb 2022 19:23:21 GMT
ADD file:5dada7bfaf9b9bf97ae9586a4658f3fe39b7cb2be2d8c5c98e4e93bc2242d788 in / 
# Mon, 14 Feb 2022 19:23:22 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 14 Feb 2022 19:23:23 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c2c21c0dad4d522476b62a0c3a97e47325ec0abc82fe68b4b4e74cf5b9143f54`  
		Last Modified: Mon, 14 Feb 2022 19:23:43 GMT  
		Size: 87.1 MB (87119192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634b5c0d15ba54e6c4026530343d59324304150ea74a0557df963e9ebd82050b`  
		Last Modified: Mon, 14 Feb 2022 19:23:32 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
