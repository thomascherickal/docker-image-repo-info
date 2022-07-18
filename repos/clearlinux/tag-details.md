<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:5391fd340a9ce73309cb5795ec8a8d3375c3ffc5947959f6df8d731d9f039a96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:0469e5f71aab6713dd86be7b32b66ffc20aade33e553d07cdf729abc1a60d9c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94793420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:155befc294e79b15e71bfcfc3541ce2a8b0750b9a2b2f16adf797c8af5b75a5b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 18 Jul 2022 18:27:19 GMT
ADD file:a340dd837722775c7d2358fca656c5874637fcb5e1a29c5e84985c66260d982a in / 
# Mon, 18 Jul 2022 18:27:20 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 18 Jul 2022 18:27:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d2b4f9a15ea82eea77089e6bbdbac0b10844a30a890c868f7671404e3fa550c0`  
		Last Modified: Mon, 18 Jul 2022 18:27:45 GMT  
		Size: 94.8 MB (94793202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470f8e25a170dfef2854bef020f046693351711ecd9f71de8cb1da68598e933f`  
		Last Modified: Mon, 18 Jul 2022 18:27:31 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:5391fd340a9ce73309cb5795ec8a8d3375c3ffc5947959f6df8d731d9f039a96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:0469e5f71aab6713dd86be7b32b66ffc20aade33e553d07cdf729abc1a60d9c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94793420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:155befc294e79b15e71bfcfc3541ce2a8b0750b9a2b2f16adf797c8af5b75a5b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 18 Jul 2022 18:27:19 GMT
ADD file:a340dd837722775c7d2358fca656c5874637fcb5e1a29c5e84985c66260d982a in / 
# Mon, 18 Jul 2022 18:27:20 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 18 Jul 2022 18:27:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d2b4f9a15ea82eea77089e6bbdbac0b10844a30a890c868f7671404e3fa550c0`  
		Last Modified: Mon, 18 Jul 2022 18:27:45 GMT  
		Size: 94.8 MB (94793202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470f8e25a170dfef2854bef020f046693351711ecd9f71de8cb1da68598e933f`  
		Last Modified: Mon, 18 Jul 2022 18:27:31 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
