## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:79f13435500de5f728b792f10f404fd9037bc8a3b0edc53ae8482f9451c567e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8c5b0be8284f3ffad21b631a565d95b206ad13fd7fab4860bed8ae57dbec5bd3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68083055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa032cdabe4be1922293729cab49304bdbfc5bb0a7ecf88d15b26752bcd58a6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:21 GMT
ADD file:e12306e266f3e237ff7df5ea95bd339c3eb4a539f31be801afd63a76e116f522 in / 
# Wed, 01 Nov 2023 00:21:22 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:55:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:711706b827bb26857b90ceb32b653a05be0e06459342cc05124da0f97f9b6ad9`  
		Last Modified: Wed, 01 Nov 2023 00:26:31 GMT  
		Size: 50.5 MB (50499123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ae13a022e930633aeb58ebf812a0350a4ec43803e013187863d358e62f15f`  
		Last Modified: Wed, 01 Nov 2023 01:04:06 GMT  
		Size: 17.6 MB (17583932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d480bc746f923acad671d7592a0318d59b3d00cff454e730e20b9e915a3e4752
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62180023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eca085d0fa4d2ab3f440a605762d5eab83321b1edfb729fab09fc20f6bdea5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:37 GMT
ADD file:90492dd68d097af40a6208353165e1b7e2bc04a31cd2270232e085416f6e940e in / 
# Wed, 11 Oct 2023 17:42:38 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:48:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ecd2705b9dde659b853da74fbe8d7227d02acd96f1d34766d44193b82468b37`  
		Last Modified: Wed, 11 Oct 2023 17:47:27 GMT  
		Size: 46.0 MB (45966353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548d6bcf8bfe2322ed1ed9f56eeab4afd1b65e4c4a62d0be4d602f14dafc992`  
		Last Modified: Thu, 12 Oct 2023 03:58:22 GMT  
		Size: 16.2 MB (16213670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f93b04aec507910fbaa9a45dcff734fa880323618be3ee146dc70f885a285af1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66742904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c330d4af463f1493cf1f188470d0d1445f9d11bf3ace6545f44b18cf2f1f8d5e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:12 GMT
ADD file:d97d8c89883987c89b2150923abea982086030e71970f5473a534e95252b4972 in / 
# Wed, 11 Oct 2023 18:25:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a7acee270b8289bdc6bb8836f1a4899f794d60337a0cdc46b58a717bd27ba89`  
		Last Modified: Wed, 11 Oct 2023 18:29:25 GMT  
		Size: 49.3 MB (49291086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d43a8471c221305b41e4a48fe1a36d8d976208b182f048b98aa6dc81e6fec8`  
		Last Modified: Wed, 11 Oct 2023 19:55:54 GMT  
		Size: 17.5 MB (17451818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:32c7184a162ee94fdac9984a9cef58f1bcf15f4c0a1acd21082769162bd02990
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69353381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:885698803969612184270761585a946f4b430a1383c328ab4924a3f6c7f6a410`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:14 GMT
ADD file:47cece2eff96bf7383dd2a9c5632f0ad7bb31b3a459677530f77a78e22658e98 in / 
# Wed, 11 Oct 2023 17:41:14 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62bc68699d611f4c048328a0468ebc10de528260c7823c8938796da30db31a17`  
		Last Modified: Wed, 11 Oct 2023 17:46:45 GMT  
		Size: 51.3 MB (51256071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a664405fd519ae385ebac7659c355b2c380dd5c84037f38e6d3673b2bd9795c5`  
		Last Modified: Wed, 11 Oct 2023 18:25:03 GMT  
		Size: 18.1 MB (18097310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
