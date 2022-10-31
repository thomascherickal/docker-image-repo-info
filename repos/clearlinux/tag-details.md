<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:c10be34af7921ef1a311933d1d46a128c5252c3bf99061b8f7d4679de61f2439
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:e3fb8dc97776a961e5ea3a51f001d07bdc9dd496a55eec96b426ea626ee7cb7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68872537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff65dc719c396a45759a5150f5c8d12a8cba64dff39409d8cc03bb56ea8f4f70`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 31 Oct 2022 19:24:59 GMT
ADD file:44b82ed4687a801c1db2114d6c588e3fcf989bb10dbf28fef58f6857829b7754 in / 
# Mon, 31 Oct 2022 19:25:00 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 31 Oct 2022 19:25:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1616c2c895f08ea4f6c86ec14b521d0c0c65add976f7eb824bbb162f89543c2a`  
		Last Modified: Mon, 31 Oct 2022 19:25:19 GMT  
		Size: 68.9 MB (68872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59fc41dc762756cd9f65033acf738392d4e67919db80c6cb55f5342146a719`  
		Last Modified: Mon, 31 Oct 2022 19:25:09 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:c10be34af7921ef1a311933d1d46a128c5252c3bf99061b8f7d4679de61f2439
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:e3fb8dc97776a961e5ea3a51f001d07bdc9dd496a55eec96b426ea626ee7cb7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68872537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff65dc719c396a45759a5150f5c8d12a8cba64dff39409d8cc03bb56ea8f4f70`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 31 Oct 2022 19:24:59 GMT
ADD file:44b82ed4687a801c1db2114d6c588e3fcf989bb10dbf28fef58f6857829b7754 in / 
# Mon, 31 Oct 2022 19:25:00 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 31 Oct 2022 19:25:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1616c2c895f08ea4f6c86ec14b521d0c0c65add976f7eb824bbb162f89543c2a`  
		Last Modified: Mon, 31 Oct 2022 19:25:19 GMT  
		Size: 68.9 MB (68872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59fc41dc762756cd9f65033acf738392d4e67919db80c6cb55f5342146a719`  
		Last Modified: Mon, 31 Oct 2022 19:25:09 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
