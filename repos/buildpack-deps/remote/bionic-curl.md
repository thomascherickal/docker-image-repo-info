## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:d4beed37e881ddf445a54a90cc5ca5e4e1e70d122bc5b4dcaa24ac93e19c12e5
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
$ docker pull buildpack-deps@sha256:53a331ea210409bbb876f16043e7794ad863599205ae49bece1889e7fc6f1ed0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36372917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94683e0a5dfe6ef758abc54690df7c50ef11c7c15e2607e80be01ae7fd91913f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 22:39:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a47fecd0167fa8860c53b97b993d4cdd955581b4a4cb77aad837a5946f76c7`  
		Last Modified: Tue, 05 Apr 2022 22:57:06 GMT  
		Size: 6.6 MB (6641629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f33f66947c23947cadf3607dae800cdba6a21e6952f10580b47120bb32b3731`  
		Last Modified: Tue, 05 Apr 2022 22:57:06 GMT  
		Size: 3.0 MB (3022350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6f391663368344db81086792af6820993bd3b16ac14ef974f1b7de89a299087a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30605088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5780ee29340d6934bbe79b88fee887bd917a237cd8351b858b8f8cb78d32057`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:07:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:07:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dd41a6c49eacf0df81b34978f371986d045163bc627fc8cc72de7188772b43`  
		Last Modified: Sat, 19 Mar 2022 03:40:45 GMT  
		Size: 5.7 MB (5712348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd796a264aa4c81e3c709b9f64a9058add3ff5a5d6182545c52efe99ffacdc7d`  
		Last Modified: Sat, 19 Mar 2022 03:40:42 GMT  
		Size: 2.6 MB (2584607 bytes)  
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
$ docker pull buildpack-deps@sha256:ad964d4dc6bdbbdb1f2ff75692f1cef6519654f8b2854a86181fc8cd0646d401
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37130470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b39fe7e4a6cd7673d5f2a173c0ade6e0deab833f432cb2518c4baa03a274dad7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:01 GMT
ADD file:d9edbb973ba7a0ee377e64ec7b7135478b3259223d5fbb83185ae0653ec0773f in / 
# Tue, 05 Apr 2022 22:39:02 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:02:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:02:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:12d1023794ad0425246985d1a3b4e8ad7a1368a1a6bd0f7a2827dd443349538b`  
		Last Modified: Tue, 05 Apr 2022 13:12:34 GMT  
		Size: 27.2 MB (27162492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebb435852a701846708d5c45ba1efa4331a97e160a2cb2ee0f6b5bdd612990d`  
		Last Modified: Tue, 05 Apr 2022 23:11:54 GMT  
		Size: 6.9 MB (6929461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf3e6751bc0c359ca9e2274739606a1c06972f2837a0134d959a801d1687e31`  
		Last Modified: Tue, 05 Apr 2022 23:11:53 GMT  
		Size: 3.0 MB (3038517 bytes)  
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
$ docker pull buildpack-deps@sha256:edbb698bc5d90a57b0166d221993a6fe1951baf387ad2996603bbd4dc1ca55d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34673552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f8e0a108a290a12cbfaa42174c46516c11047770e736a9e767d79731b6d068`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:55 GMT
ADD file:7da6edcff7f600bf3a5d740cd585065c6b3748ff587c0627def91686d1bfe54d in / 
# Tue, 05 Apr 2022 22:41:57 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:17:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:17:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4b0f8a5e4614be4866f08e8772b57664127164f512df03d05a52607176caa02f`  
		Last Modified: Tue, 05 Apr 2022 13:13:37 GMT  
		Size: 25.4 MB (25365860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8129cd0a5659bbabc817a4bd1c8756c0b31fe290cc223c764308d08599353d`  
		Last Modified: Tue, 05 Apr 2022 23:26:57 GMT  
		Size: 6.3 MB (6332585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff6bd647de512734584c4049c7a22c880934ffb49b09b9dbebf9f93233154f4`  
		Last Modified: Tue, 05 Apr 2022 23:26:56 GMT  
		Size: 3.0 MB (2975107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
