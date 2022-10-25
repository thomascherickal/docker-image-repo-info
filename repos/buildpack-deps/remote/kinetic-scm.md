## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:044006a56118d10d105fef337fa49803641ab52652693b35a7a4b6a22555ef48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d04920e171fddca160ba2431b2421bf49b424767a2a15f5be91bb9d94f21bb2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77583500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ef1de29f63807a6093e6af698173335a81692ab641a3e02e63bc9df42ea5f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:28 GMT
ADD file:3384549425c94b92a7d7be15958e3ec7494bdf83242deb465d9059d4362d34d6 in / 
# Tue, 04 Oct 2022 23:35:28 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5887826a0d8b4c403d9bfaf57279fd8b585d272c3f450d374349365dc22cd8ef`  
		Last Modified: Tue, 04 Oct 2022 23:36:56 GMT  
		Size: 27.5 MB (27455077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7fd9cb5adf6a195c3c2162caa409d926d4342598cad09f7fa4691e9ddd25f`  
		Last Modified: Wed, 05 Oct 2022 01:25:38 GMT  
		Size: 6.8 MB (6780586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9023f9ecbe71ceaba400cb934168d975ecabc157d85fe246f71d3d684947742d`  
		Last Modified: Wed, 05 Oct 2022 01:25:37 GMT  
		Size: 3.6 MB (3633909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d44eedd822ec1ffd1b32f87638bae3694f27cf99e85f8d3d8f6d1f2857fdc1`  
		Last Modified: Wed, 05 Oct 2022 01:25:54 GMT  
		Size: 39.7 MB (39713928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2965cc2f6b4e99430ed3e5dc6e19cff61861fd39ce9247198d0446c4ea18da12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78226975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf87da53eb6a1926ffac398aa2b41ffc1c7ba4e19fa01b0c1e132a9fcfa6d7ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:09 GMT
ADD file:4b538f2c7b46aa601d747159ce9e8c2c7a99b2b6e09e4efe1073ca58e47fbeed in / 
# Wed, 05 Oct 2022 00:14:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:47:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:788f7bb1e1d719f6a9a9b3b1530cc5bbe5b808a2ad77a65f23e2c6d15b8ae546`  
		Last Modified: Wed, 05 Oct 2022 00:16:28 GMT  
		Size: 25.9 MB (25873193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aeed2022326b456329596b112851c2e027ba5773dab33fcd717efb1a016274`  
		Last Modified: Wed, 05 Oct 2022 01:01:56 GMT  
		Size: 6.0 MB (5955685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a4829745394c3402e5970b4558ef9fe23515f895e7f8a99fe24ae33a7c4f3`  
		Last Modified: Wed, 05 Oct 2022 01:01:55 GMT  
		Size: 3.8 MB (3801708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fb45c30ad58843e78384afd22f7dec65ac55a285086da2083dea2426fd37e`  
		Last Modified: Wed, 05 Oct 2022 01:02:19 GMT  
		Size: 42.6 MB (42596389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f9e6c255feb050995c15d584bed8b4ef31d7171ecc8f79741ce561d7ab013ce5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76373070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e46d98faf0c177cab0e52968d9d062a3a4f181d3c42f5759c5eb9615ccd5b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:06 GMT
ADD file:30361063c284df6e20a85ff95b9c7b93648fe9e04ac935c9ff888e5c5f3af7ea in / 
# Tue, 25 Oct 2022 05:55:06 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:19:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2e58a4bc1e52e3ab8904706a68a79146364ec32d8caf1bd106c3c9966a38fc`  
		Last Modified: Tue, 25 Oct 2022 05:56:30 GMT  
		Size: 26.7 MB (26676995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c8913a9c66f64a1f5ca1349c8a8b9923f9eb9c8aed25bf3ec160a33e5a796`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 6.6 MB (6607031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491d7cc7a42af61771e26652e91532db813e380fa19339f7279420206df0290`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 3.6 MB (3602476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2cf60ff33717c4a17f0ca2f77473b69d8d357e4dc81ef8bb8a5e24382aa106`  
		Last Modified: Tue, 25 Oct 2022 08:36:17 GMT  
		Size: 39.5 MB (39486568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ce93a24cd078d6b8c4f5f7301e8e03082dc0b280b7699a23b4a638e67ae2efdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.3 MB (88334263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b98ffc392030e610f3af3f6119e1fda61df1f4b3d9ae0d893603fbbc1949cfc0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:14 GMT
ADD file:60dd11bbfa9f1e2bc613c7f05cbbb83bca9e4b81550b6a0540a5d1d39f870cdd in / 
# Tue, 25 Oct 2022 03:26:16 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:40:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:40:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d37bc653a986baef621c195bf8def80ca65133b8a3917bbd3a148b31bc1704f`  
		Last Modified: Tue, 25 Oct 2022 03:28:34 GMT  
		Size: 32.1 MB (32099941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc18decfda3085820c97e73c59dba18c534c4455c2eafc5812d29975ad7a9292`  
		Last Modified: Tue, 25 Oct 2022 06:57:12 GMT  
		Size: 7.8 MB (7752006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a931134d9aa21913f6400e3083b4c6955008f9fab7eae04019249a1d912c279`  
		Last Modified: Tue, 25 Oct 2022 06:57:10 GMT  
		Size: 4.4 MB (4361351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33eb213c2d45440f6da62e4c97dcc2936c1a9881896421d53a86927e2618b29`  
		Last Modified: Tue, 25 Oct 2022 06:57:35 GMT  
		Size: 44.1 MB (44120965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ab238169f3b08dc7c08c8e3ed46e6ad74014ba89c7d7d398a9038687df3104a5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78270889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bec2b637df9811eabf5c8c05afc79681031c55e2b577567a231be07852233f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:16:49 GMT
ADD file:2d01ff45e6105658cf6791d4ade5cc3168c7d455422fc973a54a795907023c4e in / 
# Wed, 05 Oct 2022 00:16:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:00:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:01:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 03:04:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69c33ccbf3d1b09c78fae3f88deb756ae33a9e4610a01fc9ab8b457ee6107d7f`  
		Last Modified: Wed, 05 Oct 2022 00:35:11 GMT  
		Size: 25.6 MB (25618700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6742bf73589f8dd7c6c3ba8c0c07b6783a8c31c40b8e815941b550d904b49030`  
		Last Modified: Wed, 05 Oct 2022 03:54:22 GMT  
		Size: 5.9 MB (5938180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b60e6247434b31a05dcae8802e410a92a3e9e6f9f6472455a58d4c1d5e1b6`  
		Last Modified: Wed, 05 Oct 2022 03:54:18 GMT  
		Size: 3.9 MB (3881311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde1ee2ce8c7376ef3e85ac490d31dcdf52bf954c3186472c53f3404c2421078`  
		Last Modified: Wed, 05 Oct 2022 03:56:41 GMT  
		Size: 42.8 MB (42832698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ca6937235c92176f4e66e5e83e654d8ac06099c69d6cdd2917dca4640643463c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75669106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15939ebf9f49b3608111d36fac9b9adb1584829b3dcfba4701e71c081de209c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:31 GMT
ADD file:9c0c4172b14f0d37b0b074729a4738aeb165efe5c83e2d9bfefc5b39e4a4fe0b in / 
# Tue, 25 Oct 2022 01:23:32 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:44:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:44:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf61a33f110308ce64c1dd7a5dddf2a5587ee1c8ab2351219b925428957cbc10`  
		Last Modified: Tue, 25 Oct 2022 01:25:01 GMT  
		Size: 26.0 MB (26022178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df11273ce2e4ff8fbfe44b4708e1c3b2323d38c23cc29bfb9935c1788807165`  
		Last Modified: Tue, 25 Oct 2022 02:53:37 GMT  
		Size: 6.5 MB (6473357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36f51f919c9bd6bce882afd5ce69c1de2f32276ae54369c26ae41702ff241ce`  
		Last Modified: Tue, 25 Oct 2022 02:53:35 GMT  
		Size: 3.6 MB (3625569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ad44ec319ab50167d51a4bd01dd344bd736541842217bc94d0c6da1960b16c`  
		Last Modified: Tue, 25 Oct 2022 02:53:49 GMT  
		Size: 39.5 MB (39548002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
