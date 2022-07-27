## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:6298c32b00b8dda9010116c47a9a8ca7307197a53d5649251305b84b7b85e3d6
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

### `buildpack-deps:scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:42120dc883ebe0e6a570941d6f09532a56d8a382e1b2930f40f9e4c7c38e7ffc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125610938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff6491b3adfd3862acbff5ac99938bde008f8ad65c60c1aaaba9c209764a7f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:19:57 GMT
ADD file:3451708ab45bc1bcfc1ebb2075d3af16767477cbeb79334959e0d1ff02b0864b in / 
# Tue, 12 Jul 2022 01:19:58 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:48:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:48:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:48:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d836772a1c1f9c4b1f280fb2a98ace30a4c4c87370f89aa092b35dfd9556278a`  
		Last Modified: Tue, 12 Jul 2022 01:24:06 GMT  
		Size: 55.0 MB (54999406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a9e63c657ad881997f5165c0826be395bfc064415876b9fbaae74bcb5dc721`  
		Last Modified: Tue, 12 Jul 2022 02:55:03 GMT  
		Size: 5.2 MB (5156110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1989b6e74cfdda1591b9dd23be47c5caeb002b7a151379361ec0c3f0e6d0e52`  
		Last Modified: Tue, 12 Jul 2022 02:55:03 GMT  
		Size: 10.9 MB (10876416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28818711e1ed38df107014a20127b41491b224d7aed8aa7066b55552d9600d2`  
		Last Modified: Tue, 12 Jul 2022 02:55:23 GMT  
		Size: 54.6 MB (54579006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:5fb6bde944c51b5b74b90fab28680d6bf466bc573171e4d01af8cbd9b0da5ffb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120490817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0753ca6c153aaa14a02f0db4a18f95e732d31dc4517c6e0ae0c92769f41aaf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:49:58 GMT
ADD file:a600937adf471d1624223b1e4fc5af3391a3258d28051f9f9990c978177db2ec in / 
# Tue, 12 Jul 2022 00:49:59 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:38:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:38:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 01:39:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:458c615f383e394cdb1d249caac254a3148895cc59ef0f317e0c342507c0a43e`  
		Last Modified: Tue, 12 Jul 2022 01:02:12 GMT  
		Size: 52.5 MB (52536893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79ef49a3b907a2575e08477212bfbd57aca6b32371844cdce520dc7a2e688e`  
		Last Modified: Tue, 12 Jul 2022 01:57:42 GMT  
		Size: 5.1 MB (5065360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cf6d68feaf378688713585399ee409bdef4481481b83d4896d6861cb380c90`  
		Last Modified: Tue, 12 Jul 2022 01:57:44 GMT  
		Size: 10.6 MB (10573756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e72d965a8962ee5d2e575801caee59ea34cef71d8b95f502fc38b6c201c9f1`  
		Last Modified: Tue, 12 Jul 2022 01:58:38 GMT  
		Size: 52.3 MB (52314808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:794b6484aebc000274b029042cc8b526829e4b409b780989dafb00467f3f80b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115667580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c07ede1a52f9833ae655318d6c747ea0fd3e9585cd19bdfba55dd877d54073b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:28:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:28:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 03:29:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042ae471fd57ff8851607bf0b66366fbd0a499a0ce088f1fb39c5a1caf4123e`  
		Last Modified: Tue, 12 Jul 2022 03:50:27 GMT  
		Size: 4.9 MB (4924746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70da2acc639b7236796e6cb2a0b0e3a21e6f32f8a507bdbfb823a510caf8e75a`  
		Last Modified: Tue, 12 Jul 2022 03:50:29 GMT  
		Size: 10.2 MB (10218056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f084d2e4e20e27a866ad87c0a2098498eddc9f471988ea44068990b299a29c`  
		Last Modified: Tue, 12 Jul 2022 03:51:21 GMT  
		Size: 50.3 MB (50329897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7933ee0b04b362bc912a1891bb0fc1b26b57003242f59c490f0571140a2c8d69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124157409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9878ef529a99304d4d8da799b27d263a9682da9a4407e1688c4f8481a90df913`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:18 GMT
ADD file:2dcc013bca5a420cad3b6a1ac61f52ea58a29ae05fe282078a744979c0e1a89e in / 
# Tue, 12 Jul 2022 00:40:19 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:33:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:33:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfc947b533a3ed8b8ce79820c7fe5e7634bf9c08479ed0aee1e74ee7b4f2b068`  
		Last Modified: Tue, 12 Jul 2022 00:45:41 GMT  
		Size: 53.7 MB (53683129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca36aa4204d2a708dcd1d41d1d4a128b095f8d88a2f9544f89799c36914e356`  
		Last Modified: Tue, 12 Jul 2022 02:42:29 GMT  
		Size: 5.1 MB (5142960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdcd2014de70fbce8c43a70cd1f42bceab4f1e35953db987fc318dbc0fb0d26`  
		Last Modified: Tue, 12 Jul 2022 02:42:30 GMT  
		Size: 10.7 MB (10657500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e288b20a616767a00416e22f7d8ee6390ba5b48061d92577f55bdb11121e6946`  
		Last Modified: Tue, 12 Jul 2022 02:42:53 GMT  
		Size: 54.7 MB (54673820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ddbe43ca0698552825f5c973e1128e5c670a84e8719a8ffe00455eb8a36c5518
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128234057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c22fb45e4cfe2cdcdc6d87833c33af0cd9a715d0ad66490b3065d116c3add21`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:10 GMT
ADD file:0fe47b589e2fdec2c7f7e92ab50ee94c37df9276c6771e612d29fde3aefb04b6 in / 
# Tue, 12 Jul 2022 00:39:11 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:26:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:26:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 04:27:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:992c2740c28ef02c375c076416e9a24c9172d5343205500b8388cf087a76bbce`  
		Last Modified: Tue, 12 Jul 2022 00:44:46 GMT  
		Size: 56.0 MB (56001770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b010a51f3f025a5092ebdeabc7eb1a2c2b64a0782cb5f2848c30055d5561437a`  
		Last Modified: Tue, 12 Jul 2022 04:35:57 GMT  
		Size: 5.3 MB (5284906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d877135d65d11955788587fb1d70efe0d09ac15edfe3850946b5237926fc322e`  
		Last Modified: Tue, 12 Jul 2022 04:35:57 GMT  
		Size: 11.0 MB (11032943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5afc941d55bf77416ea689331bc9b09d9ea20aea0c8661c44e4840af148c20`  
		Last Modified: Tue, 12 Jul 2022 04:36:20 GMT  
		Size: 55.9 MB (55914438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e240a6ad93dc3d00a075369445c4a82b56bdd75256fe9d0795a2fae6108cb1ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122340590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b5f52457d0e6997fcfce37f2cd26c3d0612517669d930b4fecc8a055851ce4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:40:19 GMT
ADD file:5a045303c511235feda23815b401564f1db25de2c312598258626e9be22c303a in / 
# Tue, 12 Jul 2022 04:40:23 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 06:09:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 06:10:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 06:11:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbe8f2bf6b579db32fc573a5f145cbb10fddffc9fced5f528ed1b70b2c18dd94`  
		Last Modified: Tue, 12 Jul 2022 04:51:00 GMT  
		Size: 53.3 MB (53263285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3283d319938af21e206873861ea7c615ffe89e2770155269213eb3801ea6ef02`  
		Last Modified: Tue, 12 Jul 2022 06:40:24 GMT  
		Size: 5.1 MB (5117493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169e575c90587844ab6e7ee2c27f5389c260d537f4f69c2b3b97e313f2114791`  
		Last Modified: Tue, 12 Jul 2022 06:40:26 GMT  
		Size: 10.7 MB (10660566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea6ddf91fa6d28cbbcce640b99b4dfb8df5cba0699a38db6924a2ba12136487`  
		Last Modified: Tue, 12 Jul 2022 06:41:17 GMT  
		Size: 53.3 MB (53299246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:68449c2a0645b809df5c85daaeb28acd4c1c77723a11b242472012fceda9fba0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134784139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9fde2ac9be389a7a76a500d9eed134de6125428003790a364a5c02d4cbc590`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:24:58 GMT
ADD file:98243e1bfc9c04ce4d47bbf13011c502c01aeea3a0417b4e2b8f90b4debfdd32 in / 
# Tue, 12 Jul 2022 01:25:03 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 22:32:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:33:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 26 Jul 2022 22:34:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6fb3da208bae11b3dc38c4ab84ad048c030a1da966740d02681a11866ba2230c`  
		Last Modified: Tue, 12 Jul 2022 01:35:06 GMT  
		Size: 58.9 MB (58895620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e755f0c9224d9a09cafb660e90339be47b26c4c9584cd9d94ee5c943beb9e0af`  
		Last Modified: Tue, 26 Jul 2022 23:47:52 GMT  
		Size: 5.4 MB (5405301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881c506b97552bcd229e65b7d010773118d7abbcbc802525defa3481c7243e7b`  
		Last Modified: Tue, 26 Jul 2022 23:47:54 GMT  
		Size: 11.6 MB (11628514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec75d0c4cfdabee064149a9394d0a742aa9af2d5791f5115e28291f13f91df3`  
		Last Modified: Tue, 26 Jul 2022 23:48:29 GMT  
		Size: 58.9 MB (58854704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:865d9452e5ae29eebd08f8c0660149075aa14e5ba6a9538de452fa08f6388c2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123221378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c053d2093596a8302fa9be73df2d7f1f16bafed268c3643eb3482b171c2b246`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:43:15 GMT
ADD file:2a729374ad3e12361206aeffbdface900970f010684d6409328d6be136facfa0 in / 
# Tue, 12 Jul 2022 00:43:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:38:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:38:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:39:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8c4856949e70ae5ad889cfc6a747677ca43e6945c3d56e2d4e3ea5e17da91a2`  
		Last Modified: Tue, 12 Jul 2022 00:53:19 GMT  
		Size: 53.3 MB (53268948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85304dce7d82a20f3528edaa2f642b51acaa7ad37bf801bff37fb58285e162d5`  
		Last Modified: Tue, 12 Jul 2022 02:53:35 GMT  
		Size: 5.1 MB (5141175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cbadc5d6341427c002ee8974edf24880be07e7dc4f99c9007435edf337f950`  
		Last Modified: Tue, 12 Jul 2022 02:53:35 GMT  
		Size: 10.8 MB (10765692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd57258941e6f27be345136fea0ab731687b040d44631f55e4efcb475508b078`  
		Last Modified: Tue, 12 Jul 2022 02:53:52 GMT  
		Size: 54.0 MB (54045563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
