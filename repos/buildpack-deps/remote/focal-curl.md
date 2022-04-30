## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:c47f243c7797820f7d3ecbab47c2cdfd773bac70335fcdef2b327c62b468742c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:focal-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0a5777d8a12a1445c5e5e822c7b29ca21b429f959156970b567dc6cd9ef4bb24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39958548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:808114ce39c2c8ac4fcf5c18bfd1cd0e8cf5902309833788c976f173eb883422`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:47:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:47:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b802a9f71706fa309700ea1fd5d986b885729b323ffdb716d290a98e6dfe0706`  
		Last Modified: Sat, 30 Apr 2022 00:01:21 GMT  
		Size: 7.8 MB (7768179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da477514e5fd4aae7503079d6eec1a60d6210d0717abfae57581636ebf69b690`  
		Last Modified: Sat, 30 Apr 2022 00:01:20 GMT  
		Size: 3.6 MB (3624139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5db0458077d942d6744e9319bc57db365a93b36f1483364a288241f9a68ade1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33940311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71f38f1e458dbc3104109b48488ba6c34f46b7d98c6dd010a7843b326d754d96`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:46 GMT
ADD file:5f12bea85a1ebe365907ca3979b0e31e6043dccfcb9a3cdf62be46e054494147 in / 
# Fri, 29 Apr 2022 22:58:47 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:27:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b20724a4297c7ca8b89f31d6ad53e7ead0c17c7908a4592871cdc97332193580`  
		Last Modified: Fri, 29 Apr 2022 23:03:00 GMT  
		Size: 24.1 MB (24073650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1563a0a8b5e832769a2de291e460a7fcacd9bee37ad7a2d8a73b14a0f0ddfc`  
		Last Modified: Fri, 29 Apr 2022 23:46:30 GMT  
		Size: 6.8 MB (6762469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493cef317c1c6766357569ceb016cc5074fdef707c8caf5a67a543cd3f49f167`  
		Last Modified: Fri, 29 Apr 2022 23:46:27 GMT  
		Size: 3.1 MB (3104192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1f49dd9ae94ac486a8203db83c52bad708d0f165baeb56c686dbda7a25be2620
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38189936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6623beec524176ef0a47bb171506df574dc78a496c3840ab19ddbc3645668ead`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:16:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:16:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7feebf8b53c2ab8397b63406bbd6ed34bc670367c3fa74c734bf99c6a2e8ec4`  
		Last Modified: Fri, 29 Apr 2022 23:24:40 GMT  
		Size: 7.6 MB (7634266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8adbae9f42bff04c79875d37944fa1587613ef0de5f7bca85a0b429d4e8d83b`  
		Last Modified: Fri, 29 Apr 2022 23:24:39 GMT  
		Size: 3.4 MB (3386282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c4a9fd84c7d7f84ad035dc0255f5f890d9542c87bd34b7ae17c2911f7b763b35
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46469737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eca98c067e9b8a4d597136373ba3bef2c6b8729a41d9682c6b07988eae73d548`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52152a0de6e46d74b97d1c4aa354df39f45b928545e3b3cfd5562aec916b61a2`  
		Last Modified: Sat, 30 Apr 2022 00:26:15 GMT  
		Size: 8.7 MB (8722859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7e0fa1464e2cd697c14ed00b03cfae9577e44abba441afa9930519b611d1da`  
		Last Modified: Sat, 30 Apr 2022 00:26:13 GMT  
		Size: 4.5 MB (4456217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:a43ec5f996c7e29e29c75540536ca85979b2faf8753309526455dea85a6f05a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34119248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e7d69c312775ffea2cb6067f252234386d1cab720e6e6d0e4b89fd73444380`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:14:50 GMT
ADD file:77e925ea3ddf0d01534094175d808508c4a5d0535f08d304994323efb0173a57 in / 
# Fri, 29 Apr 2022 23:14:52 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:38:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:39:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:63ac7876cbf81a317a4c88c281171f026148a0f62b17284f294a5f0eb06bb383`  
		Last Modified: Fri, 29 Apr 2022 23:36:48 GMT  
		Size: 24.2 MB (24228241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cab7346bd3d7a7b57c31d0f11c693b748d4d32b35b93f23e8d2ca324147bd7a`  
		Last Modified: Sat, 30 Apr 2022 02:34:00 GMT  
		Size: 6.7 MB (6746379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057a89ffe69f2775876926468cca360577ba7f32d63c5b7094142bc3ae9981d6`  
		Last Modified: Sat, 30 Apr 2022 02:33:55 GMT  
		Size: 3.1 MB (3144628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0fefd9a3f6d8215ddbbbfabcc5caf09ef516a36a0c0b92cfd7188ae4f84e5f57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38030581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c34b0ab29c98acd68a5ebd28f7db655ba5f3eec3bc0cd4c361df1e7a4263ef8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:11:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad05d33c3457ff71f921fd9c69734064bb89a93c55c748e7c2b83b0aa4b6237`  
		Last Modified: Fri, 29 Apr 2022 23:19:20 GMT  
		Size: 7.4 MB (7422981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa203495428900214c5ff3ea85c5b6134947347f9c1dfda07e1576ab83bf1f9`  
		Last Modified: Fri, 29 Apr 2022 23:19:19 GMT  
		Size: 3.5 MB (3542183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
