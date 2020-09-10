## `buildpack-deps:jessie-curl`

```console
$ docker pull buildpack-deps@sha256:82b07989180dbb228a2565777da175d1fb34e23bfbf6534f23c11df0c9b5b85d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:jessie-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b598f7025d3ae3ebd011318a40961717955b38173406bd655566df6f4a77c119
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71935001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a98dbdd3d63fc3e5f2a23c615a575c6d8d33033c07d49cae8d8e03c4dcfe3d51`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:24:00 GMT
ADD file:ca64ef47722e4bf4beeab729a34cd854fe7293a0a2a0a2a92e6f1347c071dfe9 in / 
# Thu, 10 Sep 2020 00:24:01 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:03:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:03:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:290431e500161a90ac38ac8631791acb27e14a913613b60b3df58f839168df40`  
		Last Modified: Thu, 10 Sep 2020 00:34:21 GMT  
		Size: 54.4 MB (54389019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaf1dd00a337044e2c0421947b13d7390883ef55a08ff9ea58d13ce59784328`  
		Last Modified: Thu, 10 Sep 2020 01:16:59 GMT  
		Size: 17.5 MB (17545982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:63d131745d7b939f4e38caf26291c5380ec116443d59fab046772c04b699c123
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69621034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee8d1ead31a436872aaaf20bce51680998f9a49610c4fa2a0412d6583ff581f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:15 GMT
ADD file:b5770ada526014c416df31779f0c640c62a5e53e8e018a6201d507999ac34e18 in / 
# Wed, 09 Sep 2020 23:54:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:37:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:37:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:82ebff95f0e21d655344637482b367c7ea0db41b80cbc667bd980d2141287029`  
		Last Modified: Thu, 10 Sep 2020 00:03:15 GMT  
		Size: 52.6 MB (52583713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f40e46cda9c751ff385c796d48a3c39740220c3885866739fe62640f9437afa`  
		Last Modified: Thu, 10 Sep 2020 00:55:04 GMT  
		Size: 17.0 MB (17037321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0b5e8a6ca97c3aff1fed945511e0691f929fe6b24f4894a744f5cf24e14f2a51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67029209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c69b8ac770fa5d75154c9c19fd5220e1adb0f808963d1ebd2efa4ebcc1b6a032`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:57:16 GMT
ADD file:1b4bf8acda0b906341b6a17ca6eccc23744ba196c78c5bc59c3e26d0b2ebe596 in / 
# Tue, 04 Aug 2020 04:57:18 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:00:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:00:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7c58b357cec76336de1011b56cc2999a53017c6a4b3cf93f2b8362b7a055c544`  
		Last Modified: Tue, 04 Aug 2020 05:05:41 GMT  
		Size: 50.3 MB (50305564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64410aa4323d878bbe3be9802befcd90ffd5681624e0e325a80f25a038fa6cc`  
		Last Modified: Tue, 04 Aug 2020 08:27:38 GMT  
		Size: 16.7 MB (16723645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:16105a16604350bb9c9e6af8794a31002bccb2361948c826312f9ec020f05f9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74465547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3583ac4ed99b91acbedfa812161fd5a17896579ce565ffc63aa49ccb0cf2a36c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:49 GMT
ADD file:85c105a2f2f0c7bff57c73bff9ecdb5ae2cb04074a0129fc1a82d4da85b95ec0 in / 
# Tue, 04 Aug 2020 03:37:49 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:11:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:11:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:49a2d30c774cb18fa05d4cb6f730f97f4965b1162debd13f35bf1733bb737735`  
		Last Modified: Tue, 04 Aug 2020 03:42:50 GMT  
		Size: 54.6 MB (54609569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb76cc7bc12f41ea0e34f0355c0a2d2c5689a14b42947760e1caf7b92ff80dc`  
		Last Modified: Tue, 04 Aug 2020 08:27:50 GMT  
		Size: 19.9 MB (19855978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
