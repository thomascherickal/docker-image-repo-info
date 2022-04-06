## `buildpack-deps:impish-curl`

```console
$ docker pull buildpack-deps@sha256:87bbaf8c98d641c5f50e9791680e133e8c2715294a2545b66c300fe92b3ab7d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:17be20a074873fadb85645576d0a18a25904c18cc7c2821d638166cb981487fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37630868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db52c51f2bdc78eb4dc21a0e6a652b1bc41e5005cd95a2949aa36a97d62e7cfd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:58 GMT
ADD file:eec4cf20bda495a93a4e4c816abd77f5a14cb3fd6ebf56e6b8d7c9f37651edc6 in / 
# Tue, 05 Apr 2022 22:20:59 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 22:47:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:47:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:34031c10e7d284f922b3f277e18997db8f3250fd9777be60a86b59e25b2bb155`  
		Last Modified: Tue, 05 Apr 2022 13:19:26 GMT  
		Size: 30.4 MB (30386032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b620199073d87654cb09ef591c8be4e7778d489c08d0f2d33d1e6ca0da3052b`  
		Last Modified: Tue, 05 Apr 2022 22:59:03 GMT  
		Size: 3.7 MB (3692650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5bf4be237bfb6e07b3c2d8940770141c9cc787c140d50f46e9e4badf20a206`  
		Last Modified: Tue, 05 Apr 2022 22:59:03 GMT  
		Size: 3.6 MB (3552186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:74428f0da6a20608c4de92337443ab9d4149ab13dd75f8ca23b62ea20c48bccc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34107193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55a32f7fa1f109e0f95c15c4b924b5c7941dbae5cb7633e8358b79367f364c4c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:33:05 GMT
ADD file:380138b8388e9dab10885559d020801299e8a053731bc61eeac23044d83317c6 in / 
# Fri, 18 Mar 2022 07:33:06 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:14:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fbf944519806fa77357b54f48091ca8c7ccaea62ebbb79761a15cc513dbcb20f`  
		Last Modified: Fri, 18 Mar 2022 07:36:56 GMT  
		Size: 26.9 MB (26921466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10b93b08ad29a35f3e5c193f2bfe6b9f9e7d502ebd11b72f4aa644268f77f99`  
		Last Modified: Sat, 19 Mar 2022 03:45:36 GMT  
		Size: 3.4 MB (3443108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e15c098c0600535f00359aaa245c8a9bbe723d52157f0a5df1dbe5fcba6d6b`  
		Last Modified: Sat, 19 Mar 2022 03:45:35 GMT  
		Size: 3.7 MB (3742619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f68fa5cf42cc1b1ab5355b09bc115dbcccc31240a0a93533d8d3a1c04a638883
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36036357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc4da7f712edb214c7b39facf98279e7f5064df276637881296126350a5bc61`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:09 GMT
ADD file:6291956a2e3fe9eea698936c2110257f655f85ef5fde2a71623e0625141cef5f in / 
# Tue, 05 Apr 2022 22:41:10 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:08:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:09:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f91b2ec0e6ea0b2df920d20005a7fd4f57f359296c67e8f7dc8210a85a5a5b41`  
		Last Modified: Tue, 05 Apr 2022 13:20:30 GMT  
		Size: 29.0 MB (29031824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2e6701d71f01758a7fe34633a9bebcc4523c8af74e634139d1dae91ada413b`  
		Last Modified: Tue, 05 Apr 2022 23:16:51 GMT  
		Size: 3.7 MB (3676915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb277949f9898a4ae702c5215a79664e8d0f8874d2fc0a578acacd75f3dfcb1f`  
		Last Modified: Tue, 05 Apr 2022 23:16:50 GMT  
		Size: 3.3 MB (3327618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c95f6d06af1dd8b9d057cacd45accf79715542f6367942d6cc5d7cfca6f361e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44565261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6edc711ba8db82bf322d73559972b0b536fc0189919e85cc9da9eaf75ba638d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:59 GMT
ADD file:12ad43f11dfcb52c536f049db16e0355dd0eb94d8fa80bc5b0cd7cee083bd07f in / 
# Wed, 06 Apr 2022 03:36:03 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:36:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:36:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d7170978615332f0cc77a33a016a1fe353d81871a63f50b984b0dac7a1fcabd0`  
		Last Modified: Tue, 05 Apr 2022 13:21:57 GMT  
		Size: 36.2 MB (36176423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a001bd2aababd21010b68132cf219c881a583ea786aae051c1d24233dbff6f`  
		Last Modified: Wed, 06 Apr 2022 04:51:16 GMT  
		Size: 4.1 MB (4146450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e952ac3aad57a80fbcf05e6e6e9a441633123d2befa88f8ed59cb111ddd87518`  
		Last Modified: Wed, 06 Apr 2022 04:51:16 GMT  
		Size: 4.2 MB (4242388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:fbbcdd4bc0b5a82bf7a1178ae2d35e7726fa65a1081e32e00ebe190d116d2d3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34510074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3678ed14dc056c834bf4fbe9b5c715a21c0eb85b2b58bcf4f00c750860ecdd2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 23:16:31 GMT
ADD file:68ec34fd3adbb39c77004745e0c6c740c02017efc5274ed14a79e417c54c00bc in / 
# Tue, 05 Apr 2022 23:16:33 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:09:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:10:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:141a3fe0a236e81d09c7406bb701e9ffa4cd6df5c814a6c137c9071355c53920`  
		Last Modified: Tue, 05 Apr 2022 13:22:31 GMT  
		Size: 27.2 MB (27215296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee819ad05fd79c3b98a1361272f08ada186ca41388b51cd377c360a59de8f26`  
		Last Modified: Wed, 06 Apr 2022 00:51:05 GMT  
		Size: 3.5 MB (3490448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f43a55d5058967c982b5d0ce14e52b6789ac432bab595cf90d32c7973f78dbc`  
		Last Modified: Wed, 06 Apr 2022 00:51:04 GMT  
		Size: 3.8 MB (3804330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9b88009fefb6efe6f2b1bddc2f8081f83841c04555fcc1ca6bfa4ca7039baa94
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38250011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86201030b31947f3dc826e1df294ae795e1f96fc597f3c899c1409095b36c81f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:42:16 GMT
ADD file:93fccbbeddbddb4c4631654eb89c174aa404957f9ba48e6eb738d040c2124b71 in / 
# Tue, 05 Apr 2022 22:42:17 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:21:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:71116f092cb4d97e181bbee9672334a28730486450b1c615aa5b7956b5a32eec`  
		Last Modified: Tue, 05 Apr 2022 13:23:06 GMT  
		Size: 30.5 MB (30524447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc484e5cf466200eaf92e0a58b88b7b5d7be1d3b5dfb8e8bd029fa6c63aff9c`  
		Last Modified: Tue, 05 Apr 2022 23:28:26 GMT  
		Size: 3.8 MB (3762182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977057d0394b24c9cc6fc05ee89b59244dec00dac84caaa805e6b74c158899c3`  
		Last Modified: Tue, 05 Apr 2022 23:28:26 GMT  
		Size: 4.0 MB (3963382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
