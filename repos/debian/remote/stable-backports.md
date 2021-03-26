## `debian:stable-backports`

```console
$ docker pull debian@sha256:25ec51132d2ee812ca01078e3e8b00fa51dcf64939804b477b2ed74c2629a0b4
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:74f7542c588fd7187cb4ba93c8a5241b5eae027e8885ab6c5485143c967b83f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50400595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79c1d66d468394bd1bcca0df692a353bc47cb813542af4728d0965b24d2be8c2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:13 GMT
ADD file:2d14c2ad5bde045e369b83b6d2234a1c2ae24eddef0667283d9dd0411df7a9d8 in / 
# Fri, 12 Mar 2021 02:22:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:22:18 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4493a02e5a90cb3bf52c9ce707ea2ee32b0696c90ccedf8ca444b14906045c22`  
		Last Modified: Fri, 12 Mar 2021 02:29:16 GMT  
		Size: 50.4 MB (50400371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8efc407f9b221871d7412c425c9687be0f0fb217a8f593d1d00acca10309ecb`  
		Last Modified: Fri, 12 Mar 2021 02:29:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:7f6f423fb920ae2c1a1cd58ae8bf09171a58c9eec7d49f849c41439c048dc6d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48111928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8e80d6c81170e65186be58f60a9c5cc1b7eeefb20b5405db7bee194d7c41e1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 07:54:51 GMT
ADD file:a6c8f40e47f56cceaf581ce8f44c6ef882f06d12a1e5f084b445d6c67171ff8c in / 
# Fri, 26 Mar 2021 07:54:56 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 07:55:05 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a85d504283138f8dbc9f6e441611402a4ab846a70336785a9babbe9795a1d265`  
		Last Modified: Fri, 26 Mar 2021 08:03:26 GMT  
		Size: 48.1 MB (48111704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a7f75bf2df0db786a1ea44036349b051f9c830d1d261a19066885ea82fa8f7`  
		Last Modified: Fri, 26 Mar 2021 08:03:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:ad33c58c8c0687fdfeca2d0ab908632341cd4e8aa8f467da39792a89274dac06
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45868343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ca32aa6e4a1fad3aa1b284ae4aa2b636637c2fdec592bfd1f256f85f6a7d78`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:04:12 GMT
ADD file:da5a732a4236dec266fb09bc30762eed406258cf762a06cabf9f9b1f5f26080f in / 
# Fri, 12 Mar 2021 02:04:16 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:04:27 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b96f470825c2d993f1480ead850ebbb12798aaa397580685094d42ba4837e375`  
		Last Modified: Fri, 12 Mar 2021 02:13:27 GMT  
		Size: 45.9 MB (45868119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092aec2534332d2ae43e63548396c1f0984a357724679e6a817b21260c724bcc`  
		Last Modified: Fri, 12 Mar 2021 02:13:34 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:890b919348aea60de2579c0dea4494463b20aa7a2636544285eade27cb63b4ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49195937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bb17d0f53318af3ee5b8967a8ff4e596a049fbbc278d6b0af3470b328da5193`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:55:56 GMT
ADD file:f992611acc6a60f5341a1edb8258a0ff9348712dd61ed71c230129c4a3ca8f8a in / 
# Fri, 12 Mar 2021 01:56:00 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 01:56:11 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:343540e83bac837be28f7cd0502eb4aa017e241063d99372efd584a61f12beec`  
		Last Modified: Fri, 12 Mar 2021 02:03:14 GMT  
		Size: 49.2 MB (49195712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791655b28bf2fdd3bf6a23570a242382d16a3547d584aa71b21f5dd15a94580f`  
		Last Modified: Fri, 12 Mar 2021 02:03:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:b9e1457020ccf7bf0bb412df0cf9dcd6beb6786f84a09afd4a6bc89c1e0a37bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51160643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7a1c7e49df7d20c2a54c092fe5307e216489ec305a1f6da9ec85ada5ae2303c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:21 GMT
ADD file:9efd1740fd46dc73a76db440d5cb727f381d74b44179b07fd6406ad58ba14fc2 in / 
# Fri, 12 Mar 2021 01:46:21 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 01:46:28 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4d08b6d4d7202004f4e15c2545beb0d5f200ea348f23f1a6f124039c1128e094`  
		Last Modified: Fri, 12 Mar 2021 01:55:46 GMT  
		Size: 51.2 MB (51160422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0500f3e3e6ff569f7f13104472d20d9dfea1ac2c7309897dcad346d0fd63b6c`  
		Last Modified: Fri, 12 Mar 2021 01:55:58 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:96b7f504ffe30cf9874a4956fa6ac56d50b8eb1ba456e8684004671ed84b4426
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49029497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa939c308b407e202e3206462fb4c60c3c1f7b6b4d939fcbd25d272acae12291`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 08:11:05 GMT
ADD file:c594dbac49f9a1fadb44a691eb000b64b3acab66b618719827e70080cf9862f9 in / 
# Fri, 26 Mar 2021 08:11:06 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 08:11:13 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:50a5ed2929d8be8cc22ec80f8dc77df6d004975610ff0d7ac5339f09c6817819`  
		Last Modified: Fri, 26 Mar 2021 08:18:30 GMT  
		Size: 49.0 MB (49029273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22250ca3da298cbcb05f6e801060a60eda587f581fb83e35f470088b33c0553e`  
		Last Modified: Fri, 26 Mar 2021 08:18:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:749779c1f1c427b340ec89455b48732fa1a0589c17e52b875f95c327e1473f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54136471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d0d85a6a8f46084e9e497a03f9b22461421c10f27b63db61d316871903641b2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:34:05 GMT
ADD file:267748e1beadf987ecf20b5b319d4c45a241abec6f3e646b48fd3d4d2b55e29f in / 
# Fri, 12 Mar 2021 02:34:13 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:34:31 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:10f5d59361c87eb2f82bf73de5a0758e2e724ba9e54a1f49e89390a14e54951b`  
		Last Modified: Fri, 12 Mar 2021 02:49:45 GMT  
		Size: 54.1 MB (54136246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eed2c13940b77ca43e3cc57a37f183e0011ee0e8d853e2496be91339370438c`  
		Last Modified: Fri, 12 Mar 2021 02:49:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:5a0f07d027b5b2becb15ee522baf1b90b7b860c02f708e79b0503aaa78fa1b04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48969268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f560e25f3854d29f6b7ad95a35acf475e8cccc87103e117fbde45fae7e85036`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:59 GMT
ADD file:553bf2a7fd72a15a37cd2eb7feb5ac026b96dc5fc24a44b72ff654f046220a7d in / 
# Fri, 12 Mar 2021 01:47:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 01:47:14 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bbe3ef4f3f91c92b647969dacfef659272cd49375e880ffa19632458a210d548`  
		Last Modified: Fri, 12 Mar 2021 01:51:09 GMT  
		Size: 49.0 MB (48969044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90409ae434d9dbff3364087ee4307ddddd8830ea4e9c88a527622db714e677`  
		Last Modified: Fri, 12 Mar 2021 01:51:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
