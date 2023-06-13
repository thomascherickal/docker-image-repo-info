## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:79076b96c6effc7b05d9c1176fd52717a3280240a1c7fc87b30885ab61bbf22e
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

### `buildpack-deps:bullseye-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:bbef72c2edbf7c2b6eeef7419211baf56bdd84c0be7743f1ae0f6523692c8db8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125400517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13390ea1290540527d56ce52a9164bdfe1fe61076e07392e22408c741e58cffc`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:29:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b4d59f9abaeb4efe1c66ff2176044e93912966342d76d025b6d1a2a37dde7a`  
		Last Modified: Tue, 13 Jun 2023 03:37:49 GMT  
		Size: 54.6 MB (54585023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:69bbed83d531c9774dd7d4508e4217f06d31f7973ac432b52c89fe18b62edbb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120266452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab899ed5a8c735e2aacf3767f6838db12dbfecff4839405286ab629fd58be94`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:38 GMT
ADD file:74586d6297f91fb43eb1f367e32039cdb4f30bb86ee4a094d0cba8e0263b1c16 in / 
# Mon, 12 Jun 2023 23:48:39 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:37:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:38:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d43c9c52ecc2ee6ecfb5eca6f12c77b0c13f02c1f5b0ca4f7af79eec88842db`  
		Last Modified: Mon, 12 Jun 2023 23:51:44 GMT  
		Size: 52.6 MB (52556725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca09034e540486d8a6e04542d506a00bbb3ab568169cc09525837c463ac6aa1e`  
		Last Modified: Tue, 13 Jun 2023 07:43:27 GMT  
		Size: 15.4 MB (15368979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d6aea2749ce0075cc252cfde2fa729cade84531e45abde4cf9056971bc0cb`  
		Last Modified: Tue, 13 Jun 2023 07:43:44 GMT  
		Size: 52.3 MB (52340748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a1298db23708c249e1f7ca5af6824658b1e9fb435787e57b7fa60499173cb7b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115442408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e4dfcff046ab0d545d56e9d9554b1aacec8aa84d0eb2e823c2994efa0e65ca`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:56:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3330bf88d2bbd0baa313813532130c140958ecb30e8bdd1d1a990d63261a23`  
		Last Modified: Tue, 13 Jun 2023 05:03:43 GMT  
		Size: 14.9 MB (14868599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38186e5e226995fff4cc17f64810ad935c484e3a9ac1011f1e1dd7e61981e00`  
		Last Modified: Tue, 13 Jun 2023 05:03:59 GMT  
		Size: 50.4 MB (50355668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:32abd16749a73941e76903142841977d777bd71c9d2568a1904a2cbde6c092dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124126736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:301eb6bbcddb3df0afcb47c6d2f5d3ca6b88bce5f29e4d5a8868f9dabed73cbc`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b90602383b5196ae0f8744277182f671de6f12c55664a9f36b274ab9266b5cc`  
		Last Modified: Tue, 13 Jun 2023 03:08:47 GMT  
		Size: 54.7 MB (54676037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8c0185d0f1eb8490e82a6cc1097758f57659e3e16221fa221f1a97960cc63d6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128226957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f1e4d6f652e5aca88bd06ee95bb1a3712deef2793ff37bdcbcb93b08a6530a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:04:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:05:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f5dde02e53ba41cbb376df97a5a106dcdacfee9b317fa635acdef0e92431e5`  
		Last Modified: Tue, 13 Jun 2023 01:12:41 GMT  
		Size: 16.3 MB (16263400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cdbadabe8bfab344a3144f3f66656501fb58a09d1d76acaba00818ee00d3aa`  
		Last Modified: Tue, 13 Jun 2023 01:13:02 GMT  
		Size: 55.9 MB (55922892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:f6f5e3e579eca9aa2806cccb6c23c6e6c054fe442af0a0087c0b3608b62f636b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122097543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c9abd606ee2eddd8571ebefae145ad7384af3d480ef9923a8e961f7c19b960`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 02:03:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:05:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6f4361e85b8c11a8c3186bfe513ee8546a5cc99eccb71ce813c015f5e68947`  
		Last Modified: Tue, 13 Jun 2023 02:23:10 GMT  
		Size: 15.5 MB (15520467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a53d5ea647b7d4fae45a1983ebd3031500dd7cfc8a2583d62638696890be25`  
		Last Modified: Tue, 13 Jun 2023 02:23:53 GMT  
		Size: 53.3 MB (53306666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9ab3b81b39dcc38d79775993d18edc4d26c1b74f0f694e0740d3a8e3397c2305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134545082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:941da36723e2fd8a00908f0e7440a8b3c24749c2644905af0122eb7e08c80299`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:54 GMT
ADD file:93fa83ca9c503a09001edab8e277ae6c67636f805f8bb49986e0ed2ad3ea8360 in / 
# Mon, 12 Jun 2023 23:17:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:31:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:31:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ebc829b9a845100e0e82d2b659a5cd374121460e523a23fa55a97ac0ddb14460`  
		Last Modified: Mon, 12 Jun 2023 23:24:35 GMT  
		Size: 58.9 MB (58927438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8f667b037b5784a622608738c6e09331fb14a8ec7467cc7e6fc14a97eea39f`  
		Last Modified: Tue, 13 Jun 2023 07:41:24 GMT  
		Size: 16.8 MB (16752805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9456eeaeb4ea7025dcd6aad36f876b89639f902465aea48d2e0028442e7e7304`  
		Last Modified: Tue, 13 Jun 2023 07:41:48 GMT  
		Size: 58.9 MB (58864839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4a12a68b9fcafa310ff42142914104596fc7e4ab42a1cd9e4ac5cefb0f69f0f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122976169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1434d82e03c16d5032f23dd1e6200b30e7b8818060dfbd28ada9b56602e659ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:42:35 GMT
ADD file:a054112be60c3f2d7811b27cde82bccfd1c2747f29b7611ee68b21cd9f3d3d54 in / 
# Tue, 23 May 2023 00:42:41 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:33:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44d1d02f91725dd9ae742f7c70add814dc3da3fde438adb01e65e1f8b0eba613`  
		Last Modified: Tue, 23 May 2023 00:45:33 GMT  
		Size: 53.3 MB (53282114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4000487deec97f7a3856b8eeb8f2984dff7a59cabf8346950db508cca6afadb`  
		Last Modified: Tue, 23 May 2023 02:38:46 GMT  
		Size: 15.6 MB (15631909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c736ce76be1a25bf3c5524841625878f78ec8b4739bb2156e0bb9052207e94`  
		Last Modified: Tue, 23 May 2023 02:38:59 GMT  
		Size: 54.1 MB (54062146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
