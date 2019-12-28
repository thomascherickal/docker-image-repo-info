## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:43304393830a303ba918dc6903c508a7018c9f4bbf0da2e19f9170f8d8ce5479
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:79d7e913123ad5a395da423bb96db30af6211601608c7fca47c7baa04cd2a51f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124324923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ff35416fba9abaac38d418d80736ccf0beef7e0e2908b67f19ccca01192207`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:22:47 GMT
ADD file:68b1541306250f957e5f1035d80f5683c1ed22e73cf2f2b563adc52424897a09 in / 
# Sat, 28 Dec 2019 04:22:47 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:56:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:57:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:57:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d0b468739e287d7cd8fa8bcb34afb10216f12567d28caab345db8873c4246896`  
		Last Modified: Sat, 28 Dec 2019 04:27:19 GMT  
		Size: 51.5 MB (51479608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44261d6f427d89f764fcd9898d2845c7327812575dcc485436bb888b2ee1d0c7`  
		Last Modified: Sat, 28 Dec 2019 05:03:30 GMT  
		Size: 7.9 MB (7919965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd42132ce8afeea96ec992f4170f1b4fe9fa1a621a93dc2d236088351e29685`  
		Last Modified: Sat, 28 Dec 2019 05:03:30 GMT  
		Size: 10.2 MB (10183322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c16ba6f425320c83bd55536bb502f6e0b7064468bed05a5dcdbf0a13e9d892`  
		Last Modified: Sat, 28 Dec 2019 05:03:45 GMT  
		Size: 54.7 MB (54742028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:5e1258e630726d7da863a25e8201d68507cad0fa32cff3f367cb91a8d520011b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119199851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14aeef1fd4d7691f5059526ca0225861d9687cf3d9fdec0639ea3c7998ac69ad`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:51:51 GMT
ADD file:03cc60d1d72b99d3b1d122da1d59f729e29848dbbf6dd18cbf657a4c38ef0b5f in / 
# Sat, 28 Dec 2019 04:51:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:38:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:38:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:39:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:58904a701fa9ff155e476053cdd7da105682fd34a283dfecfc029765d82bc148`  
		Last Modified: Sat, 28 Dec 2019 04:58:52 GMT  
		Size: 49.5 MB (49475991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8962cbd68da3db27dc20b92f9e448d10c3a6823e53156f2ba301e54789b010`  
		Last Modified: Sat, 28 Dec 2019 05:53:19 GMT  
		Size: 7.5 MB (7494157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f950a4075ac360274a49d98d4a4c73c351f221ac1f7acf157df1e1b62627fe`  
		Last Modified: Sat, 28 Dec 2019 05:53:20 GMT  
		Size: 9.9 MB (9877715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af595a9e5bd9d6de775039fb231e4cee16d03103b4186f91823002517a8cb892`  
		Last Modified: Sat, 28 Dec 2019 05:53:44 GMT  
		Size: 52.4 MB (52351988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e76a14265a08d3d51d0dc90f57fb7047899a3428aa5cba5e7eb800ffecee1f5c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.8 MB (113836067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:366757aa258c6b337accfff04e4c599bdbdaf13798e7c54024deb105274ad2ca`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:25:58 GMT
ADD file:4bf78bfddc69aff1005ff137dbb0900252b387eb72db243381eb8668106c1077 in / 
# Fri, 22 Nov 2019 13:26:01 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:20:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:21:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 23:21:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c9c2507cf34749b60069708965e9265b59dd74f435cb2b28decd5de28599b56f`  
		Last Modified: Fri, 22 Nov 2019 13:35:33 GMT  
		Size: 47.0 MB (47015849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34350c66ee177149a27a048e3caa4842198b97aa0e1f9f6483fe2ef9e259552`  
		Last Modified: Fri, 22 Nov 2019 23:32:58 GMT  
		Size: 7.2 MB (7248590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d535b9755a2a00130e735f6a7f54f88eb70ef58fea1a968c07e85d2e8ad5d9`  
		Last Modified: Fri, 22 Nov 2019 23:32:58 GMT  
		Size: 9.5 MB (9528991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745e2b2c61356760b5ed9e63b9fc4e7e7788e612e5c71f914ab8f18798dfb815`  
		Last Modified: Fri, 22 Nov 2019 23:33:19 GMT  
		Size: 50.0 MB (50042637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d894fb43bcf46b49f2fd7dfc754263398e3e5169400cc01b72f7235895a8f589
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123357052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab5c5fc77af96e35aede0332902b3b434d214be52050b2a65b0ed94707ea8f2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:8932c68f3cf662412b086b3ca8b215a092fa5ea459074d42d359a9c778563152 in / 
# Sat, 28 Dec 2019 04:42:05 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:10:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:10:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:11:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:898762c0a5be611b2ded7eb33fffee89def5fd9c6161871b3f1f06e970b7739e`  
		Last Modified: Sat, 28 Dec 2019 04:47:51 GMT  
		Size: 50.4 MB (50431115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d2023cefe917f460362808fc93a5f289f46561002704988023a04abcb63d8e`  
		Last Modified: Sat, 28 Dec 2019 06:22:45 GMT  
		Size: 7.8 MB (7795190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e6a5a666546a2fdc4d7d715747caa149ef9d403b43a49fea4ac6d10751a0ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:45 GMT  
		Size: 10.2 MB (10192064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f57c50a4b46a7b065b414b42e8f96aeab062a797c90cd356311ed7956b2aad9`  
		Last Modified: Sat, 28 Dec 2019 06:23:10 GMT  
		Size: 54.9 MB (54938683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e70fbadb313164e5dd5241062bd0a47d1e7890156999b85edcb881b62dedb941
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127789810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc7c0649b8691f45ebc1d2e8e4c8b02a895d7041995453323a0df522199237b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:02 GMT
ADD file:028a6b956388b2cf033fb64213fca841fe5708f01d7143a9883bb44273bfb987 in / 
# Sat, 28 Dec 2019 04:41:02 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:35:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:36:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b389037d8e8619e17e0b7de53ac2f84439d0b5b064350f604942c26d3b2f2608`  
		Last Modified: Sat, 28 Dec 2019 04:46:15 GMT  
		Size: 52.6 MB (52610734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9b069a84283b0c0d2f882f9d796b59f53ba2902179668ce465cd0e263633c8`  
		Last Modified: Sat, 28 Dec 2019 05:45:43 GMT  
		Size: 8.1 MB (8094045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474cbca8bafdcb28b1de38a11db97451990b86d610422bd137c2e7b61a86c3db`  
		Last Modified: Sat, 28 Dec 2019 05:45:43 GMT  
		Size: 10.5 MB (10534541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30619627ec66811f54c8f4675cbf7937aeec0c8ced378e14c6824f56ab9cb4d`  
		Last Modified: Sat, 28 Dec 2019 05:46:06 GMT  
		Size: 56.6 MB (56550490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a2cc70e8ec8a479bf335462c2286c8f73bfbdc85ad34555413751d80e5603cf0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134232829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b527db59c9cfda671a42aeeec6e9af6cbfa31437d86143dbba410a76ae914f5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:56:54 GMT
ADD file:475e71c3a164eb255fb6da7547b751028a4a08eaa818ce600be26796ce6a652f in / 
# Fri, 22 Nov 2019 14:56:59 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:10:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:10:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:11:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:95d4ac228743e0506244aa5f8d355cb2bc1d8a9cf78064e10f0834e57973f958`  
		Last Modified: Fri, 22 Nov 2019 15:05:47 GMT  
		Size: 55.1 MB (55128387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1076f157a1dfaaf03cf22fcf170b981f0baa9bd1b88a2940cc94cd75913fad`  
		Last Modified: Sat, 23 Nov 2019 00:29:47 GMT  
		Size: 8.4 MB (8369514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a82ff61e3e3971488bf6dbeff1c0e4fd4be4b9d8b53dea708a21627054e68e2`  
		Last Modified: Sat, 23 Nov 2019 00:29:45 GMT  
		Size: 10.9 MB (10947147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c011a8f45a37d9c5b87246672ad518d2dedca9f0af260309e7c428684e99eabb`  
		Last Modified: Sat, 23 Nov 2019 00:30:38 GMT  
		Size: 59.8 MB (59787781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:39cb10631e1868c25c56cd9722ecfa6cc30b305739f7d25649754d5a2580fcec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121778415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59f36874eb9b666eea6d246b673a952ec0cb2ad57ffaa2eee91aa1aa7a347d9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:32 GMT
ADD file:ebe1df568622bb8e8e8e3b2318d11550389d84f3196d3ade9aaa9ecfdecd1028 in / 
# Sat, 28 Dec 2019 04:42:32 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:47:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:47:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:48:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7d0208a582df93acf7a81d059abd969865a1e647765a53c87e2123fb6b283a34`  
		Last Modified: Sat, 28 Dec 2019 04:45:42 GMT  
		Size: 50.1 MB (50131585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46a42bc5c7805eb22e48c27565c0a108b60dd3c74386aea7cb2a2b367d00d07`  
		Last Modified: Sat, 28 Dec 2019 05:54:12 GMT  
		Size: 7.6 MB (7591630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c311db77933f5cbc7d2dc6e649e1d95c34ce4c806932601722b88f9b28a61`  
		Last Modified: Sat, 28 Dec 2019 05:54:12 GMT  
		Size: 10.1 MB (10069342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc903c6290ae481b2ee639d7b0ce90ef144f5db8cf1c9f396e521df9b32214c8`  
		Last Modified: Sat, 28 Dec 2019 05:54:25 GMT  
		Size: 54.0 MB (53985858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
