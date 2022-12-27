## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:0c64a564145ce4be1eb5c25eb6f9d5395e048581dc7ac2a6183c38a8b309672b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:5bfb3610f3c43c4c1aff913f80a2ce47eacb67793d55e14024dc8cae8d828c48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67852381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982d886e13a959d0790c53130352ea39d922997226922dd2c6747e125fa78d8f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Tue, 27 Dec 2022 17:25:48 GMT
ADD file:089757cbec5f475efd3f32c2c6f7f0c6511a517b7edd69af420ac499601855d8 in / 
# Tue, 27 Dec 2022 17:25:49 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Tue, 27 Dec 2022 17:25:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9474401fe96b6cecc5a9ea2b7fc87b8359ce2b4596fbb57338d4765c7e701a2a`  
		Last Modified: Tue, 27 Dec 2022 17:26:09 GMT  
		Size: 67.9 MB (67852163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cd40ba29e470cb2fbd8c746e49ff4c7f35bd8bb0fb1522027950719c49bdad`  
		Last Modified: Tue, 27 Dec 2022 17:25:58 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
