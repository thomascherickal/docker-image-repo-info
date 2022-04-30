## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:32d1dd0f704fb18290c6704e7b66241a944e922b9d23a3d68ccc3657016b68cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2f451ee6c634890fe901fb4c3e9f906e68750c4e9d94265be701be0a2d67ed6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77145823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eb4460add6a291c8cd6fc0bfb0ec9d2a3df158318fd81d9f53f135a1bc25fd0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:15 GMT
ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / 
# Fri, 29 Apr 2022 23:21:15 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:55:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:55:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:56:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:125a6e411906fe6b0aaa50fc9d600bf6ff9bb11a8651727ce1ed482dc271c24c`  
		Last Modified: Fri, 29 Apr 2022 03:03:30 GMT  
		Size: 30.4 MB (30421006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd42456788d884c562de4649973cbad0ff15b20c71bb817db73e99ba659bd98`  
		Last Modified: Sat, 30 Apr 2022 00:03:38 GMT  
		Size: 3.8 MB (3818745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eaf54bac42fe111f77299f5bf651ebd4d872700f461e671a8051862ad6f875`  
		Last Modified: Sat, 30 Apr 2022 00:03:38 GMT  
		Size: 3.6 MB (3559366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b6559f8defc073df8df9cbbabbe0ded1ad2d1eb31b9af9bbf6a8c5152af04d`  
		Last Modified: Sat, 30 Apr 2022 00:03:54 GMT  
		Size: 39.3 MB (39346706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b7e1fbbfbf5e1bf5c8db230aaf94aec1d34933d23ba16c8fcb803b2a5cc64cf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76194989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5444563afcca99567b8ec3ce461196208eee4f3942adbe6cccf61ee8959b9f1c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:30 GMT
ADD file:78ae02cb00d8cc788584388eeb9fdc5ca6b45f502d33acd7f6efe7fc2a325683 in / 
# Fri, 29 Apr 2022 22:59:31 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:35:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:35:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:36:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a3411c136d8a6da4e9d7d3abcbfc94f59ecb2935fd02cad49be6a79c899fcaa`  
		Last Modified: Fri, 29 Apr 2022 23:03:59 GMT  
		Size: 27.0 MB (27015834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0fc400254e500236c1a1555f53101f3d136a6466afc02b601d41b663424039`  
		Last Modified: Fri, 29 Apr 2022 23:53:01 GMT  
		Size: 3.6 MB (3569862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff75e9c518264298a148cc4e8d868ef1588d3fbb3eb5a8f37dbc41d393fb89`  
		Last Modified: Fri, 29 Apr 2022 23:52:59 GMT  
		Size: 3.7 MB (3712399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac2f30de9b874657871112606d8d66e7b11892765a38c6fb72a160749dd932f`  
		Last Modified: Fri, 29 Apr 2022 23:53:42 GMT  
		Size: 41.9 MB (41896894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3a4a573a0f2b394c1234babc465c1b7e358c4ae8aa2678aabb19ae3ed78840c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74728136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1429ae55904367c85441c4feee2219f525b6277aa3317cdc60090bdf19c2f24e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:19:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:19:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:20:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4779269ba0c40d25a7dc0dce21c857eb6326260eef418a05d8f7ebca0f0b7c52`  
		Last Modified: Fri, 29 Apr 2022 23:27:13 GMT  
		Size: 3.8 MB (3792535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc5ea7b81dce7b5d5da0ca011f59cd030d00e4c8bdb15aa0451b41aa695a056`  
		Last Modified: Fri, 29 Apr 2022 23:27:13 GMT  
		Size: 3.3 MB (3319229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3d8c61d6e5775325116e57598d0ad92314ae8bb75cc2eb561c9d3d005f7e66`  
		Last Modified: Fri, 29 Apr 2022 23:27:30 GMT  
		Size: 39.2 MB (39239915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:6ed58de963d72b45c1173945e36680a1f217194c949f257b12e94f08518e7cf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77227636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f525c57b0baa0f25153f5ce2ddce02252cdcede35040483baeea9bbc1f10f5e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:18:56 GMT
ADD file:7350517b53b7fc7556b4df07b2d762e16a9797b68f4760d536321210c8acfd34 in / 
# Fri, 29 Apr 2022 23:18:57 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:55:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:56:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 30 Apr 2022 02:00:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29912c87e17183ec23ae82771552de74ad581040d14b5d35e5678e1409ca9a66`  
		Last Modified: Fri, 29 Apr 2022 23:41:25 GMT  
		Size: 27.7 MB (27745174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357472d7f5fad9e88f737e2eaf5af11996df0615a3239cc506b47a53c3d986b1`  
		Last Modified: Sat, 30 Apr 2022 02:44:49 GMT  
		Size: 3.6 MB (3613486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e941a43a509b50d722053f1978e0c0e3fc1c311feb97823962b6ca49e790bc4`  
		Last Modified: Sat, 30 Apr 2022 02:44:47 GMT  
		Size: 3.8 MB (3776674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd2a0b1302b67de2ce7b8af1cd3b4d8bde5865b94535059a1ec4ab20cfe34b0`  
		Last Modified: Sat, 30 Apr 2022 02:46:57 GMT  
		Size: 42.1 MB (42092302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2504c60bcb8a407b522753c08d872ff640df9285c0e1513f5ca9a73ed3c1b466
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75200999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37cd66855073b128b8898f80eaa4e0479ed5cc32d7a6af1492dd59eb97c5c598`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:31 GMT
ADD file:f64deb7af5cd28d502c52ddec5392a74b3a97eec2157bb03a4c0422eafb13c49 in / 
# Fri, 29 Apr 2022 22:50:33 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:14:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:14:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:15:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8346d310386430a355c4f3bd23e20115298043169165d7b84d92e3233b6696f4`  
		Last Modified: Fri, 29 Apr 2022 22:52:24 GMT  
		Size: 28.6 MB (28637232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e3da9a8d3319d0121a79a6e6c433b298c51996b294808f5718b06ec206c38f`  
		Last Modified: Fri, 29 Apr 2022 23:21:08 GMT  
		Size: 3.8 MB (3821153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad36c963048b206a25d408e23b027027eda701e952c4b1495d5eb264b7916b5`  
		Last Modified: Fri, 29 Apr 2022 23:21:08 GMT  
		Size: 3.5 MB (3470533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b546bcbed2ba04a55610966e92af3558dce4d18ca539204c04ba8aaf7df7529`  
		Last Modified: Fri, 29 Apr 2022 23:21:37 GMT  
		Size: 39.3 MB (39272081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
