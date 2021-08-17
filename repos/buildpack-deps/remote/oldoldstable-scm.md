## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:c9bf609e41c82d55e9a85dc5bbaed9b7b45e6eacee023cad169a51fd35cda51d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e82d3fb40c016ddf0c394ded0bc55b2a87cf768b4a3f17b97cd962bf21287fff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110778470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14048e14a2a169d16f541d3d3df1a66cbcbc8aa17c67ae637eecb2dc2c057dcd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:05 GMT
ADD file:fc9409352ad67880b83ccf1ccd1587eb2666715eae04e4dd98fca919f1bb98d7 in / 
# Thu, 22 Jul 2021 00:47:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:15:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:15:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08224db8ce18b31a78a0a26d1b344d173528e50a7067797c9df4de5d8df353e2`  
		Last Modified: Thu, 22 Jul 2021 00:52:52 GMT  
		Size: 45.4 MB (45379781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd3caf86f5b9d8f8e63437571297df5fa6d454140b9c1985c47d6ad526da824`  
		Last Modified: Thu, 22 Jul 2021 01:22:23 GMT  
		Size: 11.3 MB (11294469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c316554a558d4aa95c0be17c01e4a0366d6026a98eeba53dca5baa6091e815`  
		Last Modified: Thu, 22 Jul 2021 01:22:23 GMT  
		Size: 4.3 MB (4342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721081de66bfc648ce19234c6333d6e031344f6ac90904476c9ec2dba2917e3a`  
		Last Modified: Thu, 22 Jul 2021 01:22:42 GMT  
		Size: 49.8 MB (49761833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2cac3b81fd9ab4f32e8d6c8448eee1e97a29bdf284c6dba3de5579f3962eb5b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106586591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7f196cf418b3a4cf09d01fee87d8745b9f90bf88002ad05ae9c84b66288fec6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:53:04 GMT
ADD file:bfe848278f8374ee4e7de4946371b7176fc2bbcf40afce8ee1f9738af7b06694 in / 
# Thu, 22 Jul 2021 00:53:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:11:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 02:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 02:12:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:984fc5232b7d0db08285a008f512c6a5de7610d4f37c8c97ecd7b1bb98e2dd65`  
		Last Modified: Thu, 22 Jul 2021 01:06:29 GMT  
		Size: 44.1 MB (44091732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9d89827417cfad915b22c846cd8371b341fcf557926f53731aa581557fd3b5`  
		Last Modified: Thu, 22 Jul 2021 02:27:28 GMT  
		Size: 10.4 MB (10350527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21206c9923e5c0ba9febe6fb63521144127d2dc085d2cbd0398dc9a317d2ed30`  
		Last Modified: Thu, 22 Jul 2021 02:27:25 GMT  
		Size: 4.2 MB (4161456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96a7b2ec5cfac7d80ff670a6435fd33f97173decd0d57cb8b76b3729bd85d72`  
		Last Modified: Thu, 22 Jul 2021 02:28:16 GMT  
		Size: 48.0 MB (47982876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ad644d96ced7329a4fbbdc06340c75993b803a4b0cf007e08531c13da72fe634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102118086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913ecee7c9dab2b07b5a7ed95c8d649996bc97a468d1dd89872fdd682edf7bac`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:06:56 GMT
ADD file:544c40297b94c3ecc6561cf7bfef1cdf9763a18ce5e24b6841a1b70d0516d41d in / 
# Thu, 22 Jul 2021 02:06:57 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:21:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:22:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b3cc5e47308fe8ded537d7ffdcaba46fcdf803cfe9878bd9264754a50eaa128b`  
		Last Modified: Thu, 22 Jul 2021 02:20:37 GMT  
		Size: 42.1 MB (42120108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf69efd3b547fe4dc472fd34a54c466b82ce51b7f04957779206b5ea0ef9160`  
		Last Modified: Thu, 22 Jul 2021 04:41:23 GMT  
		Size: 10.0 MB (9950872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7430ae4c6b93ca669cc72566a38f952b74dece32c5897c46e51a5907bd5a0c`  
		Last Modified: Thu, 22 Jul 2021 04:41:20 GMT  
		Size: 3.9 MB (3921255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5849792410ce49abbe1ff9b523687c9a52997076c1137a38ade9efa2c1e2a2`  
		Last Modified: Thu, 22 Jul 2021 04:42:08 GMT  
		Size: 46.1 MB (46125851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4efb8da6c37091d4348878bf934cfa4c3fbcdb2910e7f6263e3b30ad685a6b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105227352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44b4c6f44634bfe5ec3f5fe9c1eb38ec5cf857eeff43382b6f99722bf7433948`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:26 GMT
ADD file:fab290162e6d28cbe115c866c49a1e09d955450dc9e831ccbeefe40e18cfa3a7 in / 
# Thu, 22 Jul 2021 00:41:27 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:18:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28ed64be8f9ee39d8ded09482441a288852dd40c2e535b64e1f9c0271c10eb44`  
		Last Modified: Thu, 22 Jul 2021 00:48:16 GMT  
		Size: 43.2 MB (43178440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6227db87dba6bebff5c1f1a2bd2d290c25c44c23f3b974a4e99fe72b48777812`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 10.2 MB (10214761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cffb4d8549ecf5dfe60357ee2dc98dd618c73220f26c8cd505b088085229668`  
		Last Modified: Thu, 22 Jul 2021 01:27:40 GMT  
		Size: 4.1 MB (4096559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1e9f731097d2238f7fc909257c62c337b7052f2689c55215fd3cdc233510c7`  
		Last Modified: Thu, 22 Jul 2021 01:28:01 GMT  
		Size: 47.7 MB (47737592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a118e684aa2e428350e3fae74c09246820e7a5d41a92d1679f1f4139a06b633a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113280493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e61a364c0adae3b9b246c7e2afa1f6b0145b2424dc75da8e16f94a3701c7e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:43:45 GMT
ADD file:e05a48da77b08cb5622f87152f4378e29fbb9bc65a76c762d45e488e30adb647 in / 
# Tue, 17 Aug 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:04:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fd774782ceed955e627fdc8415668afabdebb5525036f0dc871ec023eb317787`  
		Last Modified: Tue, 17 Aug 2021 01:54:38 GMT  
		Size: 46.1 MB (46097220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aca3d286261da95e058ae37c67e002a572b7dfc1dd7fe13d83060357489bfb`  
		Last Modified: Tue, 17 Aug 2021 02:13:06 GMT  
		Size: 11.4 MB (11353003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d22bbd8aeb7ef47c0fb18407f27411bd8008e1189b79f7c7c3dd1a6adfb7`  
		Last Modified: Tue, 17 Aug 2021 02:13:04 GMT  
		Size: 4.6 MB (4565010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f484f8f178f4bf3f3ec40912975a9e55159419f752b4683fcf11d9317be62c1e`  
		Last Modified: Tue, 17 Aug 2021 02:13:36 GMT  
		Size: 51.3 MB (51265260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
