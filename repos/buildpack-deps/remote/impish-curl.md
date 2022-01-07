## `buildpack-deps:impish-curl`

```console
$ docker pull buildpack-deps@sha256:876a898cf56721d443859034804505426f6254babcc7f2c44c98d427e2597ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:54c923092a83d0fd403372895cc7a052c5d93975a64600e8b2dc87c3ce47494a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37624372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5784379919f76e6e2636d7558d1932259ce9a619c55a89fd18de979439e5a863`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:20:34 GMT
ADD file:c061cabbaa10b98eed8dcea770d97000a2861c407f5208a0327bef2b38a99fee in / 
# Thu, 04 Nov 2021 22:20:35 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:56:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:57:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ae6e1b672be676522e8af69609544dd00b8517e394592a58194383b26e9b54c5`  
		Last Modified: Thu, 04 Nov 2021 22:21:31 GMT  
		Size: 30.4 MB (30378721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4488401b75c6ec432177829c795e1ec36857d568171ae1f197c2c24a9b7e7d8d`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.7 MB (3693784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb8a4e0bca131c5b9e451c10a345a0a13be03cf5ac1220cdc85f170d17be763`  
		Last Modified: Thu, 04 Nov 2021 23:03:09 GMT  
		Size: 3.6 MB (3551867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cdf2e5e90315eff8c9fa17950a02925e550d668cabf6a092fd629fd2489cb835
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34103195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4c36290c105f7d65eff92415d0b8b56be4f54a2051c3e35b8e330c7dadda26e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 22:31:15 GMT
ADD file:675ad5623adf2dafceb59e4a67c75ca26f664127c76fe61c1903cc85d16b9abb in / 
# Thu, 04 Nov 2021 22:31:16 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 23:28:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 23:28:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f7dc858b30797c13a0706f9660d1290ae625ab3436fd5db984b0dac888ad9c8f`  
		Last Modified: Thu, 04 Nov 2021 22:34:32 GMT  
		Size: 26.9 MB (26917157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64923825f2b20992e031b3992dc8c85722c1421e18d7f0fd69532d01d31c2617`  
		Last Modified: Thu, 04 Nov 2021 23:37:31 GMT  
		Size: 3.4 MB (3443243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d36d145711f3ed07bdbf6134addb14e00b663cb32b4de67ff1674023832998`  
		Last Modified: Thu, 04 Nov 2021 23:37:30 GMT  
		Size: 3.7 MB (3742795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:00c6025c7a15dfe57955537030d672bcdcaf4a2389fc446007e602d155927bf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36031863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b11808ca59b32ca29aceb263695f64a95c22f3784efef11a16304f51f440ff1a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 21:55:45 GMT
ADD file:1b42b91df70bf5eb9529802354c8c97bb9ba991a7885a3fdd4ad5be4b662b70c in / 
# Thu, 04 Nov 2021 21:55:46 GMT
CMD ["bash"]
# Thu, 04 Nov 2021 22:28:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Nov 2021 22:29:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:07806c11d5adbc5d83daf2661f72147213f9056f681e452180dc14d81e368e17`  
		Last Modified: Thu, 04 Nov 2021 21:57:10 GMT  
		Size: 29.0 MB (29026100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a952a5c90bcb8e3a8ab1bd7854d8265e7fcb3cb0c0f417fb5722e8f3e0972208`  
		Last Modified: Thu, 04 Nov 2021 22:33:00 GMT  
		Size: 3.7 MB (3678628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca9702f2a91f991f023bbb9b582e71befe4781bbaa74653b2458540b02c0e3`  
		Last Modified: Thu, 04 Nov 2021 22:32:59 GMT  
		Size: 3.3 MB (3327135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0cc84931e7355f0a2ec18838056c982f9599d01d99f0a81c365098ed2373f8cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44563129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940ae21526802e5c51c15c215053b8095e827480a47aaea8d00e399c958e4dba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Nov 2021 23:51:29 GMT
ADD file:dc4e5dbd5333b274b2af1c57862eeb96c4b2eda9e8d1a5b766b4ff2aa242106f in / 
# Thu, 04 Nov 2021 23:51:35 GMT
CMD ["bash"]
# Fri, 05 Nov 2021 01:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Nov 2021 01:51:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6fb8a15f7529caac80795ba7b74d3c07d163030311fab31ef7b9eda5d4612190`  
		Last Modified: Thu, 04 Nov 2021 23:53:39 GMT  
		Size: 36.2 MB (36174155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f8d539d495275857666e419e2349b4afd49b9e35684be52fa958a9edfc64`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.1 MB (4146837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f57d31cc6184d7de4f38b999b49a84d09a99cd73ecff5fc148f918d7a9f85`  
		Last Modified: Fri, 05 Nov 2021 02:01:11 GMT  
		Size: 4.2 MB (4242137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:a60d9614189e9a414cd72cc5bcf35ff30825c9ba8c2ef9c68a3df23684370df2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34500741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386b795e60ea56fff90f8871ec0d6d4c2fa29a17fe88c124d55251bb078e45b9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 11 Nov 2021 01:34:25 GMT
ADD file:def88534019c26953298b38d1af30a296db3d6995d6c801bc98407de70a9e1a6 in / 
# Thu, 11 Nov 2021 01:34:26 GMT
CMD ["bash"]
# Thu, 11 Nov 2021 06:26:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Nov 2021 06:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c236a68e6fcd6aac214c2851f12d0e004328b6cc65c84adea73ec2c8eccd27b8`  
		Last Modified: Thu, 11 Nov 2021 01:50:51 GMT  
		Size: 27.2 MB (27206693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32c0816a844c3da682a583d08b1d066cbf7fdaff37ecc1ffe756a1762b5116e`  
		Last Modified: Thu, 11 Nov 2021 06:54:43 GMT  
		Size: 3.5 MB (3490272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd32937a18c0c808ff182ae5991f2dcc6394079d138e4d6880d9013b9e5998a`  
		Last Modified: Thu, 11 Nov 2021 06:54:41 GMT  
		Size: 3.8 MB (3803776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e7d297470161f1cb35ecaa59e269df522c549969384be9106590f1e4a89c42b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38257255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81d8008da67d1259e1a1947e8bd12c4161248619c87c61e24a715a295a147440`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:43 GMT
ADD file:d2d689ec5bbbbec520f5fc8ea75e1d642f177a30c5937027ca800b3a9ccf5b83 in / 
# Fri, 07 Jan 2022 01:42:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:07:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:07:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:77bd6b10105ec281aabfad8249bf82b48478e0eac3503dccd5d75db49b1dd586`  
		Last Modified: Fri, 07 Jan 2022 01:44:35 GMT  
		Size: 30.5 MB (30526144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ac2bdfd743d34b81a7e7855ce015d3dcab3c711230a384e4e0f31da363e5ec`  
		Last Modified: Fri, 07 Jan 2022 02:14:03 GMT  
		Size: 3.8 MB (3767780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f22dc9fa326e82f6b809f067452b917fde08df5f8c3ee42998a9c882963eeb1`  
		Last Modified: Fri, 07 Jan 2022 02:14:03 GMT  
		Size: 4.0 MB (3963331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
