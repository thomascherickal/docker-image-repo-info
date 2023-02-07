## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:2072679bb4039f54b1b84f7b558f8357ddcdf3d569c5d5bc7207881f741d559e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:3b4021408fdbd6a9d935b9f72e13b077a99b33ea4176e439f47897e0fc142759
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.5 MB (86539971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44658c6d6856f16b6c38c9e1cbb60a6a33a85db705f455ae36b197295858a653`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Tue, 07 Feb 2023 02:29:34 GMT
ADD file:754f21827a968bc5a5d3709054effb79aab04cb579afbd0bbdedab6c9021e44f in / 
# Tue, 07 Feb 2023 02:29:35 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Tue, 07 Feb 2023 02:29:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:934990a0a78447f02c2fc86811d07f50abdd8d0f60daf5e4ebe3b414e5ff7949`  
		Last Modified: Tue, 07 Feb 2023 02:29:54 GMT  
		Size: 86.5 MB (86539753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afe1b5cbc707bc975d22c3ce396a97d534ae853b3d95de6730c44d2171730c7`  
		Last Modified: Tue, 07 Feb 2023 02:29:43 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
