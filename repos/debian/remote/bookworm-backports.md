## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:ed29f21d82a900acdaca784d4c8a51bef617ee991c9552ea4b45475fc7cb21a1
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:7572fe8db8d3136cdbba32935d446b8a307505a78ad0a78f4845e2383cd57418
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55560967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21415118c1585cb9a3ac52999342a1858d5f2275d858e3df51d4eff2f89e9c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:57 GMT
ADD file:049a34b0a455f2d6bb7472efc8b4fe28600f9b16fcf86c66e654f0d7f96c617b in / 
# Wed, 26 Jan 2022 01:39:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:40:00 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:174dc37d1760a198250a591524de55fe80951eb332d1b5fda14aa58b2d0274ae`  
		Last Modified: Wed, 26 Jan 2022 01:45:22 GMT  
		Size: 55.6 MB (55560743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82816ec617559c9a376e9caf91c28afbf3665d7ed51b3ea73ddd3a21757282d`  
		Last Modified: Wed, 26 Jan 2022 01:45:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:16cb46542b1416c299cec144e1a8686d3e77e875fa49b7e83f0dd15a9cecaa4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53020412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1730a3639397f2436b7ceefad15dcbc2f751596631c33f0d4616981849039f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:23 GMT
ADD file:2b96a854a3c9d11256be667f9d982d7d8b9dc55dbebd8b4b5fd405cb278a1c64 in / 
# Wed, 26 Jan 2022 01:40:25 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:40:37 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:63d07b82886a825f18700c37fbcff6322772ad2aa7c6337ed53204a0fa13480d`  
		Last Modified: Wed, 26 Jan 2022 01:55:24 GMT  
		Size: 53.0 MB (53020183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8580736370739092690fb2221445f6f769d250aeda3ebc60e23d364e112393d`  
		Last Modified: Wed, 26 Jan 2022 01:55:36 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:4ef9ec389030b8b1e96337e0a776b6c4cd178c4d690d7f94e343e450f6fa5b35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50663005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f64bd3a673226b82688bec8fae76ff2adfac1e0e995d6a6a939cb3a475a03358`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:29 GMT
ADD file:0d5c36134a34929922dcd5c83256b9539a94c46d5b7dcd23ae6cc29721bdc320 in / 
# Wed, 26 Jan 2022 01:40:30 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:40:43 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9276ec53f1a5aac51c0a8a27bcc855b50a696f144903a4c1dfab1a458f7f7af0`  
		Last Modified: Wed, 26 Jan 2022 01:55:58 GMT  
		Size: 50.7 MB (50662778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c66a8947fe8e8366490e23e84260da5e4b5851af73edcc6d7556da34c3024cc`  
		Last Modified: Wed, 26 Jan 2022 01:56:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:8a9d4bac7f335de8d42cd8aa51c3561b05f1df343b00789ff1208cdee83a74a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54535472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcb0003ddbd54be2a34603113d391a5474537b9474a919ffe9d0949c9cb66694`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:51 GMT
ADD file:585d9a04ed59d36d1ee8be3ad5a7a488962b12f0b7d737826e25a7ab617521fe in / 
# Wed, 26 Jan 2022 01:41:53 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:41:58 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f9f8cc8e22fa2c53a109b770bcaab20fb907dd9957eb312d9f49000ff4185f8c`  
		Last Modified: Wed, 26 Jan 2022 01:47:52 GMT  
		Size: 54.5 MB (54535243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e8683350644d3736f355f49633e8b2a1a2c0943b9cc2906abd6622c1b0a963`  
		Last Modified: Wed, 26 Jan 2022 01:48:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:b8b1fc00ba118425325ff94847bae4e05687ea1c5d369656616697d110dfef83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56598371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c6be8e89c1350a83f0e6bdcbf6503e079315d502e44d8a3d72d8c91a97eb8b8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:06 GMT
ADD file:49bb0653fde7eea7609e6ad9bea8c405d8a514818936cff57f87f5fa321d2582 in / 
# Wed, 26 Jan 2022 01:39:06 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:39:12 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1308dabb988bd1e94f15ca40572eaddec8a0de059ca7c28b6a83e6821441d6f8`  
		Last Modified: Wed, 26 Jan 2022 01:47:24 GMT  
		Size: 56.6 MB (56598143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f932d46496cf03190202dec1a4c5be85cf032001ab02db13aa29ccd68e62e1c0`  
		Last Modified: Wed, 26 Jan 2022 01:47:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:ffaf4da7f2800690f6945131a5965656aad32e49fab908a7d0718f74252570c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54262267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1540a2bb7c9674b98e2effc3a0782099ebf3d2370ee7608d827caebf3d16cc8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:27 GMT
ADD file:cb994d31e0dc06b73ce5e197fffe27837867fce8ab87a858b9668290c97bd7af in / 
# Wed, 26 Jan 2022 01:41:28 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:41:34 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:45126d37a1c34eefb327242a121bbca1be988e1e2e1cf037fde7eaa131fd6db7`  
		Last Modified: Wed, 26 Jan 2022 01:49:20 GMT  
		Size: 54.3 MB (54262039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c6decd96078a5c54b2a00bf1eb695351a509e70f35c3b16a1f7c0577678993`  
		Last Modified: Wed, 26 Jan 2022 01:49:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:954b86807a35030c494ab8b5136ce0777154a0d4fe0ff61aa8794bb2e22bfb47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59942405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eedaea0fefb1e6ba3d87887c3bc626fec2126abb917bf66cdd905ba9d3f2fe3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:20 GMT
ADD file:815d918aa7e03d3a0e2d0dd87d7d9696feb37b5054d103e1ac83847b08e877a2 in / 
# Wed, 26 Jan 2022 01:45:26 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:45:39 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2fe2b17ea8278b5a905731f1d003664a61c7774f4a23cda61a596487a1b51210`  
		Last Modified: Wed, 26 Jan 2022 01:54:29 GMT  
		Size: 59.9 MB (59942176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bd39111ea4d04f1f223f4f8c863204d76b489d0d4f7f9935fcb0aad85e6f02`  
		Last Modified: Wed, 26 Jan 2022 01:54:41 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:337b6d0a2e83376b0405ddd9b3af3b6d327881670938ca76e1f701eba46a92a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53837323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ead7dd3b04a922a5a441eaf05040e1a87d732b9fee733c23e426869633b4c3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:21 GMT
ADD file:b56123b23454cb9db7a2a2e19c5219cf5643b8692bc247ac4212732f2a8d218a in / 
# Wed, 26 Jan 2022 01:40:28 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:40:34 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4155c67ca83ba1ee87acdfb0ff7b262e769e0a27829b9b44ca097c4ba1e29ea4`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 53.8 MB (53837097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e985ecb4e36187550701ad21c91b60fd5b56a191be4589bc7a296342d5527e2b`  
		Last Modified: Wed, 26 Jan 2022 01:46:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
