## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:71ae7bd72882b92017bec9d0bf11a61cc89336357f13c70e262e92a97e63e2e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b089200dd4fa37e64684e79ca80221b5bb431cbbcd8e00a9817b11c34bf0a85f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36382582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7afe1943809a6327bfc7bb2f8f3fad77a8eda9eab4765442fc525ff398a56f21`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:03:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:03:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d3b7a8084f0f50ac1b09fe5b075dd39627cf2d5bf67659da7c41138cda7b67`  
		Last Modified: Tue, 07 Jun 2022 02:23:53 GMT  
		Size: 6.6 MB (6644325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd97ebd2067d1a4bead88f69c0cdcc55b5a30fce0416079338359fc29d2bb4a8`  
		Last Modified: Tue, 07 Jun 2022 02:23:52 GMT  
		Size: 3.0 MB (3026631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:13a3c948a26109df18f18a86b14f1f49893e49b9d7753062b584a75210bd1700
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30598914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:182d2cf4817fd888bcf97a9b9babc1c930f2775bc4e9c0a73b8d54f18fffe3ff`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:25 GMT
ADD file:9604e3641a386ec134596dd717862c2386c1b90009c0646b1773930f98949d9c in / 
# Fri, 29 Apr 2022 22:58:26 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:23:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:24:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:03ca5b55b2bdc3c68d23c18a88c099e2015c6bdcef6e3c43ca0bfb6aea0b032a`  
		Last Modified: Fri, 29 Apr 2022 23:02:31 GMT  
		Size: 22.3 MB (22300451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a73dc6c378126504521857c1f5b32849b1a6f778ad3be2ae05e85a203b1679b`  
		Last Modified: Fri, 29 Apr 2022 23:44:06 GMT  
		Size: 5.7 MB (5713646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882d05cf8d5563b9acf2592cd89c94aa437d95d40a15b9f67c62ac3754b6c395`  
		Last Modified: Fri, 29 Apr 2022 23:44:03 GMT  
		Size: 2.6 MB (2584817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:267d57a221c2d9f61456ecec35b826fd9526dae070dc86ffae9ac090417d7fda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32392322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7a18566ba41cd9003f2d28808aefccea3a4a1f4acdb4c598f9267072c1ec64`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:43:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:43:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89616c81f795aeebdc336526b5d6120f4952baddbda6e27e6d138749bb23cc6`  
		Last Modified: Tue, 07 Jun 2022 04:53:59 GMT  
		Size: 6.1 MB (6083855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459cfb9478ba071444e39cdf4d9428c854e2438ae482b10dbea4dadee121c4b6`  
		Last Modified: Tue, 07 Jun 2022 04:53:59 GMT  
		Size: 2.6 MB (2573803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d3334f09b66385b29fa6f5ff6baea5b22d1d8ea480f186c6ab84cf06f4e1feb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37138698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fdb4d3c6f6197b46f7390f72c57ab28eceda8bedcc61ae24b7738acc7283d8`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 21:18:54 GMT
ADD file:c1118975f50d6835777043d4b807b4fcf30db0151d1e7659e077e9e33c4ea7c7 in / 
# Mon, 06 Jun 2022 21:18:54 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 21:45:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 21:45:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1408ae6e2634d0ef0a2f110363deef0fdf35ee2958852f9d20b92b57495a9fb7`  
		Last Modified: Mon, 06 Jun 2022 21:19:41 GMT  
		Size: 27.2 MB (27165461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9997a51874c52f806343d9609c83d010ef99ca07d34fe33a866c72416728b1`  
		Last Modified: Mon, 06 Jun 2022 21:51:19 GMT  
		Size: 6.9 MB (6931382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5698bd6c395573f235a617e94df59b4d8e7c54b59065059267f6aa81e685a7ea`  
		Last Modified: Mon, 06 Jun 2022 21:51:17 GMT  
		Size: 3.0 MB (3041855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3ffdc86103c5f7d357853f1b756a392f8a0d01bf5ded792cbe71372f181ca2ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41220619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933400d60e83cbd07787a1e3eab767030512699620d52674e5e4186f4910b2c4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:55:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d7ea724107cf3fb9dca027e66737cbba5da37d5b111c18bcbb1bc195ac8a17`  
		Last Modified: Sat, 30 Apr 2022 00:24:56 GMT  
		Size: 7.1 MB (7057904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328e725fac94afb6fc3c04f131827c3480065a1100acf76b2a2fd9c38ec61bba`  
		Last Modified: Sat, 30 Apr 2022 00:24:55 GMT  
		Size: 3.7 MB (3719532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:96a8d71f581221966b1d70fce2371182ba43ccf16fa3bebb6bcc2d4048d0de55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34684928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3dc5c91f70ec7d4d34c11122fedb7d0428de4e4fc679bce2918b8c5153ffa4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:04:44 GMT
ADD file:e2caa30d22701eeadebe1abd66923745f75d170d7baa51a62119576c31b7f89c in / 
# Tue, 07 Jun 2022 04:04:47 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:45:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:45:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:048a87c6fcb9ea8de843bbbe647d14716098af0741f7f59e30c60f39b96b4397`  
		Last Modified: Tue, 07 Jun 2022 04:07:30 GMT  
		Size: 25.4 MB (25370236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeabcd99a1d7b951343f0d1932013865edf701d725a76082d0e91a7cf9bea4f`  
		Last Modified: Tue, 07 Jun 2022 06:06:25 GMT  
		Size: 6.3 MB (6334562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9df68dac810e4f12a4ed62d3aa3fb927a412ad018af6c10348e2f7a7a2e0568`  
		Last Modified: Tue, 07 Jun 2022 06:06:24 GMT  
		Size: 3.0 MB (2980130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
