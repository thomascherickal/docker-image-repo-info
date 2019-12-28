## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:30a7efd40c673eaa290b2204d8334c9ecfbd4f340266a2363fe29a0a950ff182
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

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6a072ed2846ff5274fcecf3dc370292376fa984090b4a0006ddc4bf96e44dd86
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69582895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e0416cab1b5d1a8103f74fbd2c7e7011132810d438bca9ecf6f0b9e26c5474`
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

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d28739f5005c3fbff72dea17bfaee8dd0ebda10ab7646964c1122c513cfc89d2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66847863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665aece8839d5ca6cb66867e56490c9abefe85748d63d6faeabcda81b228bd99`
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

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:22a1419ac94470e16b696c9007a573abda9a1702af4d0689bea23e9c16116438
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63793430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1184b9c324272b5b3be87b407ea7171820982cd6d2cd250defb4af78bce40c8`
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

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:10118445dbd6c85946ec7f6f815bad1544b45781461a852fe35c7515a07b434a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68418369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a7edb0fbc307a673c71b55bc8a476c24b313ff7c64b39f9a61576f3aefcf883`
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

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6745c5a387d0b5a03d1f4a5f4bbc86897dc8e54bdf3cf6507b2f9de714d129e1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71239320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18d53532fda86e1939497571097057ac2b01f5aa03979f9a51c0e7fc324f00c3`
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

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:84eea55895084a6ac7fa533855c8e3bd908fa9cb85533bffcf77fc2a73e328bd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74445048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a72848fbb2fe01f0c7ea2c3520e0813df43403916f47cfd99fffab2b544193de`
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

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2b3b032bc4de8c276b6ab2a224c871c9c71acfedee8973697c1e98b63ebdd275
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67792557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab69d514bea7130b515830fde78c847335d5be99cd8f7f194760fb47ecad57c8`
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
