## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:5cbb8f7177833bc49ee4dc9cbd84473e9bc9af5c52f482c0522af6d9bd33da7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a070a43acb36c23e98f8cc8bca3dac0be379b24661c532e7abdd1b2dfd2d6623
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70987350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea63c37fd38e827975db0dc1be530873b1f0a362e223b431faeac8359f51121`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:28:02 GMT
ADD file:d09d72986a18210fc325abfbe18d3d35fef6de8ede47304410bea7528e5ab5e6 in / 
# Thu, 10 Sep 2020 00:28:02 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:08:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:09:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5da2bf34dd483faff62b98f29a31447619812af8afb0cdee07c188e866571393`  
		Last Modified: Thu, 10 Sep 2020 00:35:58 GMT  
		Size: 52.5 MB (52488092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c931b35f2563d7d9db709f3ab5b56a2f0281308f452acc51620919959073a9e4`  
		Last Modified: Thu, 10 Sep 2020 01:17:58 GMT  
		Size: 7.9 MB (7870622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8964fa9112bd6ffcd1be08e066d6e3aade5cbc082a4e29ed533274a85381328`  
		Last Modified: Thu, 10 Sep 2020 01:17:58 GMT  
		Size: 10.6 MB (10628636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e3d07a72e4792491c62861bb9dd9e8339add3dd18b66e629fc61a1de81882095
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68172741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396ce5ff78c8cd15014a1ad400a7da8057b58776111835ea56473054e629f364`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:56:41 GMT
ADD file:9c8616d4fabe6861a7f03ec7c1849957393374004adaf865fad27fc7e91057dc in / 
# Wed, 09 Sep 2020 23:56:44 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:42:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:43:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dd8dd816178223393e19e5b2cd1f62df2d94bc6d5c9c393d8da9f901c96e3f93`  
		Last Modified: Thu, 10 Sep 2020 00:05:28 GMT  
		Size: 50.4 MB (50413542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2d13ac158f55a44a68ac2d72292b51ad657a5202b688ec68c8cf3d7b42c7d1`  
		Last Modified: Thu, 10 Sep 2020 00:56:35 GMT  
		Size: 7.4 MB (7444216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c022e48ce06ce9a71076c5494577357f81ef67fdb3da661d48226f9f774c37d`  
		Last Modified: Thu, 10 Sep 2020 00:56:36 GMT  
		Size: 10.3 MB (10314983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6fde8b3053da057eccc64ef3a635390ce7a040aafcbeeaa7044753c05d37d288
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65299710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44e5421a431f12176198d788b442c0ca7771eebc40833c1bbbd355ae16c610f0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:11:28 GMT
ADD file:23fbc90316c23c82a8b8da300c8a5623fc3db73c430d1cbdbfab09ab920a25cf in / 
# Thu, 10 Sep 2020 00:11:29 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:51:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:51:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d4d2daf5b278e6cc19610d2a52a8745b441acb4d3e087f6cc35aff05d6ce2a0d`  
		Last Modified: Thu, 10 Sep 2020 00:20:05 GMT  
		Size: 48.2 MB (48156817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a6077d1cb3cebb93b8c52f5ee67a1e8892b694f688bf524f487683dd6d73ae`  
		Last Modified: Thu, 10 Sep 2020 02:04:24 GMT  
		Size: 7.2 MB (7183991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68290485256667f0290c0c36ddfaa24ac0efa67a798c296d2394e992241c37f`  
		Last Modified: Thu, 10 Sep 2020 02:04:24 GMT  
		Size: 10.0 MB (9958902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a221ba658b24a9488f0d68299872a5ce19cce7c72babe1ce36cb848ff38280a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69223797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38770754234db7ffc4055cf74af1117e2c2fda4f94292c5433ff3dda66a5fc29`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:52:18 GMT
ADD file:0b10d18375e8cd004468a07659e73e4afcd826f2808314dcc8fbb6b773c3ed6a in / 
# Wed, 09 Sep 2020 23:52:28 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:32:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:32:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:21fc4451f3aee8da37deddc4046fa3dd8ea41b5a39481b93c43bc5dd385277d5`  
		Last Modified: Thu, 10 Sep 2020 00:00:09 GMT  
		Size: 50.8 MB (50845252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a512823677991a1ec2c1f7550a8c3a6487f162cd565b6dd962c3aa9b66dc8e4`  
		Last Modified: Thu, 10 Sep 2020 00:44:13 GMT  
		Size: 7.7 MB (7742930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8c9bf36c9423fe3a0d5d41b5d9036503bf5255e2c101307b378c250acebbe3`  
		Last Modified: Thu, 10 Sep 2020 00:44:12 GMT  
		Size: 10.6 MB (10635615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:cedf8c70d6b1a4d1ee25dc67d5afb3cf36662d530cb12c99a3ea9b6dfb49f644
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72634401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b642741cd63d91b49a4efe155dff3b11c6892bda07d90cbaa7c08ea7ae4ef75`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:20 GMT
ADD file:0f16119ad5399bd128cd02055185b1f534348a2ea02757438ace9e8b088822c2 in / 
# Wed, 09 Sep 2020 23:42:21 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 02:03:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:03:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9cf7fbf089a5c33a8981bcf78f935777e9a0e1340c0526fbe21a102ede6f5a74`  
		Last Modified: Wed, 09 Sep 2020 23:48:07 GMT  
		Size: 53.6 MB (53574966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36d7641398c875328b89518c4c6818380e424e9aebcaa4eeefd60ae4fbcb51`  
		Last Modified: Thu, 10 Sep 2020 02:16:09 GMT  
		Size: 8.0 MB (8045826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5a56cc39855fb74a0eddc89ad1e907b97eedb1bd547082944b5873578db6bc`  
		Last Modified: Thu, 10 Sep 2020 02:16:09 GMT  
		Size: 11.0 MB (11013609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a45f4ac63ede8ffe4053d1ad6ae689d6ac48c6621d4935fbf44b7b467cb4167e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69196014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8575f5c18263a5b9bf88182384bb72b0c62eb4065b0353242ee7854a8ef056b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:49 GMT
ADD file:c8977e04a216367623fcae06b950449d648b73fe2ebfeea8ac4d43b825fd9072 in / 
# Tue, 04 Aug 2020 06:42:50 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:43:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:43:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d1b4f7d45a45e5da796e6015b373bab6d97853967e128d506ed0b95683b889a2`  
		Last Modified: Tue, 04 Aug 2020 06:49:31 GMT  
		Size: 51.1 MB (51146678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a299ca8f90646201e10c46e3299d7cb736e87e65cf92c7bc2363c5f7d61a0985`  
		Last Modified: Tue, 04 Aug 2020 10:54:08 GMT  
		Size: 7.5 MB (7450327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0eab5aef0c2a963011fc5090931d6499bfdbcfbfa1b05f6c2134d7eec1353f3`  
		Last Modified: Tue, 04 Aug 2020 10:54:09 GMT  
		Size: 10.6 MB (10599009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:39ca9cbf286b1bb5f7b475f375777638f0fe0823b5f1c68b5624f955c868095a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76033867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc819b9c20b3daed6be43ad8ee03a0562d7b2bdafb2509fb1e35834cc930743`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:51 GMT
ADD file:6525cb187fc85a4741e9d9de398149d93f43e196e99a20d48f165a25a1a8f36e in / 
# Thu, 10 Sep 2020 01:07:08 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 03:30:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 03:31:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:184155505be08ee96b6e64926098f03c472ad33bae3d34b8f683480960d7b5d6`  
		Last Modified: Thu, 10 Sep 2020 01:30:22 GMT  
		Size: 56.3 MB (56336687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f84de13452ce499d161f512ceea2535494fd124e4903980cc88297c393465b`  
		Last Modified: Thu, 10 Sep 2020 04:18:28 GMT  
		Size: 8.3 MB (8307371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62889fb00d8e6d8533f5a3ae0d38209c3a2e220aefda427a5f00b595e3862e8f`  
		Last Modified: Thu, 10 Sep 2020 04:18:24 GMT  
		Size: 11.4 MB (11389809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bcb9ad2299c26a5e7fcff9ff33b8fd039fd3018aefe9887e232a1aa2ec93cdf5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69107178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b5d6929e5dfa8af0347b8be633c04d9b3ff2f52abfa530ca850f6ae1dfb5613`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:52 GMT
ADD file:8cf459b787b06e517199d5538d4a79b845b7b7d72ccf10fffdee5a385c0895bd in / 
# Wed, 09 Sep 2020 23:42:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:08:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0777a1517003dde2e616b494a11a7867f55924ffac710d8d2c15b7b50fbeea1d`  
		Last Modified: Wed, 09 Sep 2020 23:46:42 GMT  
		Size: 51.1 MB (51060992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333de3e2208d03a2b8282fff302f01069c5055fcb9e04e30943bfacf9e32d01`  
		Last Modified: Thu, 10 Sep 2020 00:13:13 GMT  
		Size: 7.5 MB (7541388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6b6e21fb8e9c70b582f6590d13e44a04a2d8a32abce90cbd029989466129d`  
		Last Modified: Thu, 10 Sep 2020 00:13:13 GMT  
		Size: 10.5 MB (10504798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
