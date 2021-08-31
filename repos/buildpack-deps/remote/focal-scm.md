## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:6315aec3d3d0c866c492bd9485e890c45a220196aa07c375cd62d8a3652ba2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a72c32c022e2d1cebdcbefa2fc0810ed6a0c7be253660f8ad5ea9c521ee826b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100680837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b4080e2629487fd86346ead8e8e820c05cb893949b1970238bd1ea0e4cc8ae`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:45:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:46:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844d0dd6bf6aa5959f603bad64a331fca5cda171d344450ca89c77e67410ac3`  
		Last Modified: Mon, 26 Jul 2021 22:11:07 GMT  
		Size: 7.8 MB (7769926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e2a2dd7363ebee0e3b7e3d44204409298c305ea2a5f38345f68c7b769033b`  
		Last Modified: Mon, 26 Jul 2021 22:11:06 GMT  
		Size: 3.6 MB (3624037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaacada9b3485ee466ed24e835156869e37b446a2fe7a324d2f9349b81b4d0e`  
		Last Modified: Mon, 26 Jul 2021 22:11:30 GMT  
		Size: 60.7 MB (60718930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dee7b6f04c4f83196ef597f3f808046a2dd9027ef167d781f8e63e8863dd65b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89389160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a657cdf3fbed62a72c2fe65d674734ce4b12fbee60d88edce235c8aa2e5a041f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:18:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:19:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0761e0b1ad0205162c66dfa83bf91ca0344921eca2bdd1d64b0970a5c75f0c`  
		Last Modified: Tue, 27 Jul 2021 01:42:27 GMT  
		Size: 6.8 MB (6767075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c226da21dd821a4b4f19689b2131f6e34d29095f42b4046f2eb48cf954e0076`  
		Last Modified: Tue, 27 Jul 2021 01:42:24 GMT  
		Size: 3.1 MB (3103731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305b0cc7ca4c4e47790a52a092d4cc7774810f9fee0f20387a45833bc8740475`  
		Last Modified: Tue, 27 Jul 2021 01:43:20 GMT  
		Size: 55.5 MB (55454116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:19b36271f8dc3c3e32d2efe26aee8d1196a466b9e9daa03445d90e2db344a923
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99176541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88006fc39d950f9ac4bcaac8419a7dcf84b7b72b94bfecdf46a55135c344309f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:10:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:10:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:10:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b8ef0ef6610d6e720afe76a3df03bf2afed7f16cc8b12dab2279c75b1c408`  
		Last Modified: Tue, 31 Aug 2021 02:19:41 GMT  
		Size: 7.6 MB (7636852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a226690073506846a68b797c6c96615eec776aefa661831f4abff3715172704`  
		Last Modified: Tue, 31 Aug 2021 02:19:40 GMT  
		Size: 3.6 MB (3600358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d5c6943027b3d6294ec2bbad85003c7584f70a77a2b64b363ee36bbf30920b`  
		Last Modified: Tue, 31 Aug 2021 02:20:04 GMT  
		Size: 60.8 MB (60766232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3c557088facf8e21f8cb162d5da3b29b0b4d22b7978c6e5330f1abcf4069d200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115856069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81f3ab03184adf9e5ddbbaaf4424797d4ab33a9a2a2acc21b05608758876dbd`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:09:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:11:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f198532bfc08536f5ad0c1f1242b55d34d7aac9ce9dc059a6109c2d7e20b7`  
		Last Modified: Tue, 27 Jul 2021 04:23:58 GMT  
		Size: 8.7 MB (8722787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8f157ddc9f96bd79c6823da12b4c54366d23b79691f3d8f39665ef321ff86e`  
		Last Modified: Tue, 27 Jul 2021 04:23:57 GMT  
		Size: 4.5 MB (4456512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a51a75aca451f998a1dcf27f7a8ece4fb2c2aaf4f7a09896e4664873136d52d`  
		Last Modified: Tue, 27 Jul 2021 04:24:25 GMT  
		Size: 69.4 MB (69386343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:87aef79db204a762d5f40f658ce076db36ab3efc621aa006c6405230ae43653a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98117720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b46e24901559406cd7200c4359b8f96650d7eb96bb6cd9a829fc4b415f1ad1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748dba3041b2bd31a240176639b763492a369d59b429da56c854b823820b27b3`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 7.4 MB (7428812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e0c13c39c1426302723ee65c5c58538ee64cf9d25b9629ac690cedd2a7169b`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 3.5 MB (3542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80abe2f24b0566481303d246a8e9996957224b079b7ff282fae87f647409e82c`  
		Last Modified: Tue, 31 Aug 2021 02:46:16 GMT  
		Size: 60.0 MB (60019295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
