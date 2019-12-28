## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:c2dd0b5a45a0f508cb5903cad298167b9f9ccd795ca8afea49f07e984795f7a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a0fda67f80cb1e5d8d1cf5d332333bedd93fcf88aca088206fc6093dcb0aa987
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69461094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4c4dc28e989164cd78109a93eaa7b29e91e386c73864a809029f17e629e2942`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:3f67740cbc1b7fefda4dc75bd2c0f0e76df9ae6b845f37b33cf8eea958403b6c in / 
# Sat, 28 Dec 2019 04:20:39 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:45:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:45:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3f64e5c246a10532414f3b69dcf620cbf27337d8900089f4139ab3215186e02f`  
		Last Modified: Sat, 28 Dec 2019 04:25:14 GMT  
		Size: 51.4 MB (51358861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a40087c7676442e3d13e8a213aa17fb44a1cbab4d952197f09edac463f58edf`  
		Last Modified: Sat, 28 Dec 2019 05:00:44 GMT  
		Size: 7.9 MB (7919349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce8ee259aabe18e11221885897dc3fc3f8081c56a276bef858633277e6384ce`  
		Last Modified: Sat, 28 Dec 2019 05:00:44 GMT  
		Size: 10.2 MB (10182884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:0c322fdf59c92f1beab0a721977cee47da93d7f6d6f0b2e42e054babd2803c53
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66654815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d79fa9a8a3723c70dc0cdf3e087fea946454d5476e230185aa25ee72d78ebd8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 12:12:27 GMT
ADD file:2baa1f0574c2834ad17d2f76e28f77e533c06686ddf3e7cd093dcb4c72ae9942 in / 
# Fri, 22 Nov 2019 12:12:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 17:17:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 17:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5c41680389ba4d76f3e046357090c3c237888674b176f2ed957bbb159706f221`  
		Last Modified: Fri, 22 Nov 2019 12:21:10 GMT  
		Size: 49.3 MB (49268003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc981530e6b8edef7874ba6212f5b9cce279a30e51b2c53295a4e4d2571adb1`  
		Last Modified: Fri, 22 Nov 2019 17:44:40 GMT  
		Size: 7.5 MB (7509588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3cb96c42f91b6aa679e1b44ac84fbecb2cd38d5efc5a37efe1ccd33f65c7cd`  
		Last Modified: Fri, 22 Nov 2019 17:44:40 GMT  
		Size: 9.9 MB (9877224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a06d54a2eba914a5aac47e6422f9d71b14c99ded692b4f0021db8ea32a5618da
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63782495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fd37a85faadf606bbff1b9b07046ec0cd6a2a6317e72cff768ed25cc7d16c86`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:21:14 GMT
ADD file:c9fbe61f7ded389c614d7a2dc7a73db387e5c89419aab9b0acdf46d39fb6cb04 in / 
# Fri, 22 Nov 2019 13:21:15 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:05:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:05:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7829ca4b083805aed02c7dff13add2b8d98f2f2acc202324179e6b3fd2e8e8b7`  
		Last Modified: Fri, 22 Nov 2019 13:32:22 GMT  
		Size: 47.0 MB (47004823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa54e745c00d42991e0ffcf809df32fdde29efb873febfbb04d106b5f13c385`  
		Last Modified: Fri, 22 Nov 2019 23:29:08 GMT  
		Size: 7.2 MB (7248647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73cb25af478f5d8f5f1eb45a63aa43bb357348836787fe1383a004dbaf87a28`  
		Last Modified: Fri, 22 Nov 2019 23:29:08 GMT  
		Size: 9.5 MB (9529025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:df0cdb56da6e68b409e00a4ea50daed77391b35f851ffd679d8b1fc844b76506
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68258901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd4c50bf9de5877e3d16a8ef400a537d78f75e9cc4528b29a5d44f75fb85b6a3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:40:29 GMT
ADD file:9facbcd1b6cfe39d1286c4322f52b4a0fffc19c418e69808a91a18d24389ceb4 in / 
# Fri, 22 Nov 2019 13:40:34 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:08:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:08:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c9323f8b378204c8971fa964b7dea92c5c3506d0fc91bcaed5414c36962d408a`  
		Last Modified: Fri, 22 Nov 2019 13:48:52 GMT  
		Size: 50.3 MB (50254093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79451582277fef4301136fd87a74ac924308c99b67753cd6c706bcd80c4d6345`  
		Last Modified: Fri, 22 Nov 2019 20:26:20 GMT  
		Size: 7.8 MB (7814071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c280be30668695ab64918c37e490a5e9c8f57f6e700f9dd71a928bcbe0397ee`  
		Last Modified: Fri, 22 Nov 2019 20:26:20 GMT  
		Size: 10.2 MB (10190737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:653b729b75d10ae904611a93e8057ff9c402f40b7d08928d22d10f0fd8b6863a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71105852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f30a330b5abc783d01a5807ebffb0548463186f5abde7f68e8531b9033c007`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:38:52 GMT
ADD file:de81f6da93dbb580dd4c6a23ebd6cef637ab58e6f566e5ff7a217d4def3ed529 in / 
# Sat, 28 Dec 2019 04:38:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:18:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e3ee43b8971d572beb3640b791c4bba0d66137db2252115ebd9b2bb3ab7704d1`  
		Last Modified: Sat, 28 Dec 2019 04:43:38 GMT  
		Size: 52.5 MB (52480376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372a64d1cd36c22d0befce3fc6f8cba8fa5023d7bd33fc658de98186e128919f`  
		Last Modified: Sat, 28 Dec 2019 05:41:00 GMT  
		Size: 8.1 MB (8091626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac8412cc2ead4ec139c961dbfca9f633b422edecc1798b4b7057866f1cac71`  
		Last Modified: Sat, 28 Dec 2019 05:41:00 GMT  
		Size: 10.5 MB (10533850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8a44339ba9d1fcc8d73384a5ce8895145f2be8d2837a443d6974d5fefb1a785b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74436002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3135fff24fceb7868e65f135407338012fe50f43f54443a7765f853385340ecc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:53:47 GMT
ADD file:b12b950fad43a45b27069cc60b807b788017c0b7afbda941432314ed9baedce9 in / 
# Fri, 22 Nov 2019 14:53:51 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:49:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d9030213e9ca0dda517374420b70437d57b213737e4313d3d3b7da588c75a611`  
		Last Modified: Fri, 22 Nov 2019 15:02:18 GMT  
		Size: 55.1 MB (55119200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16d2f968598a1b0dd8a6598974e5227877e498cc41ef594f8083c7abdf1a4ce`  
		Last Modified: Sat, 23 Nov 2019 00:24:36 GMT  
		Size: 8.4 MB (8369585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ba3989924e2be4d02a61b9b821e3f11edd034ec4268e32478ae75a2ee96016`  
		Last Modified: Sat, 23 Nov 2019 00:24:37 GMT  
		Size: 10.9 MB (10947217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:63997583a8b3cb77712af27cb2e68f8c6800b25127e097cf7354a054f4516114
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67616146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab3b80c85518c808b3cba8243463549053d729f239023eff6454511af1882b4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 10:39:53 GMT
ADD file:dfdf0ec49bef8a55fa525692bafadf9503d769f6fe23f0ccdd904236be48169f in / 
# Fri, 22 Nov 2019 10:39:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 11:24:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 11:24:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5236d095abf6f42c79c788819ad11be11514c8a8774db88619e96d7f50894887`  
		Last Modified: Fri, 22 Nov 2019 10:43:47 GMT  
		Size: 49.9 MB (49940120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de0148a2b53b8c484e691bc4e736d5e54e5a5226d9a2584acfdde9b61f5ad94`  
		Last Modified: Fri, 22 Nov 2019 11:35:52 GMT  
		Size: 7.6 MB (7607980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f5e6e78499e671d55a0eea16bedc319ce1a849b8bb130123ea84e3a36200c`  
		Last Modified: Fri, 22 Nov 2019 11:35:52 GMT  
		Size: 10.1 MB (10068046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
