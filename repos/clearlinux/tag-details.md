<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:9c53cfff6143af6b719142122e034deacb61164d7324e8e96f49364d566b4291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:88652d2682bd63208e55f069c0ca4d3c30fe3acf2c5b730d16f8099a6d437162
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72608691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76910055bf303c53cc6204cb91696670b33fad2a323caef165de8d9895029aa1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 26 Jun 2023 21:19:42 GMT
ADD file:864641dfe7a29604e98a4cf0f19c1856a9dc7448a6417bfb2dac8fd057218fc7 in / 
# Mon, 26 Jun 2023 21:19:43 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 26 Jun 2023 21:19:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ff944905da5739d4d03dbb99b22d4ca8924ea3ba190e1489c92b232041374f1e`  
		Last Modified: Mon, 26 Jun 2023 21:20:00 GMT  
		Size: 72.6 MB (72608474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f881cd8540f048a4faff30437a9e3ad6f080f022b325356d38554f92ddbe401`  
		Last Modified: Mon, 26 Jun 2023 21:19:51 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:9c53cfff6143af6b719142122e034deacb61164d7324e8e96f49364d566b4291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:88652d2682bd63208e55f069c0ca4d3c30fe3acf2c5b730d16f8099a6d437162
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72608691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76910055bf303c53cc6204cb91696670b33fad2a323caef165de8d9895029aa1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 26 Jun 2023 21:19:42 GMT
ADD file:864641dfe7a29604e98a4cf0f19c1856a9dc7448a6417bfb2dac8fd057218fc7 in / 
# Mon, 26 Jun 2023 21:19:43 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 26 Jun 2023 21:19:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ff944905da5739d4d03dbb99b22d4ca8924ea3ba190e1489c92b232041374f1e`  
		Last Modified: Mon, 26 Jun 2023 21:20:00 GMT  
		Size: 72.6 MB (72608474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f881cd8540f048a4faff30437a9e3ad6f080f022b325356d38554f92ddbe401`  
		Last Modified: Mon, 26 Jun 2023 21:19:51 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
