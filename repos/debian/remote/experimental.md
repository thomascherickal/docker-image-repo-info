## `debian:experimental`

```console
$ docker pull debian@sha256:a398e43a5fa7d5940280acf0a86ba01d7bf63803a688d73e11c9a182d11cef99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:c7373e7ea5d8ba737558796032703d81347a1e17b32e46120b56e7e880141efd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51949863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f247d2e133ec7647447b486a1b828f410e5611235b0cf62451140ad9b0dd90e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:55 GMT
ADD file:eb55e131be32f7ea28d64283a0a3a09c157c58a7b7aadee1acbbe29762740b59 in / 
# Tue, 31 Mar 2020 01:24:56 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:25:14 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5849424bb1bf5e300d7218e461c40939164f8a60a7cfa279ea53a0d0fae8f267`  
		Last Modified: Tue, 31 Mar 2020 01:30:14 GMT  
		Size: 51.9 MB (51949642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7eba7b1f65ae7e782e816095c831d5ef6da4964739881a2a4a22c1f0420180d`  
		Last Modified: Tue, 31 Mar 2020 01:30:29 GMT  
		Size: 221.0 B  
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
$ docker pull debian@sha256:2b41df5eeb1591dbfdbb11adce452e371ce90e5e2e53ed2421d7d19909d9685f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50883010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:101eb6ba461a99bb9110f4c7cb2d07ea8095cfa9a55429f6090ba34e4f94594e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 02:09:50 GMT
ADD file:6b32f439e12aea74e183bfdbe74465986394f44d1977aff411df14e9d94e9be8 in / 
# Tue, 31 Mar 2020 02:09:54 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 02:10:20 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9a73cfc4057951fa3b653942a829aa795f75f40d9d7c3dea749c34b143cddbd9`  
		Last Modified: Tue, 31 Mar 2020 02:15:52 GMT  
		Size: 50.9 MB (50882786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4c8d13083fc37bf23a3c79c08338e7bee09edf34ed89df1c628efabece66f7`  
		Last Modified: Tue, 31 Mar 2020 02:16:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:3aefe45ee78c2b11f2b2114c516d05294eb2a21b11dab8687feecdeb75623e29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53085911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12901ed6b0618874021b04e1a5cb011ac3b1be515c3f698062da2db087838883`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 00:43:39 GMT
ADD file:88672776988a857aec646e66129c02ca354e07356c08ea8685ba7cdd8488dec3 in / 
# Tue, 31 Mar 2020 00:43:39 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 00:43:57 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:184cca0a947c292018eeb70034b2a59867daea7475d6a49f87251467b37969c3`  
		Last Modified: Tue, 31 Mar 2020 00:49:39 GMT  
		Size: 53.1 MB (53085690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4412beb36d1152b55414e51b9bfb58de1f7e331e05b5393400cbc273962bf017`  
		Last Modified: Tue, 31 Mar 2020 00:49:56 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:39a6ff67edc3c9bdda1c75075071d727b633d76a34956fdb4738891e6d93992b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55835144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2346fbbac0ddb5f17d9f3f66a8b8c379b3eeacf6c93849ea03aa7223a4e58bbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:38:23 GMT
ADD file:74a80c387973a5774f4fe95d7dc55f1b6c519d240c59edf690627d9a0e7f6171 in / 
# Tue, 31 Mar 2020 01:38:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:39:16 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7ae94100b5293d1ee61294c40974056b2c12f787904b73a1f9f3bd236ad387a2`  
		Last Modified: Tue, 31 Mar 2020 01:57:42 GMT  
		Size: 55.8 MB (55834920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa76c98211a7946c222da6c0dbaa628101d5a4472701e28977ad3cbe8b4b3f0a`  
		Last Modified: Tue, 31 Mar 2020 01:58:14 GMT  
		Size: 224.0 B  
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
