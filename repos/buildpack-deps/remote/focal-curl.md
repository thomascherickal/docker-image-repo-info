## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:139fbe4d080e36a24a07ce826b9f34793aed0f2ea4a3060d622f2f9204bad04f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:focal-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:577ab5375346239a411e7b8a20882febf76564a20092492c60089c9614bd58fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39946087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3978effc4af1fb7f140324ee1b2ef790c7b87608d8633f6099ac4a442193e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215646fa628a9c18e31f7ea7321ae4140b44d69995ec4cdf3968cbce9a5c0b4`  
		Last Modified: Wed, 05 Oct 2022 01:23:38 GMT  
		Size: 7.7 MB (7747231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6c7ee6250b02a6cf0a3a3080d082e4ce4f858e2749921bc2623c896c487897`  
		Last Modified: Wed, 05 Oct 2022 01:23:37 GMT  
		Size: 3.6 MB (3624405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8b15c3f4b12c531ad54a4129ad38bc19cb166573ec4213563fc6bf9ee949f5dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34433973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3679946ffe22fbdc937f477ccad2f1008636611a792de1cc56c09bc3c310d8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:42:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8314cec2c7a441a36532dc89979b531fd7dab365416e8d4f077f16c6322a222`  
		Last Modified: Wed, 05 Oct 2022 00:59:17 GMT  
		Size: 6.7 MB (6740274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b75361ec0073f1728c7bbc9fbf5e55f5ffc978176453aaccd3f3097a710904`  
		Last Modified: Wed, 05 Oct 2022 00:59:16 GMT  
		Size: 3.1 MB (3103607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d808aeab858717abffe76943dbb23ab89d6827acf98659287d2dbcae10de6802
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38192254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a93a8359bad558c79616802989335bad753382066c99091bc80472e1449812`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:29:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:29:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d5f59ce75940e1fb5b63ddc6afa84fc2256930712aa7e7290b055bfd5cb1d`  
		Last Modified: Wed, 05 Oct 2022 00:41:52 GMT  
		Size: 7.6 MB (7613905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e40ea3779e888d76ec1b65f3c196c09a8624d6c8fca71eb05d6df3e96bbcb68`  
		Last Modified: Wed, 05 Oct 2022 00:41:52 GMT  
		Size: 3.4 MB (3386727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:06975634dafaf93c307495697babcbab0110d23547c8fc4590dec336dfcdce07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46456747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb899fcd86d207ffe8e8e6cccccf6fc5aae8b200d5d0094b196cf01751e8972`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 10:52:08 GMT
ADD file:75224b75d955b3021df8214497d6835e1aff42b5ce83f96b779b63c4a8e15faf in / 
# Wed, 05 Oct 2022 10:52:10 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:54:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:55:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ecaa0fe591301d50850e37b61a6fac5429c04a3c39272da2f7b748eaed7f5c52`  
		Last Modified: Wed, 05 Oct 2022 10:54:26 GMT  
		Size: 33.3 MB (33296076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd13e27b4ef16e3a4f1fc7d6784c100856a30934614492936f7f8e802610cde`  
		Last Modified: Wed, 05 Oct 2022 19:17:43 GMT  
		Size: 8.7 MB (8704507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2eb56e07e0b2a6f0fbdcee055221848b0c5384a68adb4e6e1c38537aa1894`  
		Last Modified: Wed, 05 Oct 2022 19:17:42 GMT  
		Size: 4.5 MB (4456164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:03f6b7e0468f3a039213527067a008db1cef213244a75d3406a175aa2d68b215
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34113041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629e46285cd96bbf2061784773e791fccde26297e92c9cf51561f276b3c6fc5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:12:13 GMT
ADD file:8c408c11e1eeed71fdd784404ddf9ac52b700161e6187e2313c2751d756e3442 in / 
# Wed, 05 Oct 2022 00:12:14 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:43:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:edcdeceb0859700b9f2e87516c30c0049092e29666696c30e6b862e0df3d4961`  
		Last Modified: Wed, 05 Oct 2022 00:29:16 GMT  
		Size: 24.2 MB (24242839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750231dc28469e93ce7c6e7d14be0b30332503e15a9a7516729ab0815bbeb749`  
		Last Modified: Wed, 05 Oct 2022 03:42:06 GMT  
		Size: 6.7 MB (6725280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3455cf9ca9db352ee4e1bdf9c1bd8bd85713203a5b2ae128f9a7d02af28fea50`  
		Last Modified: Wed, 05 Oct 2022 03:42:00 GMT  
		Size: 3.1 MB (3144922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5a7f851b281d0a8383ebb5d105e975aebc9a7f0a0af82f5c0fefd30c6893c8c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37985034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a54e3219d44697978850492168a60aa1b203ec6eff40b2f9dcbc3af8e1aee31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:52:44 GMT
ADD file:f82ae9ee8436728ac9abdb4af38412611ab80a6dc434a66f2acd4f531df16e41 in / 
# Tue, 04 Oct 2022 23:52:47 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:18:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:18:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:55110f99e16edd33cca5c8eacd76396b8cd5660b1e57a10cbdea2b85f8c1dce5`  
		Last Modified: Tue, 04 Oct 2022 23:54:22 GMT  
		Size: 27.0 MB (27044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d458cf1a38d357dac5ba50202b285fecb19e5b69bb0d829213e080855b10460`  
		Last Modified: Wed, 05 Oct 2022 00:34:44 GMT  
		Size: 7.4 MB (7397444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5e08d5df1e8833e029f15faa3eec8852f7c8857e7d9a8f8ba37b23335843bb`  
		Last Modified: Wed, 05 Oct 2022 00:34:43 GMT  
		Size: 3.5 MB (3542720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
