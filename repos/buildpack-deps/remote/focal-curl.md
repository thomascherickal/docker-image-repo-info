## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:9d3fae6f15dc199b90dab2709e4836ff51fb9c713d983d791dbda48e7fb1eb9b
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
$ docker pull buildpack-deps@sha256:b1bb273927172a3307daf2e435ad3eaedac707b52aed1a80a6559b5045aa918b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39966612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699ca4594065556769c48f4df863439f7854e2dc3d247de1ca0ef27c44f306fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:43:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d2365e1e08bb86c1668a76475087cb6db5b42ba70cff99e936b0dda67d9215`  
		Last Modified: Sat, 16 Oct 2021 01:54:19 GMT  
		Size: 7.8 MB (7774998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c425bc29205ed0c522c9332f7199d4e5805576b76cfa97ff9e345cdb268a5`  
		Last Modified: Sat, 16 Oct 2021 01:54:18 GMT  
		Size: 3.6 MB (3624513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:96fc46fd8428121f4cba8731f07c3d2b0477826da21811e89ba2facff69b90c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a44a4a803282848534fb0e2b5a618208d8f0fcfaa6918c8c5021e765bc45ea6c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:20:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:21:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366ab467c7f452a8e5cb76b5ed3c9cbce43f7cb04f7024c6478ca446f92e399b`  
		Last Modified: Sat, 02 Oct 2021 22:38:21 GMT  
		Size: 6.8 MB (6766828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d36dec707683a0afbc780af0a45ca17744ac7a0f640d578af3195478d90621`  
		Last Modified: Sat, 02 Oct 2021 22:38:18 GMT  
		Size: 3.1 MB (3103932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2fb36e233ead75cc8b3a9e8a7feaa46b31ce507f9666246b82975f177db2bb7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38408082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da02243d8b4488513cd7351f2ebc075c8db8b4098ee398a79e228a8f2a72b20f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:17:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689db6ff62963b3e4aae6a2abb554c5d5882b06774174e624ba845094921121b`  
		Last Modified: Fri, 01 Oct 2021 03:25:21 GMT  
		Size: 7.6 MB (7635218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f06ec2d3b194d9726a65c75b82d7339dc700bc20d923f047e02a735a78925`  
		Last Modified: Fri, 01 Oct 2021 03:25:20 GMT  
		Size: 3.6 MB (3600459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:eef3c0a41f6cfc83f7c300350cc0da51c3d3185a17d758edbcdc8b4e2b6c3ccf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46471758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c8645449e8182a2157126f6b3219cb1ec8436d8919a30c6ef1e8eff0cf511c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b70bd5d2bc58b580d50736dbb70b528bdcd2910275584c8774c52efd29b8838`  
		Last Modified: Sat, 16 Oct 2021 01:29:38 GMT  
		Size: 8.7 MB (8728083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e49a7fcde36f5b4cd0c87bace3ad307d0709d6942ff3ec27c5090922c1c7c`  
		Last Modified: Sat, 16 Oct 2021 01:29:16 GMT  
		Size: 4.5 MB (4456437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8102a47411513107d38819cf1c50c53a59b006b8758ef1760d08cf6ef9189d53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34121525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81fb5dedcf54f0770eebdd37611586bf30053249c901ae7232aa30b16ab13d82`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:14:21 GMT
ADD file:9e85e474b240689ee9bae50d5101df1d6128c335d61a8010cd69202f778a773f in / 
# Sat, 16 Oct 2021 00:14:22 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:55:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 00:56:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:828cfd0a7a30e2a8cf76cca67b8314a0738943c0ea83f167ea5b8bd084c19324`  
		Last Modified: Sat, 16 Oct 2021 00:27:58 GMT  
		Size: 24.2 MB (24226165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acf80d7193afc4761abdd46a164fd3130cfdb676ff3801645cb819e88404dad`  
		Last Modified: Sat, 16 Oct 2021 01:28:59 GMT  
		Size: 6.8 MB (6750726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab037bb968a07aace1a589724d7eb8ec30de3a596a4227fa9fc39de318067cb`  
		Last Modified: Sat, 16 Oct 2021 01:28:54 GMT  
		Size: 3.1 MB (3144634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:df2267e8f1ad540996bba096ece6a0ac191843ccd329f8acea0b78f977e3433f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38091428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f3fe3fc44fce5558d3d6596b6c1c62d958ff8a740b249bcb858c65f15c905f7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:09:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe453f45d32c58639c70b42127d12e8467533bc152ff663c5ffc8d0b5407293`  
		Last Modified: Sat, 16 Oct 2021 01:15:04 GMT  
		Size: 7.4 MB (7428503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df987c93c7f716b8ea845b480a00ccf4e4d962df89ed9f8cbefecdb1d9a96cf2`  
		Last Modified: Sat, 16 Oct 2021 01:15:03 GMT  
		Size: 3.5 MB (3542069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
