## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:a9a6392fb4b683a5840a79134f20e432384916a8effb03f416c5681d45eabd76
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
$ docker pull buildpack-deps@sha256:7a5b23ab4c1ef03d310ce1bfd492cb01e8703d251e7e70d3cd4f3067fdc1a5b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36374105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28972bebc7a752c1f9d4c433c82d72d81d93914c3bacd337b8ad7aab5989c9d8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d74cdf65aa24870bf2345d9c4fa42388a09f5388e94469f3e6f08644a35dba`  
		Last Modified: Fri, 22 Apr 2022 01:43:43 GMT  
		Size: 6.6 MB (6641787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dc3910681266625514ae173ec9b5aad8bd2bcc5b5ed7ce0e668a4f43e1a93c`  
		Last Modified: Fri, 22 Apr 2022 01:43:42 GMT  
		Size: 3.0 MB (3022435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2ad0779d0a643e03fef83b203659cf646d699a5aa5713ec751181362801977b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30597751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bcb9765ab0be412a34f844a4fc2f60611517e6c37be27f4c2d969b3026db285`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:25:38 GMT
ADD file:3230d8a499e37ff816595cbac3892a80005afccf8a55053c28e24989d52de08b in / 
# Wed, 06 Apr 2022 03:25:38 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:03:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:03:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:419a71fa3c92c7dd0e8cfbfdf694362de1c27dafed508aeb2e5bc9ff8376fc98`  
		Last Modified: Tue, 05 Apr 2022 13:12:06 GMT  
		Size: 22.3 MB (22301415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da9b34da99841919b0af9f447099b7d6b004654e1f27cb9822534950a1f44bc`  
		Last Modified: Wed, 06 Apr 2022 05:23:44 GMT  
		Size: 5.7 MB (5711821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b36893f5a19e981da33035ae9e385a11b6213d3c677e36b6da86f20b55b167`  
		Last Modified: Wed, 06 Apr 2022 05:23:42 GMT  
		Size: 2.6 MB (2584515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b6f5b1c6ddbeec77bee0327bcbbb2d25de2354f8d85feccfd9ac84b011306580
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32383682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa877f6e0226e484651d7e5029dce67729b26350387bbef41347e10355d160e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:51 GMT
ADD file:bb36cf2c131b65fcf3f10eac5cb640ad749d77110482b30bff982a284aa9e9ec in / 
# Tue, 05 Apr 2022 22:40:51 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:05:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d35feac4abe85b38af36ec148f2c2dc7a795f9862a0b6dcf2a1511b752a44996`  
		Last Modified: Tue, 05 Apr 2022 13:11:37 GMT  
		Size: 23.7 MB (23730866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d801162d026edfcca58a7cb8496fef045e4a4d9b8a9222ddd9150ea3a76c0e`  
		Last Modified: Tue, 05 Apr 2022 23:14:45 GMT  
		Size: 6.1 MB (6082517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d8ec603557719433228d854af4b6ccc8cee23ff6b03fd8959265858f5cf59c`  
		Last Modified: Tue, 05 Apr 2022 23:14:44 GMT  
		Size: 2.6 MB (2570299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:13252bc0d7d694c58219fd9f673ad15af92130d536e2677374795285c7c5013f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37131667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f409d77e400be4bfc8037b6ae8da36f53a30a0a95e2380c36fdf5d650e92faa5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:53:57 GMT
ADD file:164f0ee7842870b8f94ab2ee8f9151b49e08f461b99fdfa1b7586fa864d4a320 in / 
# Thu, 21 Apr 2022 23:53:57 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 00:16:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 00:16:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:57fda0d035c311017871931fe2f2a2c241e46b4bc95d2a87dbf533afd8e72668`  
		Last Modified: Tue, 19 Apr 2022 13:11:34 GMT  
		Size: 27.2 MB (27163453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80020c29fe6d0575254dda040fc655dfaa84bca26136ce9b29f390d4fbb29b6`  
		Last Modified: Fri, 22 Apr 2022 00:22:15 GMT  
		Size: 6.9 MB (6929643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cdf0da60441cb8fc028c8ef1f25bf94a0e154a9fe189221f99d9d7e17e0579`  
		Last Modified: Fri, 22 Apr 2022 00:22:14 GMT  
		Size: 3.0 MB (3038571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:445874864f13ae0d821935f63091610da722c026f99e6bc2489617faf7fd6212
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41214813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ac4383bcdcac122088f60edfdfe2cfb3927bf0553655aee8917cd4df036b3a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:14 GMT
ADD file:1dc494089c70f6414b0a1f5e2e09605266508bf5ec19e1e2fb17028253f8953d in / 
# Wed, 06 Apr 2022 03:35:17 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:14:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:74c6ac89233d470993bd9d67b39dc7ccb63096b55dc274e26eb50345bbecdcd8`  
		Last Modified: Tue, 05 Apr 2022 13:13:08 GMT  
		Size: 30.4 MB (30438429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563966e866b8408203dd947bd37b2f758861f63028138d65cc64046803ebd89e`  
		Last Modified: Wed, 06 Apr 2022 04:48:34 GMT  
		Size: 7.1 MB (7056771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684f920d2f0aebaf225cb6f750b185a3aa32bbc6ce9e0f72a1a80702b33ea9c`  
		Last Modified: Wed, 06 Apr 2022 04:48:34 GMT  
		Size: 3.7 MB (3719613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:211143c2ab1142fcf58fb24fd0b866b3dcf6bfe07b179cc5ab2f9bf2a19fee54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34672976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4f3aebbf1a49ac8203089dd95e8d3922fffd25d85b13558405d634a6abf2773`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:17 GMT
ADD file:bc2c78cc62a5e94931f8bd76f2fa050b19598c050fc18aa56bbd202826ec784b in / 
# Fri, 22 Apr 2022 00:39:19 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:30:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:31:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:18c1f746bcbccc4e7599497df0d1d562571c9ecd9effcfb7bee0bbe17d1156b5`  
		Last Modified: Tue, 19 Apr 2022 13:12:34 GMT  
		Size: 25.4 MB (25365079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8405e5ec3de7029a8d9e579e70b8ad1e1c0c54178d2bceeddbddd9891f208caf`  
		Last Modified: Fri, 22 Apr 2022 01:50:36 GMT  
		Size: 6.3 MB (6332722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f8f2095b8a73b68dac155f8b672164e44e681428870a909eb95d1bbadfd2d`  
		Last Modified: Fri, 22 Apr 2022 01:50:36 GMT  
		Size: 3.0 MB (2975175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
