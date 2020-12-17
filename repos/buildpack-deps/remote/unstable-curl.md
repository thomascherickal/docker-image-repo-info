## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:4adac52da1d69a7349d42b58478cc3594d2029b2a1460c767f5b345c71450714
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

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:adaa1110d05962b994759c9fadf437bc8b6371bc20645b7b0998e5fdde2523e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71910781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:633377eeaf645f7f47188400665b88acbbed523b78c7fa3a48abc92c885f5f79`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:07:48 GMT
ADD file:51a85ad79ebd7e288cd0ea14cd2ae41990aab2d77352f801f09c3a4682cb83a9 in / 
# Fri, 11 Dec 2020 02:07:48 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:38:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:38:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ff8cddfd21234a3c42ee0af471b251a807aa29af4ca00392976a17d3257ed269`  
		Last Modified: Fri, 11 Dec 2020 02:14:23 GMT  
		Size: 53.4 MB (53352668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef14a4ea0da8e77ac285fc34da3f621eefa6d7488e15459c75f3b0e6dd417ad2`  
		Last Modified: Fri, 11 Dec 2020 20:45:29 GMT  
		Size: 7.9 MB (7909956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808455b058cdba0d0507a63c245515e4edb434ac79066cd7ef0f85bffa77f8bb`  
		Last Modified: Fri, 11 Dec 2020 20:45:29 GMT  
		Size: 10.6 MB (10648157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:52089c49d51fe5cb4628b8e41d3a1678bc41f02a3eb82160ac3565b25cd2c486
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69088091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14535af0059fac782c9fa5c800008947c810df2d469ea662ab041392e8943d0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:07:43 GMT
ADD file:a57353f597051225232a9e7abed847b86e4c6dddd2072732b4625acbac7128fd in / 
# Fri, 11 Dec 2020 02:07:47 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 01:58:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 01:58:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:af6b8b544b162386c7b3c6d5c131158e341ff3b454198faf077cc6c1427321df`  
		Last Modified: Fri, 11 Dec 2020 02:17:13 GMT  
		Size: 51.3 MB (51288429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32247566aa2494e1bf6e9f3c3f6665570e5b6ca9c0efc4201c1ffe6fb588f9`  
		Last Modified: Thu, 17 Dec 2020 02:16:24 GMT  
		Size: 7.5 MB (7464549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79eb6eeea7eb9883a84eadf7c898a88cc2a4964df470eae23c4ff5d9d3a43b01`  
		Last Modified: Thu, 17 Dec 2020 02:16:24 GMT  
		Size: 10.3 MB (10335113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cfce4f5d68edf1df54dda28c78d72f2200aa2e324474e92183ba7614e665bb0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66164783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4f365e5cae12c5898d9f313832343d0bb3295a8a0d8821f665e7909e9c9d735`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:26:33 GMT
ADD file:fa1941c40adf31f1de7cad83033e24d208bc560e0818d6c0977fe2e74ef87e0d in / 
# Fri, 11 Dec 2020 02:26:39 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 08:20:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:20:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:54bf394474a2aad8c49632d0f0974854752ca4ff40354a996cb0806ea65d7253`  
		Last Modified: Fri, 11 Dec 2020 02:35:33 GMT  
		Size: 49.0 MB (48987318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138f735b8d86c59a8efe8701930d51f00aab24ac3ec03c9701b22176d372ffc5`  
		Last Modified: Thu, 17 Dec 2020 08:53:55 GMT  
		Size: 7.2 MB (7203215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da4363bd6c95216be34a5d4d34419bc9306f517103d0013669f9fa1bcfd225a`  
		Last Modified: Thu, 17 Dec 2020 08:53:55 GMT  
		Size: 10.0 MB (9974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4978b94e5eb829c0f10e5b19656a9da4b16e335b80601e935c10454c5dacdc3b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70639729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0d691f1c298b510838912286c919561709b980ccd0393c4b49d440146b9723`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:46:54 GMT
ADD file:f2ae922bdd400314a7bdccb54b19fed4d2441eabfa76c14f4656754f4639c9f2 in / 
# Fri, 11 Dec 2020 02:46:58 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 10:09:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:09:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:56da081f64fe82857d727ffa4501fbe0725d416c8b8062202081a62f97fd37f6`  
		Last Modified: Fri, 11 Dec 2020 02:54:16 GMT  
		Size: 52.2 MB (52214368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c005981f7ee140e28c3d2e8afd11ba4168bd84130ed5887eb9c2bf7799c9d7`  
		Last Modified: Thu, 17 Dec 2020 10:39:38 GMT  
		Size: 7.8 MB (7771435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0395265f0c70c22b0a204b62d47d48c5edb8cce1630c9a39e29b983acf94fad0`  
		Last Modified: Thu, 17 Dec 2020 10:39:38 GMT  
		Size: 10.7 MB (10653926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0515a57a6c51304e67415e7cb267ec16ffc4c983cd46c07ce07e6b6a78bdb352
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73522749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18c32febe50164d652f5f5ff9e93c341e3238a3662d80b9f7d2d7cf665a00868`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:43 GMT
ADD file:ac372b15438c9387718286ebd1a5b9512e674cdc90319668b3612fcb0cd99441 in / 
# Fri, 11 Dec 2020 02:04:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 08:10:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:10:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bbad886384348be399f916b804d2efe113827e77f3c2b05f9b19a4dd67bff32e`  
		Last Modified: Fri, 11 Dec 2020 02:11:56 GMT  
		Size: 54.4 MB (54407631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107edbf54231bab6e619380b341236d89d7c373021e0ca4ced89d4b094f74537`  
		Last Modified: Thu, 17 Dec 2020 08:27:04 GMT  
		Size: 8.1 MB (8083852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770453472dffc640059e49933b5042237ef0d2a63e4ecbc572da6109134c440b`  
		Last Modified: Thu, 17 Dec 2020 08:27:04 GMT  
		Size: 11.0 MB (11031266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:41c67cdc48b3f0cc8e7370b8582a393f7e94a6fd7cfa52a1d1a7ff8e6c593733
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70157331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84151c18eecd0b176e5d9ca4240497a39a7787d60b2bee148a969b87520ae2c0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:55 GMT
ADD file:144f263fbf8197586830814ff675d3c7d3ac8e3df7debe6633a1e91f84ff845b in / 
# Fri, 11 Dec 2020 02:03:56 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 02:16:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 02:17:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9b60fb1f705939e8d3e124cd99cb825ac48613619a7a75de5656f0bde8bb1f05`  
		Last Modified: Fri, 11 Dec 2020 02:11:04 GMT  
		Size: 52.1 MB (52069726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b68d01e1e193d2323fdb149c22c9d1eabf16cc4c4941778e09e00b76b2f652`  
		Last Modified: Thu, 17 Dec 2020 02:27:52 GMT  
		Size: 7.4 MB (7430962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0d13fc3849ec4bd1574242ac59b139c9b0b7dbd2d0afa316911acb27045559`  
		Last Modified: Thu, 17 Dec 2020 02:27:52 GMT  
		Size: 10.7 MB (10656643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:62092e9b95736875c9bb5a3f6e1faba71a7e13222afc69048b49d09967a8f68a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77098891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c216dd799f70798cdbaf81e4ee75e36f6db03f57e60d10a39750f1aef844f7c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:34 GMT
ADD file:d6769e024c4c1bf3ac50de798e3b70ddbae5e8dc6c4edc64cbf31ef39fba2896 in / 
# Fri, 11 Dec 2020 03:34:40 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:37:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:38:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:897184b44dea4f1c1b646278a369b1024dac0562097178b81b92da84665fd760`  
		Last Modified: Fri, 11 Dec 2020 03:42:05 GMT  
		Size: 57.3 MB (57314487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee2620ff3e328f5bc3688195568d3b5b1cef135eedf50ed4cfc28b1a10e1f5`  
		Last Modified: Fri, 11 Dec 2020 19:54:04 GMT  
		Size: 8.4 MB (8363461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c218c75d39db360d7134c468b34f1237b347888e09366545db43481f8e2a50`  
		Last Modified: Fri, 11 Dec 2020 19:54:04 GMT  
		Size: 11.4 MB (11420943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3017614b9b409ee69b2becd2c84d78f54ec8384b8e00874525b2fbc0ed9680a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70005606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a64da09af5caa2c1fe742df6511e82c9994984abfb4205faf1d494312a45f4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:29 GMT
ADD file:81f25bd988cd2db6809416e7139b279a1a04ce8e2b864c71e35768d7211232db in / 
# Fri, 11 Dec 2020 02:12:36 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 11:18:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:18:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d882124dbf8a54501109f018ee08c93cb805beed092d3bf2e6979740fad5f861`  
		Last Modified: Fri, 11 Dec 2020 02:17:27 GMT  
		Size: 51.9 MB (51894888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d19883059c6574b24a1136327bfb2a42e1709d68c54db24a7b443ea27ba6fb`  
		Last Modified: Thu, 17 Dec 2020 11:47:32 GMT  
		Size: 7.6 MB (7585305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3620af9fd07136686b0a9a787703282d968f4e2b3e04654c62094c925d7eefd`  
		Last Modified: Thu, 17 Dec 2020 11:47:31 GMT  
		Size: 10.5 MB (10525413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
