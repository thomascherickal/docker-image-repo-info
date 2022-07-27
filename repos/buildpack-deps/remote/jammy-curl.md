## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:6e1863d6a3a1ae01c52a88fbc74146304e5595013574a54c42b80245eaffd51d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6cffff22d396dd078e5e2cd628ccf844eb73626ec518a80adf4230fb6bb8032f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37803023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a6bccdca61edd1e8afbd8ba332375b4a1c0e9af494e990e9af6c8449b09eb52`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:16:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:16:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bca3245ce06c5f92cf1528db00b152cdde37af4bf05c5d3976141dc4a704c5`  
		Last Modified: Tue, 07 Jun 2022 02:27:12 GMT  
		Size: 3.8 MB (3819557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7cdee01903ed192b91b97760507cc18ed88be4ff61e33e87bfe6f1944605c9`  
		Last Modified: Tue, 07 Jun 2022 02:27:11 GMT  
		Size: 3.6 MB (3559751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8b38d601886c85e827412a72db59389bed4004fa4dbf78f3f37fa85e61d00200
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34301330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d47f3f2b32dd554d3836cfd4c207f5bd5f9e86596a7a11c925ffc081571e616b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:51:35 GMT
ADD file:26c86cfcbc153addbca421974e648a7af07234cb3f741bfb030aa0db90b6a7c6 in / 
# Tue, 07 Jun 2022 05:51:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:06:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:06:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5aeb313108e16ff98084efb2ae2830cbe915ea38b3e2fd1e32688dd9d8c11320`  
		Last Modified: Tue, 07 Jun 2022 05:56:03 GMT  
		Size: 27.0 MB (27017432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45c90ba572bc21702aa900361eb375e489774d4b4e6ed6de286e452ca54f45a`  
		Last Modified: Tue, 07 Jun 2022 09:27:53 GMT  
		Size: 3.6 MB (3571068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a804f93703587d0a692de1b12d12224b7248f7d60cd7b0e150aa3772a6901c`  
		Last Modified: Tue, 07 Jun 2022 09:27:52 GMT  
		Size: 3.7 MB (3712830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6c95aa0070f9e503c7d18c2454f2a178c9caddbfc60bbbec53fdc6941b17e4d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35490709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:305a558a5701fd2ebc053891635f41da3d99fe09d983945b0729b85b7467bb7c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:48:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:48:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6155c325759d93f782b168bbc88964ddfe411faa203824e0d07cd6457fe5a6`  
		Last Modified: Tue, 07 Jun 2022 04:57:25 GMT  
		Size: 3.8 MB (3792707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408b3de6df6b01e21cd63f4825cd89fc1054971d120e93b8bba543d30f9ba68d`  
		Last Modified: Tue, 07 Jun 2022 04:57:25 GMT  
		Size: 3.3 MB (3319790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4f0c9ee08ee683bccd0633ef7682eb8581128af204ad69f13dac7991be91fddb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44433267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce91d9f4de92302a664096a43859b83f25a6c4d0a6cdc52b1c37717cce0556c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:49 GMT
ADD file:62ec907c651e833838867bd541cf824f5f609ea4e2b19c4b26cec74a57b60470 in / 
# Tue, 07 Jun 2022 05:46:54 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 23:14:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 23:15:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b851cfa9fcbcb74629241502e21ebbae255fe40a2f26949573f278672b65c308`  
		Last Modified: Tue, 07 Jun 2022 05:49:53 GMT  
		Size: 35.7 MB (35717509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46343fc34cefc64643ad2978b456c5594781763e18fa40d5e422cf0e46e272a5`  
		Last Modified: Tue, 26 Jul 2022 23:57:02 GMT  
		Size: 4.3 MB (4289632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a263dc068c2c9cb95560c1132cef9e8f9817a9a18a04618da486f2aae098c9cf`  
		Last Modified: Tue, 26 Jul 2022 23:57:01 GMT  
		Size: 4.4 MB (4426126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:240a9e093c82dd630ca98d8e0e8a7646b322e7b0a33b61ea443b1124cda66bb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35137335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6f92023f6b88597b197da1cf2abf8a3d385f9e41d47710470e02f9e627420b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 18:18:50 GMT
ADD file:d19287898059e2e99fffa362a449097aaffb132af21a1d1e72c5b898ff785df6 in / 
# Mon, 06 Jun 2022 18:18:51 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 19:31:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 19:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1edfbf9ed16b67ab57bd93f6b8aa57ec157383c958bd3e39e94cdac02ca1db32`  
		Last Modified: Mon, 06 Jun 2022 18:41:31 GMT  
		Size: 27.7 MB (27745919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0b2b247adbcda207142d115c60814f361a65d9e79b584f05cf2c7ae16de140`  
		Last Modified: Mon, 06 Jun 2022 20:28:14 GMT  
		Size: 3.6 MB (3614448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e32164a9b5dee9bb43c693f8c7c833ebe435e4b86660f7a14ce30decd26898`  
		Last Modified: Mon, 06 Jun 2022 20:28:12 GMT  
		Size: 3.8 MB (3776968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7d1360570849e9883f22e9ff6887167ecb38fa516bbbe25d8bbcb1e632a798a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35931098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81e5d99dbb0096d9b6658182f0ce821b139f389c7a5fda313f72f7239a790290`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:57:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:57:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c21ee3fc0eae5db8aa29b016cfeb4872fbed236a180eb98f9c578ecb1d24f1`  
		Last Modified: Tue, 07 Jun 2022 06:09:06 GMT  
		Size: 3.8 MB (3821587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869606af1d12204312dc361122a3664437ee80f9a31ca39e0f6fc7c7b9ec5e7f`  
		Last Modified: Tue, 07 Jun 2022 06:09:06 GMT  
		Size: 3.5 MB (3471029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
