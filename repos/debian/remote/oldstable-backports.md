## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:f79d5d1c1ea2b5de529b5290c75121c5d8162987ee395cd45660c348872e6116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:96cbe179bda137453706c2fb1bcff9791bf7954502e728fa76eb12b4a61f3726
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50437256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8d00394c540c916c45931972a9321db681bbcb0066c0954d6f37727b94f7280`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:44:17 GMT
ADD file:8a4f1d7e5e52aa53b75f2808ce11c808a8e77c6404891742f522fb7a7e986f37 in / 
# Wed, 20 Apr 2022 04:44:17 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:44:20 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c45c7abc4a6b3c318a73fe816c8198b2491c4dc321a9ac23dd5ee43d702623fa`  
		Last Modified: Wed, 20 Apr 2022 04:50:13 GMT  
		Size: 50.4 MB (50437032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b310eb2a533b74f3b684fae98b6af97bd425384fc31bc31856ef9557a5ffd74`  
		Last Modified: Wed, 20 Apr 2022 04:50:23 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:9eef1bfa84a63b32add0f6fb0d3eb368376705d1a0b0f5d13d76ae8acb39e680
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48153811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a6ddd233e439acef3129bf25994a738fe0479e34c70a12c1e1a5a691b166971`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:19:14 GMT
ADD file:4d7d89b6490098f2e1b62cd1f0c77de4312f6ebc5563a0f8a8750c4818f47a2f in / 
# Wed, 20 Apr 2022 07:19:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:19:28 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fc45a926bdf002ad9abd6b8b8688c6fe998933998dc0c4ad013d1479dccac1c2`  
		Last Modified: Wed, 20 Apr 2022 07:35:53 GMT  
		Size: 48.2 MB (48153585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f236f4cc3ae736f495e1ec7a18233f6ceb35d6a5db334267cf17900f61895926`  
		Last Modified: Wed, 20 Apr 2022 07:36:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:aa244641b77ef5dfde72983f30478ff7f5302053790bbf82e5377262637407db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45914783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dee576f5e8d507c6454a001e9dcc5812158bd5fa30da519a0c61268901cee51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:21:06 GMT
ADD file:6eb791ed26da9f66900c8910f26852b98d89eff857c3b311da8cc84ab2c1fc6d in / 
# Tue, 29 Mar 2022 02:21:07 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:21:19 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f2c3d159380c9c644e808e974c1a8c35f654cbb83a1efd058d01343006270c2f`  
		Last Modified: Tue, 29 Mar 2022 02:37:17 GMT  
		Size: 45.9 MB (45914560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa4e71ba95ce6c640965c2257e878dc526e668abf4450ca3292212cf09b951a`  
		Last Modified: Tue, 29 Mar 2022 02:37:28 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:2cc0a75cc76b25edd5f8f5125fb35300d64aa8c3bbe5623f25d471c640f3a726
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49227940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c2a64e9ebb6d4acc67c28de26324c208f6a40e50a89548a9209d30261e08ea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:30:12 GMT
ADD file:55626f1299c943934f8cd38ec9a9cde4d4b8beede74a23774f4fe6ca0b7ec45a in / 
# Wed, 20 Apr 2022 04:30:13 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:30:19 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6d6f4a9b5619dae92e0d604298044fd2a8ed8c396fe01e6ab40d3f2bd5605473`  
		Last Modified: Wed, 20 Apr 2022 04:37:38 GMT  
		Size: 49.2 MB (49227718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0d06947fd270084fb3f4d8cbe2dd6f4b7b7e3ea4b15b9ddce40569f59960f5`  
		Last Modified: Wed, 20 Apr 2022 04:37:49 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:e48dcd70d79303ea68def419ed805d2be9cd9c7fe944b6c7e036b70f715f1b14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51196061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66e73c39534eccffd38212da259cf541310ab2843a0456c94d9cb17135f6cbf1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:42 GMT
ADD file:19e770beac41792d9baa38c96e3426b5d62b0526bba5ee4c638295c30d0f03f3 in / 
# Wed, 20 Apr 2022 07:38:43 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:38:49 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:58502976986d74622893d9aa344c104e0e78fb67c58c87fd7088cbe5c6805d35`  
		Last Modified: Wed, 20 Apr 2022 07:46:49 GMT  
		Size: 51.2 MB (51195838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6d1feb32dc131b86ad765ef22b9b5d40bf7f834b6189442563ae49404f4fa9`  
		Last Modified: Wed, 20 Apr 2022 07:47:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:195cfc4c88e902d9fd7799b55c56a54dc4440d0756a646378d2a4c17b581b763
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49080099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef4f643d413d25802e663ee90b69ccba4a8b00d1502dcde33ebda8e98951edf3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:44:08 GMT
ADD file:2d8c34802d0b44aabd27e95eff2ce94751098f2cc68aae7f789185fd8aae0d0b in / 
# Tue, 29 Mar 2022 07:44:13 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:44:23 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bd194f847b7470ac501b6bd3620e76ed1178f748e2cdc221ee013f7d5c74b72d`  
		Last Modified: Tue, 29 Mar 2022 07:55:01 GMT  
		Size: 49.1 MB (49079873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a3c96700fbe540f5b46f50c924617ad1e1b8807c5af7c41c263a598e31488f`  
		Last Modified: Tue, 29 Mar 2022 07:55:17 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:d23065ab45378951f00db916eb4aba0d4bace807f7447c3ce41d1703e247abca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54170162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561ac87780f529176713452b3f3f0e67e5d5cb08f7529d938be52cbf9d79bc2d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:48:12 GMT
ADD file:ed5800f209002e99add8748fd1a1f5701a24178942a2ce172d2bea191a3933a1 in / 
# Wed, 20 Apr 2022 09:48:20 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:48:35 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e7ad4688b6e90819e677c7353bd462760334d88e75dd149723d5df19b4f8abd2`  
		Last Modified: Wed, 20 Apr 2022 09:58:34 GMT  
		Size: 54.2 MB (54169935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e0d9921edb11b71468cbb29cab97b4395614d904fafa3c1392593e8e9b6bb8`  
		Last Modified: Wed, 20 Apr 2022 09:58:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:8bc60865b92ae4ed66f9aea5c2b7fcddd226a9d2ff7084623f3c44a450f4ba59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48999487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36bec06d9249882acf48ac9348e6da4eea39fc34a60da5d84a4d40305986165`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:41:11 GMT
ADD file:6f25f699dbf6ffb4c1440b1d592fca93d523bd9d8db26167cb18b1ab609c5bea in / 
# Wed, 20 Apr 2022 08:41:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 08:41:29 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e78d245215ba52c813dea79f6c77d96b807db3a4255717eb46d340e59def4bed`  
		Last Modified: Wed, 20 Apr 2022 08:50:34 GMT  
		Size: 49.0 MB (48999263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a528526ff08e607b03c9bb88ea282d83f01947cbf231612b0e4e8d551af5e14`  
		Last Modified: Wed, 20 Apr 2022 08:50:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
