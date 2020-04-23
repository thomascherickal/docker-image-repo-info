## `debian:experimental`

```console
$ docker pull debian@sha256:652e98edbf4cd28b2f0860be75a3562ffb2c8849bcd878612d14b7ec2035c1d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:22585778342597709836b5e03fca3e64cdc602d0204b8d6dfbcf15d2145e8dd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (51979935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:598a0c29c569fde1a99fe781d590d72db5706b51d8f510431849666ef988c9be`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:42 GMT
ADD file:6ee109aa41831586899e9a04462a7c3a57fe9b599a263fb0ed2fc3ba1ed57b9b in / 
# Thu, 23 Apr 2020 00:23:43 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:23:58 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1411ff81de269e0758691342315f4c16f9a93db2b77b392e2e3fc3f3ba93b2f1`  
		Last Modified: Thu, 23 Apr 2020 00:28:27 GMT  
		Size: 52.0 MB (51979713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f31581696a65b3d4173140a5bb8db1d74ed3c22a7c834e1eb8b8f4d19dc60ab`  
		Last Modified: Thu, 23 Apr 2020 00:28:40 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:95be7053b64bddee6868073e7c21f38df20ff9b1278400e6b33056b9968363f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49930988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94fde9b3870a6707d39b60df13babccdce7897521e044bd60cb82503d35db8b1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:55:59 GMT
ADD file:1054b396b0c12ca5eafcf793f7dd85625f6ae0eb1ca9e1570abb8739f0d14db1 in / 
# Thu, 16 Apr 2020 00:56:01 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:56:28 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:84299eb4029fefaf91d9694e65fcf03975cfbfa5665cad38cc2dfd0141bbbcfe`  
		Last Modified: Thu, 16 Apr 2020 01:03:35 GMT  
		Size: 49.9 MB (49930766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78c826742a0ac73549c3f6c4e48820f740ccd1adc5b790343656e000dbeab67`  
		Last Modified: Thu, 16 Apr 2020 01:03:55 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:605f7674b64a00e8cf05eb6b666dec37a74f6bb414e1f81ebf2bf9e071345844
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47655577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78d8e570b6cb1eb6f40af1fbafb1815aa46b11f6923f990d2649ab7242cdc6a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:06:33 GMT
ADD file:a90852ff16b33798be6a6f90806198b01fd7b34d4f49542d74eceb892a0e85d9 in / 
# Thu, 16 Apr 2020 01:06:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:07:05 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ac815513fa4fe30a3f7f3a3fd76e1d2e7ea628d31f5a592e8e2a7a7e1e314675`  
		Last Modified: Thu, 16 Apr 2020 01:13:30 GMT  
		Size: 47.7 MB (47655353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d851faf879470227ed2916ff19cbb5af9ea3d0638bcaaeb7a4224ac2022dc5`  
		Last Modified: Thu, 16 Apr 2020 01:13:48 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c4055918046c4cee6749617322fbd124bc477c05d93c9bc773860d3a347f1ac7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50910266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:270a83961b936749fd14047aee15a5c739a6884a5b1f33f00e7b5e50fff8d737`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:46:36 GMT
ADD file:e154c2710b139a3977dbce9fb9f6d3be632f5459c071214e299ed0ee657db70c in / 
# Thu, 16 Apr 2020 02:46:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:47:10 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2e7a424af27736d7d8b86a9fc3ee21c7c58692a57e4a8454123077135bd6ecfd`  
		Last Modified: Thu, 16 Apr 2020 02:52:32 GMT  
		Size: 50.9 MB (50910043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9b8943c0a67b8724154dcb25565432cdcfbd725c0915ed670593ab9a4b002b`  
		Last Modified: Thu, 16 Apr 2020 02:52:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:869b054be7d001857ecdad8f97673228a71efbcabf8e8d598336720272a7ed1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53123934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9822202228ca7c667ce8f0631b1f005460b34212e0e292884ccc74a6e70c8043`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:42:55 GMT
ADD file:1175e5211df616c0061144ef189e0e4972721e25de7304d81f14126234b4bcec in / 
# Thu, 23 Apr 2020 00:42:55 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:43:11 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1831d7d095361283b5fc12083dd3b6702748739d46bc96b030aadf6dfb65f769`  
		Last Modified: Thu, 23 Apr 2020 00:48:31 GMT  
		Size: 53.1 MB (53123709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5550f45d064b7dce5076b86de7c11b525f0ebad9481b0c136a4412e7ddaf8ee5`  
		Last Modified: Thu, 23 Apr 2020 00:48:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:2c5ff7c29542ee3bd0bb1957764f633b50ad05898e1cac66f36f4d4b687a30c9
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50696359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c04cd5f22a1eaf19f4ead327fbb4bb4c70d6aa23248725359498c5b8e1660c59`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:14:06 GMT
ADD file:f4f731cdf85bc353f740a040496bad65f39a579c6a7ee34955a69c0e09ea983b in / 
# Thu, 23 Apr 2020 00:14:07 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:14:31 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5cd8c4531ac615911882437b1e6150cbdcaee37eb6cd1a20c0178acd6b29ab6e`  
		Last Modified: Thu, 23 Apr 2020 00:25:33 GMT  
		Size: 50.7 MB (50696136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a62aa1f5581f14603946532b9f2ef19ebd8d7536234a2c46950aa957a52b0`  
		Last Modified: Thu, 23 Apr 2020 00:26:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:4d866739b8a74a2b7c713ea8336b0c3126657c1b348c633edd92348da4f3c926
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55860733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe527ba2854d351f84371cec0974f8657bb5f72e86910695a359a65e48863781`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:45:44 GMT
ADD file:0647b317a7e884dc3e0962f057c40ce30983d26454377712ded21516f5a6c316 in / 
# Thu, 16 Apr 2020 01:45:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:47:11 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0f1b76c6e53151a809adac8940a52aafa0006e6ba49d57e564dde15d95e5742b`  
		Last Modified: Thu, 16 Apr 2020 02:07:42 GMT  
		Size: 55.9 MB (55860510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b971b58338efaceeab4e975334bb0af3442338ebef9f72a079f4b1e703e5cee`  
		Last Modified: Thu, 16 Apr 2020 02:08:31 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:b7064e1b3292023431c3a6eeccac96ffee94929b61a7bc63d17daaf02ea7b7a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50576666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa1970e33c157b4ccd0b452486203138f0bfa32507aa8a3cd538080f93bd27a7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:44:39 GMT
ADD file:087b26013a7688f4dc9c63a82d8357ae59ffdbd147a0625b6bac5af574fadeac in / 
# Thu, 16 Apr 2020 00:44:42 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:44:57 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:502638eee8fe0f7473b48aaf95f9f96a86eda464b2804b4fae2d44e497600148`  
		Last Modified: Thu, 16 Apr 2020 00:49:17 GMT  
		Size: 50.6 MB (50576447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e295adb2ee802a9fc7397e0dfff62f87cd288ba80745972f98b668636f4e45a6`  
		Last Modified: Thu, 16 Apr 2020 00:49:32 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
