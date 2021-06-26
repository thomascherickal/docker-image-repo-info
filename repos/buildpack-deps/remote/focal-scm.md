## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:ab061f99ca713bde9ec4124c53a9a7972a6a42b715997685aeb7154f15c8a1af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:37806232d5eb3338f99e530e4d140e38e06276f746139e390dd9fbf272cd50ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100648590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9708f9987c805379caf5652993156d653b13ed71f397966ce7bffced355145`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:51:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:51:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Jun 2021 00:52:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b912d13b862fd5a362840f26d0ad46f398a249f785bd94ecee18e553d2db10e`  
		Last Modified: Fri, 18 Jun 2021 01:07:50 GMT  
		Size: 7.8 MB (7769437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1834cfc49396132940874c10eb85a40884eec9a4c5b70d635b4a2ad437b57ccd`  
		Last Modified: Fri, 18 Jun 2021 01:07:49 GMT  
		Size: 3.6 MB (3624091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa102afcd5efba79a11d11a564b216881e2d0767ea910ce562efdc07c8e0bbad`  
		Last Modified: Fri, 18 Jun 2021 01:08:12 GMT  
		Size: 60.7 MB (60701370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dcc1deccbd7961dc635cee69f4e075b06b9485298c0a4e8cfffe7770a9b92a2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89556409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5485a7fd87c69e1234e8f8f0dbd5486e820eb956cdb25284dc5e24ec267f5bb6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:00:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:00:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 06:01:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b011bc4cd9cc61587fd89efa70cfd1536e16dde9a8a5dc740579ca82f9b5243`  
		Last Modified: Wed, 23 Jun 2021 06:30:26 GMT  
		Size: 6.8 MB (6766701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80661bd8f69548c62e7f12dbed47226be394b312a65e3d68db3227e896ab4ed7`  
		Last Modified: Wed, 23 Jun 2021 06:30:23 GMT  
		Size: 3.1 MB (3103880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d397a8f6ce52369de82a7b212b004dd53d0fd34358e13a9cc84f84d004e243b`  
		Last Modified: Wed, 23 Jun 2021 06:31:22 GMT  
		Size: 55.6 MB (55634086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:73be83f86ba2a4f2558b2adf145e13563a7242ed5f48081acf4af5572be5a069
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99135704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a20646e315f53f4c346676f7f9fa3318f84b13d213ecb4f62de2d150bbf143`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:15:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:16:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Jun 2021 00:16:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f991cc7d8086f742770bc68ea3d374ffb47c85c4a65288e00f75f51cd144031a`  
		Last Modified: Fri, 18 Jun 2021 00:23:57 GMT  
		Size: 7.6 MB (7634452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfceea9d1b75f3829e4442176bacb2670946d8ed4a0655dc24ae5ed1b938183`  
		Last Modified: Fri, 18 Jun 2021 00:23:56 GMT  
		Size: 3.6 MB (3600413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9b4c2f36cbd2c56995ffec8a7928cb08eb5674e63009e2082bf4434bc0d59`  
		Last Modified: Fri, 18 Jun 2021 00:24:20 GMT  
		Size: 60.7 MB (60742036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2e25e3bf9ae397639b7dec4c428ced33a4717da1ca74e6475118b50198a70288
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115839673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff49a51c00e9662fb8773737214b8669e51ab7ec9d3704082e46651b1f453626`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:17:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:19:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Jun 2021 00:21:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5ad3c9db7d785b733500d4105691410c88da518424a8e6b4778668a6958210`  
		Last Modified: Fri, 18 Jun 2021 01:21:46 GMT  
		Size: 8.7 MB (8721563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83725bea45164975cc2629f6a50653e36e72dee8f75ff38b10ad250887532e96`  
		Last Modified: Fri, 18 Jun 2021 01:21:37 GMT  
		Size: 4.5 MB (4456587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ffee0601a514903e8848335d9322aab58db8b162aa4dc56f38a7b820473d9c`  
		Last Modified: Fri, 18 Jun 2021 01:23:06 GMT  
		Size: 69.4 MB (69383278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2073949fc3f0634c1f7e25a9e146e3ff74ae522e78165e66734f4fc937034348
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.3 MB (98324181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31279ebbc0777d70ae8ca211fa2084a69057ccb78fdd10179fdc8f0ca172440c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:44:00 GMT
ADD file:737a08bab262cc2abc326912fdb8c8038222b272a5967b25ec6c761539c9d456 in / 
# Thu, 17 Jun 2021 23:44:02 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 21:32:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 21:32:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 21:33:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be436b7e641e3737311249dadcc71ad61ba7bc9597248f426c58c8548cff8af0`  
		Last Modified: Thu, 17 Jun 2021 23:45:32 GMT  
		Size: 27.1 MB (27140902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c37ce82d11b2e609fa6749e9ead72662c47e8511d7f872de7c66e80cdab2d3e`  
		Last Modified: Fri, 25 Jun 2021 21:43:35 GMT  
		Size: 7.4 MB (7429023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebd75052f63261612beab488d84627a01f33f49d7713e08fba04b0bb361931f`  
		Last Modified: Fri, 25 Jun 2021 21:43:34 GMT  
		Size: 3.5 MB (3542094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5d9a133b3c4e4bf8c0fa19fea19af398c7f51776d490836768427153e1a949`  
		Last Modified: Fri, 25 Jun 2021 21:43:52 GMT  
		Size: 60.2 MB (60212162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
