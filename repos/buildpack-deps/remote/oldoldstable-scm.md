## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:947936c3aadbe5c308e3499292a4a2bedcc6a04f4bcd7ebc840bccbd39e40f43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d4168f65895fa9813c42d789ed449e8f2b9e3f41e5ebca8ba683edc433e5049a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115267951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00dc15ece40d3e671d9429048e1d326401fcb99fd411dd43670dc37be0006d6e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:21:06 GMT
ADD file:2ff99c4b1a4acaafb9f4705b01b8d997c1af388f3732ed81d317a1c52f4ec30e in / 
# Sat, 01 Feb 2020 17:21:07 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:26:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:26:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 00:28:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be2ea31e65ce4ed34b999c4be891da1ed0e4c259d9ccdebc7e0ac094771f30af`  
		Last Modified: Sat, 01 Feb 2020 17:26:36 GMT  
		Size: 54.4 MB (54389437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cae66b02b08f93ce3e7805bc52085a3a041a2ce382ab23586991947b05b4e6`  
		Last Modified: Sun, 02 Feb 2020 00:40:03 GMT  
		Size: 17.5 MB (17545770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b354be6fe0058d0e101c2850b2a9735e2317de1479af6c713070e1128eacbae`  
		Last Modified: Sun, 02 Feb 2020 00:40:18 GMT  
		Size: 43.3 MB (43332744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:60e3f18b07971c3c37e4220e25cd55e46860c1620c8b787d87664f9e7110b254
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110775824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e5a990c92a9e2b30c364f341083faf49d30ca801fbb865c2f9d849c0799763c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:54 GMT
ADD file:32b8a625927c1f5bf5f1b4ba44bb1c2af32e6dbd8f0a379d6a0a7612aacb9939 in / 
# Sat, 01 Feb 2020 16:50:55 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:31:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7911b8b96f54b072a80e08f30051237d4db6aa19229c178eadfcb7a0448a1504`  
		Last Modified: Sat, 01 Feb 2020 16:57:29 GMT  
		Size: 52.6 MB (52579602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4464e1d3f05f646bcc989c3bd8bbf247c2c65c1787f9b741b44e7b0eee15a2e`  
		Last Modified: Sat, 01 Feb 2020 17:46:53 GMT  
		Size: 17.0 MB (17036474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef78e4bce8c7efa5e0a384621cdd3c8a3825ee1d9a1d174fbcff03687dcd56a`  
		Last Modified: Sat, 01 Feb 2020 17:47:13 GMT  
		Size: 41.2 MB (41159748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:697246e8e5c46604e74879475a920d7a4c50dc6e26a3b2f7780df0b4f865d196
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106802034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287f8b70517ea6088ccab4f5db094c7a3633919753f810ce797fbb85f72207c7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:48 GMT
ADD file:bab8bee7939784a1d5baca51f04a76319f9f7b86f0bf7c14a50d562afb38d34e in / 
# Sat, 01 Feb 2020 17:00:51 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:08:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:08:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:10:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381ca3674bdab054305b554fde6fea73521f10f49d1e5e4aa83e7b87a6f65006`  
		Last Modified: Sat, 01 Feb 2020 17:08:09 GMT  
		Size: 50.3 MB (50303070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb354be3b609b8df1ed44520b7c8f5163810b20a9dd2674898e0ef63bc8f3b`  
		Last Modified: Sat, 01 Feb 2020 18:28:28 GMT  
		Size: 16.7 MB (16722874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250584ac835ade07ea0bf9cb419d5c9cfe6d41ca5f33bee2de202c8bc23d5829`  
		Last Modified: Sat, 01 Feb 2020 18:28:48 GMT  
		Size: 39.8 MB (39776090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:fa35eda655d911cef95b6d5199129b7ccc52f2d3c92997bf3896a797c38030cb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118439447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4a1eabcb1258eea7553cd08d4229f8563b5a8de9f64ad5caf56c381c59c7f9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:48 GMT
ADD file:23c9537c86963e84613c942db01132e5d06384a5fd0b9f92595ecd7aeff0935d in / 
# Sat, 01 Feb 2020 16:39:48 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:29:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:29:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:32:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:605158be38a8eaa27411bc385ed7dcdc4884e9ad8da221b2c160b4dc702fd008`  
		Last Modified: Sat, 01 Feb 2020 16:44:50 GMT  
		Size: 54.6 MB (54607256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ddb6eab72836c2f7baabe2d7cc8baedb1fd4b769a0b80c9bafac7bd2504cb0`  
		Last Modified: Sat, 01 Feb 2020 17:43:34 GMT  
		Size: 19.9 MB (19855762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297985b73d122356ed17677fc8b290e4f7868384fae0b731bb529cb8791165f4`  
		Last Modified: Sat, 01 Feb 2020 17:43:49 GMT  
		Size: 44.0 MB (43976429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
