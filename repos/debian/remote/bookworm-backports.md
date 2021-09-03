## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:455bdc9b1c5d8818cb5202e2e43658b2036ba1ad650bfdac4ca35bb45d49cb2e
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
$ docker pull debian@sha256:98b79f625aec6cbf0905e5cf1997fb96ff925ed49dded97d5b64e92b26d416f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.5 MB (55464952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2753d942e16377d4c5c80ad69d0b889be016a613cf92a15ac65b9e6208cd0a13`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:20:37 GMT
ADD file:b3abf53bbd840b5d0caa3caed8a5e2b14e1ca06a7890d6187badc0bf84c9bb34 in / 
# Fri, 03 Sep 2021 01:20:38 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:20:46 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c6b538e7fa83f0a49e0b09b7906a3c49f5127fc7244579b32c0e30a7f87ab905`  
		Last Modified: Fri, 03 Sep 2021 01:26:09 GMT  
		Size: 55.5 MB (55464727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55e138f0b4a34079339d900f887c798ddad10591207e555208744cedcb70210`  
		Last Modified: Fri, 03 Sep 2021 01:26:20 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:752efbe09a079971fc51e0eca0b7955851a6132c29208b3e398792edff8656eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52962725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f311e80d57663818d6538df3bfc9f45e7df6a4084aca1d119cb7f05c73004414`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:48:59 GMT
ADD file:87d4bb1f0d2bd4a51a7b029729c25e5c9ba11c60ff37eb54f5d44aac9dd05c90 in / 
# Fri, 03 Sep 2021 00:49:00 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:49:11 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:595063d6b6f25205b41676ea8bf8baae9b7e5ca5cb61323cce21f922c3775a65`  
		Last Modified: Fri, 03 Sep 2021 01:03:24 GMT  
		Size: 53.0 MB (52962500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf975968a4a2e0222e257d6701229b91703cc715b563da8de1044243c4cf5c`  
		Last Modified: Fri, 03 Sep 2021 01:03:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:9edff494511efea5bb5e2e9998f2b3aea9dbbcbf1bcc033dcb3d5aac480a90cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50611927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d03616513b67e62e8000fc3531840221bf34df6109297aecb63d642df393b3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:58:05 GMT
ADD file:28018c1477d768b73c22f034e36316a011bcf20f0a06bd01a99de6a19becb514 in / 
# Fri, 03 Sep 2021 00:58:06 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:58:18 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8cbb380297181b10b2232513a4f88949ebedc1ebb60f176c3e6d7494e5ca254b`  
		Last Modified: Fri, 03 Sep 2021 01:12:49 GMT  
		Size: 50.6 MB (50611702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42272e0f093e0c2feb988dbe3538119ebbdecd73033d2f116d567041cd63ec14`  
		Last Modified: Fri, 03 Sep 2021 01:13:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:379d571b7a06b14a2a7ccf018c725372071f0b996f2c5fccb372257c9799a20c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54510321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66fce5d38b9deb1a5b1c4b39b8ff2634f93e07869412a23ce4696531af5bf923`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:55 GMT
ADD file:ff057904bacde7a459057d2a1f17f75b0ef999b8af75a3946b96be1cc867dc5c in / 
# Fri, 03 Sep 2021 00:39:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:40:01 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a8ede13fedbf244b8f95af0d62d6e42f0e301a070c97a956a39c33bca3379f43`  
		Last Modified: Fri, 03 Sep 2021 00:46:24 GMT  
		Size: 54.5 MB (54510094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dfe2f88354ce411e9aa7e4984397850828a3be23dc052303a40dbcd8ffef22`  
		Last Modified: Fri, 03 Sep 2021 00:46:35 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:289601165a4621338763b9149f4fc9b0b7e85b2d83b4b92806fe715780c9881f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56509228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61036ab828d5030540cfe945dd45dacf1ef6b9071e14ca0e78f4a0162ccc300e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:03 GMT
ADD file:2a2a117c9516418c2782edb340fc34f10f1af67ade1189c7ec46a16933f76e6e in / 
# Fri, 03 Sep 2021 00:39:04 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:39:10 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1bde0c2366a3f98cf069a3d438f9065010d27a96ebdb2138fb741604c1fe19f0`  
		Last Modified: Fri, 03 Sep 2021 00:46:38 GMT  
		Size: 56.5 MB (56509003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace87698ac37bb338a479ad0d55dd5e63cf44a2a305db858b89f5d00b9a9c1bd`  
		Last Modified: Fri, 03 Sep 2021 00:46:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:ffa9f8dd122f695a1573e3bb4b217fbe1e1cdf7770308ffb951020372639c87b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53802306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b84a1ab9a4edf03f48d6cfb3c8de52e2b16e801aabe2a883fba4afcc1eb2e24a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:08:46 GMT
ADD file:fd4f41920f6da2199c3a6438b174d6f9645f6bccbb15b7bfad1217816b252dfb in / 
# Fri, 03 Sep 2021 01:08:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:08:55 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1fde5974b9029fc3967cfcf4e7665b974d0488fc66fa5f037257f98d58365898`  
		Last Modified: Fri, 03 Sep 2021 01:16:14 GMT  
		Size: 53.8 MB (53802081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafff29bd99b7d3aa6014f2e813d78e8c0eda03b3759e23e9297034c6ee9829c`  
		Last Modified: Fri, 03 Sep 2021 01:16:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:9eba3035857ca484bd0414a59bf8857405a4c64bb25c34dcb30d821c85afee6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59526527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab5cffaf828f98f3f994f38221c6f3d681194e504efd9c4b4be6b1c3be3ccb95`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:20:52 GMT
ADD file:8c4f85d12b49771f370ff2d26cbefa13b6abd92b68531781c09d00ca174457b2 in / 
# Fri, 03 Sep 2021 01:20:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:21:31 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:842eaf445b44995004f2497f1b8419fb7e9e38e2348927060a6bd434d949be24`  
		Last Modified: Fri, 03 Sep 2021 01:34:04 GMT  
		Size: 59.5 MB (59526302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56c32a2ad1caa58a0d62c25d6c203a249e19552ba2bdcd222df920eea3faae6`  
		Last Modified: Fri, 03 Sep 2021 01:34:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:045f7287e8e6c65b564316bf4753f546750ae2ae2bda32ef696ee1a1b7e5ce5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53750167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3eeb3dd89a7b0f209000d675fd964077301d8a9131b8b7b02b3cf1de9bfc6c6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:55 GMT
ADD file:e73c798962eeb5d20834ebb4927afa2388c767fca5f0cfe4bee992525ae52587 in / 
# Fri, 03 Sep 2021 00:42:14 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:42:26 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9a221ac94f84eac2fe722cd5a1cec57bf3017ea4a544c69178ada20a3bdf56c7`  
		Last Modified: Fri, 03 Sep 2021 00:51:51 GMT  
		Size: 53.7 MB (53749941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b742147984fc6fedc841b6b864680e02a8e1d1a798e57b5e5bfee8c8d82771`  
		Last Modified: Fri, 03 Sep 2021 00:52:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
