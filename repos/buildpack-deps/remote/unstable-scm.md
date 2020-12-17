## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:78d4d5351d0c08e0ec515345d0a228b6e3f7b8dafec6a4fb66b18598d0e1c800
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

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:eae55c0515fe5ecf855f26be4ec44c171e9b962ddd17f299b91e8bdf0f74d0c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125760503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a112a83c31adde593315680306247c536a2660d88385f90a1ea439b222bd0fcb`
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
# Fri, 11 Dec 2020 20:39:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:9b370405a02e03f983f976e728ec9583ee8d52d7d8ed64f1f97453afc2d84052`  
		Last Modified: Fri, 11 Dec 2020 20:45:46 GMT  
		Size: 53.8 MB (53849722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f3a372c67ce22d463e33931c9e56a7ae023b090c220ee82cc47f48860ae5c79d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122941544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:113aeff9d74d55177bd21cab8a2574298ffd5ed47a89f95bc47d0a63c77e6ca6`
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
# Thu, 17 Dec 2020 02:00:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:b5f6c898d79741c0a4f968f3105ec2550e291341c33ffaaeda29f2e0c23a1793`  
		Last Modified: Thu, 17 Dec 2020 02:17:04 GMT  
		Size: 53.9 MB (53853453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9f7e2deec2a55bb9f43eaa0ea3114e52e04d8bbe8637ea302c164c0e549c63cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115753860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b422d39ee20a117c62b727b95393ddcd0c0b955d4922857e4670eb16e44cfe`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:26:33 GMT
ADD file:fa1941c40adf31f1de7cad83033e24d208bc560e0818d6c0977fe2e74ef87e0d in / 
# Fri, 11 Dec 2020 02:26:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:29:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:29:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:30:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54bf394474a2aad8c49632d0f0974854752ca4ff40354a996cb0806ea65d7253`  
		Last Modified: Fri, 11 Dec 2020 02:35:33 GMT  
		Size: 49.0 MB (48987318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d959969d53555f2806838ef7825603115e52bc31662dcb17623ba77bf941b1a`  
		Last Modified: Fri, 11 Dec 2020 16:45:13 GMT  
		Size: 7.2 MB (7203302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f104a599ccc89fa932a5c9977f3f9e107d9364f7c408f3d954dd2fc7475cd05c`  
		Last Modified: Fri, 11 Dec 2020 16:45:14 GMT  
		Size: 10.0 MB (9974214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc95b5f2d19ce2f5db34e78db2ba59c101fa341c37c56cee3b9c474bbd05b03`  
		Last Modified: Fri, 11 Dec 2020 16:45:39 GMT  
		Size: 49.6 MB (49589026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7946fc1dcd75182347233bd75a4a4cfef58b67920fb455580be6f8faa551647d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124611009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:581def6d05f356597aae0742ee29ec92f6925ae27392f3635265fb5128b853de`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:46:54 GMT
ADD file:f2ae922bdd400314a7bdccb54b19fed4d2441eabfa76c14f4656754f4639c9f2 in / 
# Fri, 11 Dec 2020 02:46:58 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 18:56:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 18:56:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 18:57:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56da081f64fe82857d727ffa4501fbe0725d416c8b8062202081a62f97fd37f6`  
		Last Modified: Fri, 11 Dec 2020 02:54:16 GMT  
		Size: 52.2 MB (52214368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5ea5ffc1beeb347c710279a3ac88b6b0e4edebb2feaf5c372e9118d8bf5c0b`  
		Last Modified: Fri, 11 Dec 2020 19:09:03 GMT  
		Size: 7.8 MB (7771425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fa408149a9595cea659967e65fc21816e34d52435f6850a7cbd24c27554905`  
		Last Modified: Fri, 11 Dec 2020 19:09:03 GMT  
		Size: 10.7 MB (10653766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545a3bdfa310b636354f945709a533dc9ceed30a5245b06d29e16d8413b2592c`  
		Last Modified: Fri, 11 Dec 2020 19:09:24 GMT  
		Size: 54.0 MB (53971450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8b018a3e9e7cb060f6c9a420780c50ae6ca31270559acae5d189b111ea6c791c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128667173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d97dcd39e886e49045ae0f67621998a97cfdd0dbf60a9f3582ce4e4800d7a3a6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:43 GMT
ADD file:ac372b15438c9387718286ebd1a5b9512e674cdc90319668b3612fcb0cd99441 in / 
# Fri, 11 Dec 2020 02:04:43 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:54:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:54:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 21:55:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bbad886384348be399f916b804d2efe113827e77f3c2b05f9b19a4dd67bff32e`  
		Last Modified: Fri, 11 Dec 2020 02:11:56 GMT  
		Size: 54.4 MB (54407631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a1fa60ad0eb054cbd1cd0835ea8c5cd169d07d3c248db1a1875afc88788134`  
		Last Modified: Fri, 11 Dec 2020 22:03:01 GMT  
		Size: 8.1 MB (8083810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6419106c96402824bca45e76445779dcb0a68ae6180cd7bb95e569e7824326d`  
		Last Modified: Fri, 11 Dec 2020 22:03:01 GMT  
		Size: 11.0 MB (11031118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656fd76cf8eb115da886a3aed66bb03433866762b94f84d1ba2dde4d30245f25`  
		Last Modified: Fri, 11 Dec 2020 22:03:24 GMT  
		Size: 55.1 MB (55144614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:55a14432e47a6c3edeb7aa8074e823515d3f82fd446d6efcc8f5ce22528b86a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125064977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c955ebc3dc50237edbe6ec23577eabb2ffd048536cbf6540ec67d7f74c995b0d`
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
# Thu, 17 Dec 2020 02:18:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:ecc9f97b68d53e1079a6372e2db34d03bbde1f3d3ecf4df179d09936896b9658`  
		Last Modified: Thu, 17 Dec 2020 02:28:48 GMT  
		Size: 54.9 MB (54907646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e167489faf43c037aa7476938619dee1b4cd51328e9fd597b82a6bbf8cc9e130
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135220136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5acec05ccd4960593c45bce2317345ce347c49f3cb00f892a55bcee875ed4b3`
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
# Fri, 11 Dec 2020 19:40:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:77815484de78d295d1bb6bed7b78f53e7d6209bae716c033ec4b4c0b13f08572`  
		Last Modified: Fri, 11 Dec 2020 19:54:28 GMT  
		Size: 58.1 MB (58121245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:aa319c4e0f2b9fac0a0e916ba8d4ec4433287e904cadffa143c6a2ac5d36d6b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123330404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec19588ca067f2b410ef911a44cb2093bc2464d301cf85f5d0003848b666f31`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:29 GMT
ADD file:81f25bd988cd2db6809416e7139b279a1a04ce8e2b864c71e35768d7211232db in / 
# Fri, 11 Dec 2020 02:12:36 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:07:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:07:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:07:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d882124dbf8a54501109f018ee08c93cb805beed092d3bf2e6979740fad5f861`  
		Last Modified: Fri, 11 Dec 2020 02:17:27 GMT  
		Size: 51.9 MB (51894888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6b2001d1a8b91d37dd19d21d1f31ce0dfcc83648225746fdc024ebfa8f686`  
		Last Modified: Fri, 11 Dec 2020 16:16:50 GMT  
		Size: 7.6 MB (7585246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c42824152b87e26d9c06509c0a9035c25ec1a1740793c472931585f433c904`  
		Last Modified: Fri, 11 Dec 2020 16:16:50 GMT  
		Size: 10.5 MB (10525335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeaadbfa1d0a0ab4d448f235e351c619f71777466221df7ff844225f0a1e6221`  
		Last Modified: Fri, 11 Dec 2020 16:17:11 GMT  
		Size: 53.3 MB (53324935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
