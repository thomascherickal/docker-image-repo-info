## `buildpack-deps:hirsute-scm`

```console
$ docker pull buildpack-deps@sha256:818933a4d4164902f1879fe421851a3b5709ca106f3fe77766c3d911aaf6a33e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:hirsute-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:03c440ab93f47f6f25a8234febc88184480f28020791200b902ad758cc4fc7fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84470558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:823cef2ec1834c9343ac135b8763c224793328b28dd2afae1dad1a2da3016cac`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:55:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f50de6f11a7b6e208c43425014772ef0610d5f771979c6704e166be5c0499`  
		Last Modified: Mon, 26 Jul 2021 22:13:33 GMT  
		Size: 5.4 MB (5431174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bfd280fb76c1b9717ecd762750a8e603d628c6cffebe143f0b34966a47bae5`  
		Last Modified: Mon, 26 Jul 2021 22:13:32 GMT  
		Size: 3.7 MB (3661446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9939f009cb8ebf9ee9b4f6b6f99c0a7ca437c96b046a6345f065cbfcc3dde`  
		Last Modified: Mon, 26 Jul 2021 22:13:53 GMT  
		Size: 43.5 MB (43540366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6fcc5afd47847c2e97114df73dfbdb7cb98b3dba59c9d5e0460f5353e0ab2cd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74810727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12dc9111323484a0279e67f569d4cb21203c02f93aa3dcaa657dcc5ac889e26f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:32 GMT
ADD file:76353e48968f6c84802b150e577cc7fb1bc50985e78e1b499ecd8debfe50d8e5 in / 
# Mon, 26 Jul 2021 22:52:33 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:681a32f1cee4135c0497939e80766271e03a995a197d8293224e8f6bd470bfdd`  
		Last Modified: Mon, 26 Jul 2021 22:57:17 GMT  
		Size: 26.9 MB (26857313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181d081ccdbe67f74ab6dab322dc6e8e84a9b56cb1909518f7d199a8fc8936d`  
		Last Modified: Tue, 27 Jul 2021 01:47:35 GMT  
		Size: 4.9 MB (4858897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb191db7ef79ad38fdcde76e18b9267b765696ecf8c500929ef80b649f800`  
		Last Modified: Tue, 27 Jul 2021 01:47:34 GMT  
		Size: 3.1 MB (3138386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b923df82160d2d4eea0012b206b82fae9ca16efd703aacc1069a7bb396b558`  
		Last Modified: Tue, 27 Jul 2021 01:48:15 GMT  
		Size: 40.0 MB (39956131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:dc39d4d5ad2393f751cf3c63f3554a86fd36ec973743ec05e74c87c96be0f1a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82871381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45b3ee151b13a9ba4dfa1e59a49779f6fd06172ce632529f3c030bc2ebda616`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:49:12 GMT
ADD file:878284607eb47bd96d58adc1bce14366656e20fede92cc0ff58787c14419cffe in / 
# Mon, 26 Jul 2021 21:49:13 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:32:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:32:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e34e08490be30f2dbe7ff29e0668c6e5aeba97f012896805dc1c38253e41bf42`  
		Last Modified: Mon, 26 Jul 2021 21:51:45 GMT  
		Size: 30.3 MB (30299715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f88e5c290191a11d04a6a70e2c9d084f4f65a3b98566dd7aa057aa01e790de`  
		Last Modified: Mon, 26 Jul 2021 22:42:41 GMT  
		Size: 5.4 MB (5402637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e43382b5ae512202c4b72ab829799e18bf61bf87928a28767164981394ea8d`  
		Last Modified: Mon, 26 Jul 2021 22:42:40 GMT  
		Size: 3.6 MB (3637846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d15bb320d287ed358835906f8dfabfecbcf99b47c08f1fafb1b0e95ca69ab20`  
		Last Modified: Mon, 26 Jul 2021 22:43:00 GMT  
		Size: 43.5 MB (43531183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f27c67b36f263760a8087131c54011ace3bd5d7db22c6529665d6abadf899e03
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97492523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8b571049a41e25671a9c46d043cc1d74fe7567e153df521e45039f369392ac`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:18 GMT
ADD file:42c46f2fd1479c7d309139946c738ffe5c5379a9561b96a8d7511bdb0090481e in / 
# Mon, 26 Jul 2021 23:13:21 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:38:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:50f10986101895abb3160c75977e8e8eb7b79e82f78fa9dd1883692b644e4675`  
		Last Modified: Mon, 26 Jul 2021 23:16:36 GMT  
		Size: 37.4 MB (37352998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72f19678043711c11465b507df75ce318af4bd2b392f685ca3841dbba055aa`  
		Last Modified: Tue, 27 Jul 2021 04:26:44 GMT  
		Size: 6.1 MB (6133314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a982650c2954b338afda90c5ba86d7603861d62a22b2e3800362985c59823f`  
		Last Modified: Tue, 27 Jul 2021 04:26:43 GMT  
		Size: 4.5 MB (4523551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4da86ef0de66c418b38e81b81a9690c0e7b660053a2b63e8a7b090c8ffdd23`  
		Last Modified: Tue, 27 Jul 2021 04:27:06 GMT  
		Size: 49.5 MB (49482660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c7feb8b2814ea8ded0a17260a7a7ac99bad50629756985a26a74b390710e1d1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75595229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a0dfbd696fcfe90ca2bb0e5b1f657720ce568c85d30575fb93c6565517296c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:24:43 GMT
ADD file:399cdf15e2e703457111e0585186fa94182dcefce41f795abd41eddd1b10cefd in / 
# Mon, 26 Jul 2021 23:24:44 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:16:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 00:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f03e05f8f3a48ff7994fd656018adf1f6bd707a2827d3bce0fa7435fafe04db`  
		Last Modified: Mon, 26 Jul 2021 23:44:22 GMT  
		Size: 27.1 MB (27140041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b18328c2ee0bb5276608140b8a8467b6a2ee03da83bc425802e0b076060fc29`  
		Last Modified: Tue, 27 Jul 2021 01:10:03 GMT  
		Size: 4.9 MB (4945324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afb0382af3d5aa29a9736f3967604d202347f0fa55cf43d804d2b204bf6d3f1`  
		Last Modified: Tue, 27 Jul 2021 01:09:59 GMT  
		Size: 3.2 MB (3177613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039d531e9f9a40c9a15969b59f3504018fbb8782d1dc9c079e15a99c5f1b4349`  
		Last Modified: Tue, 27 Jul 2021 01:12:00 GMT  
		Size: 40.3 MB (40332251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8b550504b593e6f43513cb1da65be1e53959dcf9f127603cf7fc853d67509645
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.5 MB (92536944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c62138c4f2b680d7189e22fd0153d5482f468287a2480677ece43e8b41cb64`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 20:55:31 GMT
ADD file:bdac50808129a68a89c50670c12a81b904aa091dbd47eddb391da90ab245345d in / 
# Mon, 26 Jul 2021 20:55:33 GMT
CMD ["bash"]
# Sat, 21 Aug 2021 05:06:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 21 Aug 2021 05:06:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 21 Aug 2021 05:07:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0dde1b40c8bf5cce712bb8e104aa59e911b2c25d8aabe5075842cec6026b2bea`  
		Last Modified: Mon, 26 Jul 2021 20:57:32 GMT  
		Size: 32.6 MB (32624229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a38e8077603d246000c3961c0a084deeefa3976054bf5d46eea0cac71bd0fb`  
		Last Modified: Sat, 21 Aug 2021 05:16:35 GMT  
		Size: 5.8 MB (5800724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52a2eee85a32047662a4c1df323e6becd600499def8f3ff6844cfc97a9b99ef`  
		Last Modified: Sat, 21 Aug 2021 05:16:35 GMT  
		Size: 4.2 MB (4185060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5878f655cac880d7c4ee784ca5f06ebd004fe275531df853fb0e9978d81e32d`  
		Last Modified: Sat, 21 Aug 2021 05:16:52 GMT  
		Size: 49.9 MB (49926931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
