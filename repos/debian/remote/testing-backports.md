## `debian:testing-backports`

```console
$ docker pull debian@sha256:3ec93e25938f6f605d6bf5a362dbe92c34bf4d6d5cdfa015b3be94927031260b
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:ae3b9eb2947bcd89648ab9b14b1c67d736e1f6b247743c0966e81d24f7f2f35a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54102749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0575c221e2cb39bbf3ea7456b42551564b878315035ba6aef45885607898f499`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:07:27 GMT
ADD file:f87e67a50d51914c2d4d77ad9fb2395ec8f720b21958111ea5e493ea7b788d12 in / 
# Wed, 22 Jul 2020 02:07:27 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:07:34 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:73b408cb748b0d1dd55d6ee6f4be6beddeeaefef08a2f1733d219cfa7c8eaf22`  
		Last Modified: Wed, 22 Jul 2020 02:12:41 GMT  
		Size: 54.1 MB (54102525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f72e30863d53058c856c7b0f2fda777954df739578ba0dfb268ec1d85acfd0`  
		Last Modified: Wed, 22 Jul 2020 02:12:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:a2cc3c61b5465f2e3864b836a4a4ea018f2fd411a6a7971ec71509a6ff886f7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49784730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bda10c44cb33e62a133ad0f79884e41c2c45caac32d10fadbb10fae58ca8d41`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:26:11 GMT
ADD file:187c521285de33d9024f13e882a0a77eb73fa40812d206146aeb6ffee3b41d93 in / 
# Tue, 04 Aug 2020 03:26:19 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:27:00 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8aae9c3601b98cd2570242d799d9ee7afb8c97a1007181ac9ae997042c2d08b3`  
		Last Modified: Tue, 04 Aug 2020 03:39:19 GMT  
		Size: 49.8 MB (49784505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9731bb2fbee23630f5645430701e408633f38b3e0a3eff143404abd5cf00c36e`  
		Last Modified: Tue, 04 Aug 2020 03:39:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:c13d981aaa6f0876c9c686ee1e5f124b6a0d3246b53dc2c44537b8552d0bc7e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47570702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4eaca4d22fa2edd4d94e6f75e27175df72c18b4a7355220e3b4c79e72c8387`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:52 GMT
ADD file:c87cca340a64bf8c47ea42d353b472eba58c679d0346ca265ea40e979d8adc8f in / 
# Tue, 04 Aug 2020 05:01:54 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:02:02 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6de6f46d5cde63d39bdf0307e4aca1b00858eca00dcdd17496279110ae989555`  
		Last Modified: Tue, 04 Aug 2020 05:09:25 GMT  
		Size: 47.6 MB (47570478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34156550e93302068ca3a8aa04b9ba4643af4343fef8f7419717aa6bf10c2d3a`  
		Last Modified: Tue, 04 Aug 2020 05:09:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:0f8e793be605d691b8df3261608cd5965ea5fe427ebf022e7a63328d9d20d8b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50752073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f1dbc14a11e6bedbb9fdd7030d487c9bacec165b9f0f2ad4643c804a3d9cd6b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 07:00:45 GMT
ADD file:725f94f7e6e800981fa8f39228f0ef03900a97a621fb2415173496995bc2de4b in / 
# Tue, 04 Aug 2020 07:00:53 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:01:04 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:059d2624bd4cbe096feccc25cf0f53c2c9f670f108be6124ea6aeb3b78724b69`  
		Last Modified: Tue, 04 Aug 2020 07:06:56 GMT  
		Size: 50.8 MB (50751849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb7cd0063eeacb154191b36b56a2c431184a07b63d87a819d23f93e64a0c6ad`  
		Last Modified: Tue, 04 Aug 2020 07:07:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:7dfc7661280267803ab00a0f46399357ddca4e879c7ce7f7402cc61eba12e2c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52909923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f233e4f2ed10742f1784c7cdb1d70498d2314abc4200142fd3ebf17c1817b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:40:26 GMT
ADD file:37d069bc693b5dc1cf3f5afa51967bb38b27e28e870341db5d25eee7577a3c38 in / 
# Tue, 04 Aug 2020 03:40:26 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:40:31 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:12dc0ff6b6c89bb67e2fe16bad31f939115457037b3e5b626ac0a1fc9a1d54fb`  
		Last Modified: Tue, 04 Aug 2020 03:46:09 GMT  
		Size: 52.9 MB (52909697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c31a0415abd39f740f099f54b68250970a832bc7a0c6dd2c07d19638e1e384`  
		Last Modified: Tue, 04 Aug 2020 03:46:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:c9a1b4420dad423628e6ebd6f69364984b4bd22bacda45056c98ca9ff88ef989
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50550999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc551cb77ec5d96f55b00c307649afb2bb9f7e2962274950c078fdd45a9ca49a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:44:20 GMT
ADD file:a53836046b0070207f3bd1a278810d10133a25b6349c816dccf4b727a71faed6 in / 
# Tue, 04 Aug 2020 06:44:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:44:27 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3a0317c61d2d4f59c9c7065c26ee123ab008467a8954cde60d1d216013fb93c7`  
		Last Modified: Tue, 04 Aug 2020 06:52:09 GMT  
		Size: 50.6 MB (50550774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc0fd2bf7883f64c62cae3e1e3fb5469934bbd84462e1d01ee3bf8fb055a0ae`  
		Last Modified: Tue, 04 Aug 2020 06:52:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:b4d26727d87d305166a5a928f7d79740a7dd52d0d209b3f548924fa90390eff7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55656136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78805455d57b37879b9217945a4584a9f0a71bea9ded801e9ef7ca3ca35acc65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:47:25 GMT
ADD file:9716ddb36e63999f28bcc07b306d92cd35c4756a6acde3756dbea757b729c977 in / 
# Tue, 04 Aug 2020 04:47:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 04:47:44 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cd5f9f7e65334c771d2f0cd8807ea5d5471b03ab32cd37132f270f6823fa6f2a`  
		Last Modified: Tue, 04 Aug 2020 04:55:20 GMT  
		Size: 55.7 MB (55655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b474f6d62bf8aea2bbe1eea581efe6282977066d7245e4700fdb02efb4c679`  
		Last Modified: Tue, 04 Aug 2020 04:55:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:c106c833bb51628dca35b6953d6eb5ccf8ea2e4ee94a5f24e24fbd0a72ffad65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50416994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f077bfea59d9d68ec196db0dbc6b46607dfc48b2e45ae2efefffaa2c429e253`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 01:18:08 GMT
ADD file:87c6bc96e112611ea9270b13a2a63f740c69d75d0d16c0633bfefe826cd3d1c0 in / 
# Tue, 04 Aug 2020 01:18:11 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 01:18:16 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:427e125cbccb0b2c09e8ac1181fc23797930ffb9685be2271427231984a38365`  
		Last Modified: Tue, 04 Aug 2020 01:21:03 GMT  
		Size: 50.4 MB (50416768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4373ec860ecd6bfcb3213600ca8a0ddfdc08e143796892174a3408250bb46938`  
		Last Modified: Tue, 04 Aug 2020 01:21:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
