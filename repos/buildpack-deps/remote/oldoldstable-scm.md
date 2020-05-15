## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:079f10944e48706aa11385b2b149f565c1fe6a2544ede43d5e4f24426fc9edda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7c8af508daf8a2dd0d119a771e83d34a8a74e7d8e52a4ad418c595117f663e50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115272718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c433b506e5ee0b8cb77000d5955267a4d03d516158636262b0f10465077f312e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:29:14 GMT
ADD file:e2991f3845275348c69ea6ada5b84ab1607a345d096ad349fccd010c365a4ebe in / 
# Fri, 15 May 2020 06:29:14 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:35:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:37:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34656812d18fa35ccd0e5b0a4b845092186ee2084e4890153e6a4b84c9efce5f`  
		Last Modified: Fri, 15 May 2020 06:37:58 GMT  
		Size: 54.4 MB (54391709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1e5b56f90876f03875a4e57016b42f26a64621a0e9bd68a87d75fd23c172af`  
		Last Modified: Fri, 15 May 2020 17:52:05 GMT  
		Size: 17.5 MB (17545861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a4abc0a58c1148900b72170eaa36d1001b1152826cd3ada2e2938fd227327b`  
		Last Modified: Fri, 15 May 2020 17:52:19 GMT  
		Size: 43.3 MB (43335148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:11ad853c1a3252899edbe37b895204e92aef86f5b965ea61c126e8563be6561f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110775825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b57c5cf974f4c743ef6a73bbd4bd5b24e2f5ef88bff23d5d4305d4344a103773`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:38:25 GMT
ADD file:63b1bfb335518fc40ecfe92c179a8d32d00b3dee86ccf70751c74ed2ca14cd28 in / 
# Thu, 14 May 2020 22:38:30 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:47:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:47:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 03:48:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ef4eb1ad38349445de10c8a3682121a581770f589f1a35b7cb327b49bb1797d`  
		Last Modified: Thu, 14 May 2020 22:47:16 GMT  
		Size: 52.6 MB (52582082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f3d44466578cfe6461e4b482b19224356c7b6537b39780b2e75a727ff8ed7`  
		Last Modified: Fri, 15 May 2020 04:03:29 GMT  
		Size: 17.0 MB (17037233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90476d81b98379937371481027b6bee589dad9dbda48c9b553b41f039ff3dc2b`  
		Last Modified: Fri, 15 May 2020 04:03:50 GMT  
		Size: 41.2 MB (41156510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3b34d04e44f4ef7eaf84b19b521fc6136a94a3744ac8327a7c900907f6b16c00
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106807024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a08fc5145aa3ffa8023a6771abd57889351fb7436c89c44d70d990c3f7f43c2e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:00:40 GMT
ADD file:a56bb3e7bad583ad3aa641fc5aa4f91db9848e13388179a63b14ab0aa7fe06dc in / 
# Fri, 15 May 2020 01:00:50 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:38:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:38:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 10:41:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2cbbcc58403b5ede472aaa750e8ded783a6a7d6c87b217ae8713700515dfd33`  
		Last Modified: Fri, 15 May 2020 01:11:43 GMT  
		Size: 50.3 MB (50304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f880f61061969936f29c8cc4a0b12ac569f2e4d7946b61d7f077d65f13e5c4`  
		Last Modified: Fri, 15 May 2020 10:58:53 GMT  
		Size: 16.7 MB (16723381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6e728b8f32c320336b080a08a6d8fa094c7bf4064a84ebaf331da1fcad49e6`  
		Last Modified: Fri, 15 May 2020 10:59:15 GMT  
		Size: 39.8 MB (39778662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d2041f2c85c5a0fcfa9ea5eceb4e09873e718b391e4d532a0d9866a814a63d29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118455821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:936b4f5f4d87ba952ea295b79dc902d8453f8297a8108aecc58a1d53d91df66f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 07:08:25 GMT
ADD file:4f7aa7ecb1a9f0f641f4c7dfe0e5360a0705c5e0eb159391b79bec0e4442bc34 in / 
# Fri, 15 May 2020 07:08:26 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:11:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:11:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:15:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6277e17fa0a21fe6d4617d7259f00c2649972514e9940fbd56cb6d7b75e60de5`  
		Last Modified: Fri, 15 May 2020 07:18:45 GMT  
		Size: 54.6 MB (54608707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5e945f79d261702a2e4dcb64d114abca64e1b6503a3b336cc15a1c68960260`  
		Last Modified: Fri, 15 May 2020 17:27:52 GMT  
		Size: 19.9 MB (19855851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aa3afebb13160d1fffafda1bc7af540c974a11c0cbc7377a05755342a11ea`  
		Last Modified: Fri, 15 May 2020 17:28:11 GMT  
		Size: 44.0 MB (43991263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
