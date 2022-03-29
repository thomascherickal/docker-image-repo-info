## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:999bb7a4bf64a185b22a386c09e06d8cb59690ecee182a4319843ed2e400ace8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:163d5a64fa7c0c51860eb64d0cca9189c0b4c55220889ee65ce7cd857f0b1635
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61073462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae58812f064e987538314d076b3bccfd243eb7f9f8142ee47fced60ae3085f5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b009ccae6a1d207b657810ecf1852a8962af32ebbeb5d308d1256b48784f7ddc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58637908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1ee243651e0aa937ff30d183fd7ca898e1cf74100f94c9fda241b2ed9037ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:55:32 GMT
ADD file:4e79cc43996ddc8062073aea4d6352c3ca3c736e9b09f1eb440f913d5a52469d in / 
# Tue, 29 Mar 2022 00:55:33 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:56:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:56:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a58c023b263eaa1973763831b149ed127bbe67ee8cae67d60e261db1e9d54b63`  
		Last Modified: Tue, 29 Mar 2022 01:12:11 GMT  
		Size: 44.1 MB (44123307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c0117421f3f6b9a01b30e38d3562bc7a42dc789c5af5f80877e67cd59edcb5`  
		Last Modified: Tue, 29 Mar 2022 08:14:25 GMT  
		Size: 10.4 MB (10352487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c612024a40834a1cb0833f65b0e86ed44bcd14476cd83a108eca13607211c477`  
		Last Modified: Tue, 29 Mar 2022 08:14:21 GMT  
		Size: 4.2 MB (4162114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1a5d79b51ea47b0e80de853251d0d2b86ce2da11fe12a262f42884c5dbac2d28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56029996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c9ac325c2a3334a7574bd9e39cb0850a25fe61ac42b0754cd691f35222950f7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 09:36:25 GMT
ADD file:e869f7223f16639eccabff7b2c6a85a7e6b075d0933c31f2fecae79c1c26d5be in / 
# Thu, 17 Mar 2022 09:36:26 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a9f775cd9058b832779f6c0dd1ca0fbb1417961dd87ca3ba6200f41aa283371b`  
		Last Modified: Thu, 17 Mar 2022 09:53:00 GMT  
		Size: 42.2 MB (42151366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c76f62b4a80636807fcffcd72fa68808c0faab499371e9e49ea3805cb8de8`  
		Last Modified: Sat, 19 Mar 2022 03:37:42 GMT  
		Size: 10.0 MB (9956816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe67020a39019149bd81805e6b89528643f4464d33964fe8bd1c39ed3c68dfd`  
		Last Modified: Sat, 19 Mar 2022 03:37:39 GMT  
		Size: 3.9 MB (3921814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5cc0481a1d70bdedc0c10e80f7dd37b558d8efb3e88ddce3539b14af4e7246db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57305214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26769edb2bf581cf2034eda01009578d213071340c2b4c2332f983f9789c162a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0d6ecff05d590b97ebc357d19bd439c17d4142359ceceb25dda468284e978583`  
		Last Modified: Thu, 17 Mar 2022 03:32:27 GMT  
		Size: 43.2 MB (43213043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf8187d7f23f7722584cf9a7359b8e6859ca891c112d0398819cecdac7fa008`  
		Last Modified: Thu, 17 Mar 2022 22:24:30 GMT  
		Size: 10.2 MB (10217652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9ad8247187d77aea7d1a40486c48551a68a63e2b6be93a43c47cc27d726beb`  
		Last Modified: Thu, 17 Mar 2022 22:24:29 GMT  
		Size: 3.9 MB (3874519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a64369081dfe289e1a44f7696b642e5cd7c29904918880522e4afed06bc6e6ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62073605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9151c83ca390f7f1b97833bc1d8c665a6358c18b5cfacc224f694a9b522b9fb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 08:18:34 GMT
ADD file:60679f2ddce5e36577f1a8d320d5221029cdbdf145c7043ae099312d74451d17 in / 
# Thu, 17 Mar 2022 08:18:34 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 14:32:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 14:32:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e21a7d1d60294e341bf8cde8b67cd64035b84fd968946be519fd79ec45925ece`  
		Last Modified: Thu, 17 Mar 2022 08:28:24 GMT  
		Size: 46.1 MB (46147889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b8c8176f5881909d36b8bc4d5ddfa2a2b80e8161e45e01b75b1d367bf2bb8d`  
		Last Modified: Fri, 18 Mar 2022 14:48:17 GMT  
		Size: 11.4 MB (11360144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaf0a804dd2d29797cd2ba58b689e56b24ae765d0e8a4369f839bd12b7dbde5`  
		Last Modified: Fri, 18 Mar 2022 14:48:16 GMT  
		Size: 4.6 MB (4565572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
