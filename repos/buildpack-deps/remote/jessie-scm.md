## `buildpack-deps:jessie-scm`

```console
$ docker pull buildpack-deps@sha256:6b48f31c5ff12addb004054fa6fcc1b7f7960b952ec0e05896f857d563873589
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:jessie-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:759adfdcb1751f26029bf6ca4f46a74b0a956c5dd94044c8ec12a790225467d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115267566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1449565446805a3c2c2f942bfc63961db576c879ffc12e1ba0a5a5da8b887393`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:57 GMT
ADD file:607350db53d30cfbdaaa75b7a47bd59de2bfa83fe4a50be9e7cccddcbfa7c61a in / 
# Wed, 26 Feb 2020 00:37:58 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:09:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:09:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:12:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:92d14a6520e1a734155afb0c5b456614718259f56397290ed22fab220c2b96f4`  
		Last Modified: Wed, 26 Feb 2020 00:44:41 GMT  
		Size: 54.4 MB (54388885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953765cae32285a96cb8dfceb67d75359de4ed5b8c5ca50bcd1aeeaf19acb19e`  
		Last Modified: Wed, 26 Feb 2020 01:21:34 GMT  
		Size: 17.5 MB (17545643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e6b16cfb54d978d891e093f8e8ac63974b286241077fbc2788d0798be6b9f0`  
		Last Modified: Wed, 26 Feb 2020 01:21:50 GMT  
		Size: 43.3 MB (43333038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f166b1eabf8b766932c6c284dbbab2e03aeb4e3493c90eecb963eba0e1e4b771
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110775747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0677629aff0689f7b8de6956046980ce220b43c6ee685c6c42292be7c6943649`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:48:18 GMT
ADD file:dfeb6a347568f49dda331c0a3507c2f67adbd728b7d05bb73981892d7e1a602c in / 
# Wed, 26 Feb 2020 00:48:20 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:42:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:42:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 03:44:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ecda12258fd08534cd1becb346cca0f577a29d87b9a0e10f9506312ca70a556`  
		Last Modified: Wed, 26 Feb 2020 00:59:47 GMT  
		Size: 52.6 MB (52579149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347038a62fb32cd535e9daedd7ec90325fb85dfe551edeffed203385b1fc4a58`  
		Last Modified: Wed, 26 Feb 2020 04:02:38 GMT  
		Size: 17.0 MB (17036652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9a36680cec80c39312e70464848dba16bd184e4d413a2439d6c54bb9f4c355`  
		Last Modified: Wed, 26 Feb 2020 04:03:06 GMT  
		Size: 41.2 MB (41159946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:53c1e278975c57852a1c16b8cd1e437cfd7935b10053c943e4fc2bae8b57bec1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106801497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:862ee7d6e6a6f0ced10fe2254acacb55741fdddc612f9e1efef3f28d5284f2ff`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:39 GMT
ADD file:a467dd7304add7a1979638d51c2e28f9355aedccfd4727532a90b0db7fb1d9d6 in / 
# Wed, 26 Feb 2020 00:52:45 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:16:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:16:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 02:18:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10fa2b45efadcc8561689d641256044af7890a575a625a567d96dfbbac1c5d05`  
		Last Modified: Wed, 26 Feb 2020 01:07:57 GMT  
		Size: 50.3 MB (50302762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc01a96123ffaa0c4c0e711f6d51ee89062e113913ee9965abdd34e60170cc3`  
		Last Modified: Wed, 26 Feb 2020 02:35:03 GMT  
		Size: 16.7 MB (16722914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c627136ee3d7a33f5e4b63afd27dbb92239f6a01ab462de1efd491552191ee2`  
		Last Modified: Wed, 26 Feb 2020 02:35:22 GMT  
		Size: 39.8 MB (39775821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:776359156a5fd6280f3f5caff8f2b95f6429b9e5ece9d5bfd4a65ef07feb090e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118439204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d3cdc61a3dc263fdc7df5f27ef6c2a35ae0644f9d41d9fca4e338258227dc73`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:34 GMT
ADD file:55edca1096804fbcbd260441dec447b0ee75e01826e82a48d2f4743c90ee01be in / 
# Wed, 26 Feb 2020 00:32:35 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:12:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:16:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1fe0a93005696879fec845d0ec4f9bfaf8c2e5d43a8bf4dbb1aa7bb31ef50aea`  
		Last Modified: Wed, 26 Feb 2020 00:38:54 GMT  
		Size: 54.6 MB (54607169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127f47054d5ddf851c1c3cbe9918f68fd635af42568819db800aed86dd229c0`  
		Last Modified: Wed, 26 Feb 2020 01:28:46 GMT  
		Size: 19.9 MB (19855832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bc41ac0634e633f90a357022254157a91569283f6a6bd11c7879b957cea087`  
		Last Modified: Wed, 26 Feb 2020 01:29:05 GMT  
		Size: 44.0 MB (43976203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
