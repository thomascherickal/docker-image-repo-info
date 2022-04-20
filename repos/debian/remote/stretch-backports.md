## `debian:stretch-backports`

```console
$ docker pull debian@sha256:6157d662f4a08f5b92802ea97957bb9360954f190e1c1d03d134e32e4f499321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:a0415b442feac68daa84c8593f6b8cde23d8ecade4ef46ccc8a3786a12cf8b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45427658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33386c6b36009d7d27bfe0879f50041853630fd16c3f454848232b8ae31eed03`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:14 GMT
ADD file:6ed691b65385dede44a92f9de9e1428af431197c66461aa0f9c61e2f7c8bade5 in / 
# Wed, 20 Apr 2022 04:45:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:45:18 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f5196cdf25181bc7e4411865a2e002932b7b6b0ffce787c04c1bdeaf1f204f20`  
		Last Modified: Wed, 20 Apr 2022 04:52:01 GMT  
		Size: 45.4 MB (45427434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2394e6d00af092ff7367c7fb33292903653e6cf6aabe32479e312a38bb0cb5b`  
		Last Modified: Wed, 20 Apr 2022 04:52:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:37a8411b446d12d110918e96391ed07b36aabf0edec7bb132ea9d77ad181a2bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44122895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a67b0b313d69591facedfcacb81e41c77531f53965b82e865f19f66001e835`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:22:06 GMT
ADD file:407e28120c3ae0a1012433a9787cf812e0ecc360e63ace9fe21f6728470b4db1 in / 
# Wed, 20 Apr 2022 07:22:07 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:22:21 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c6849d3c2fa1fe7c2c78db1c26ca92e44c119dd3e92d93450115c927ecb6dce6`  
		Last Modified: Wed, 20 Apr 2022 07:39:41 GMT  
		Size: 44.1 MB (44122673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98248ff0db11472ad62001823042f2e1f5bdeac0e6a484c74ce326e5ecc0eaba`  
		Last Modified: Wed, 20 Apr 2022 07:39:59 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b381ccc9cd3b0a12e13a95c0930e9185b9a0e3138bb8c85c75711a7f70dd9bfb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42151379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:013e9658675a4d7dfcebd7098f9c22921e461692fcd1277f5daeba8c284765bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:23:57 GMT
ADD file:3dc1697adfcf63a288e9ec7a2c40438b8ba2ccfff0382a1ed5457f30d7a37f76 in / 
# Tue, 29 Mar 2022 02:23:57 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:24:12 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:aecfa9e0b0179abf68bebbcfc35453928546e01ad1c8b6eaadf759360762dada`  
		Last Modified: Tue, 29 Mar 2022 02:40:33 GMT  
		Size: 42.2 MB (42151158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb87be6f1130e26d8508411eaac526000f4d19c1c67d19f897a41728962eba6c`  
		Last Modified: Tue, 29 Mar 2022 02:40:52 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:69b33411284e960871a5c65303ac7002e770fd086c9d102c39b0759509cc5c74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43212238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3af33a0b58fbfa12ec25670dea899cd58d4023aceb7c58b142ae38b7f2612bb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:19 GMT
ADD file:73f1db8536438ca891f4b507a569e6c561364db0f05914ebea9d3fa97e1bf837 in / 
# Wed, 20 Apr 2022 04:31:20 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:31:26 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a41fbedfa4b1547a2b4fea33de48af745d66a94741d3cf344cb2766f0e80211b`  
		Last Modified: Wed, 20 Apr 2022 04:39:38 GMT  
		Size: 43.2 MB (43212018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b96a53eb3beb1d44463d8aff37df806ccd9366541010ca13c54f965cf0267e3`  
		Last Modified: Wed, 20 Apr 2022 04:39:55 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:8e4e2bfd809ff66a5d33f6a8f356c4889968e30ee4f0f52a5029b62060db9945
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46147950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f444c2a94f9431981aee1e2ed6b26aa68aed33aaa74258ea84a735bf6905799b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:39:57 GMT
ADD file:e8c6a60834ed931ccc3c93b1f2c9b9ca2bf190b0d8d2474382ee8e96a7e35b5a in / 
# Wed, 20 Apr 2022 07:39:57 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:40:04 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cd343d4c0c2fbc67ddea33155621bdf36074fc30ffb6f917e716fbb81645f79a`  
		Last Modified: Wed, 20 Apr 2022 07:48:48 GMT  
		Size: 46.1 MB (46147730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4a0a39c21cf6cf5a561cede12d53c959a96644267af6576c061c575c761786`  
		Last Modified: Wed, 20 Apr 2022 07:49:05 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
