## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:dbba68715899748e496e12c3807632c13e05ffd80b651787b7c5154d77340eb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:41592dd1e67dbffba26634f00619f5da6af28bfaefed9cf9475afdaa03acbf6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85728568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37fba109e84f956fa8db5ad6c4f1d621aa0184f493c6f92c176ecf3b10843533`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:47:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:48:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc37bca66e7c29e0d65a4279511fe9a93932a4bb80e79e95144f3812632b61a`  
		Last Modified: Fri, 16 Jun 2023 01:56:54 GMT  
		Size: 27.6 MB (27612943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7beeb5a79f9bd13c90ee4c9f68636fc642df773adb1bd04e27e2115f6c12a6d`  
		Last Modified: Fri, 16 Jun 2023 01:56:52 GMT  
		Size: 13.7 MB (13744092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a98e278987c0da01adb1f6145dec78bd526ecc11c227e2e74c48de9cd72c40`  
		Last Modified: Fri, 16 Jun 2023 01:57:09 GMT  
		Size: 44.4 MB (44371533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5a6012c64abe5a1e4977712e462e6802d4c5e7a02f2030a15e71b72ff3dfe57a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86748441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23973e09ff69a4949c38d23ac559b76967b561c2e71a9c4d1998f800fc603a88`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 00:50:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca5128fe76949cc104af7f40ce0f7213fe093079077d47dd525fa0189090c57e`  
		Last Modified: Fri, 16 Jun 2023 00:59:51 GMT  
		Size: 25.4 MB (25432780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d8ca764d56bdf14c46fabd5c4e2e988ce166d01c8c0631d7c345802ace7bf1`  
		Last Modified: Fri, 16 Jun 2023 00:59:50 GMT  
		Size: 12.7 MB (12662932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b3e8b607724476a55e2e23faa2859f1e37c17323d12df2f9b87de3745b98e3`  
		Last Modified: Fri, 16 Jun 2023 01:00:07 GMT  
		Size: 48.7 MB (48652729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f4b6f4db12ef63968941c8377fa0e0c0bcee84d18bdd0a12614b41b634f32314
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84580504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14bbc99976613f7010bfbffe01cff6a9c09074f1d54233d81f2928fa1eb6bfa6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:25:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc6a8da5865fc488969148ca6c503307bba4023ecc0cdceaaae76a8b9852f031`  
		Last Modified: Fri, 16 Jun 2023 02:35:25 GMT  
		Size: 27.0 MB (27029986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8dde3bba356efbb171daed99ec516dc5c5c9a9b19d538fcb9fd0031bd92403a`  
		Last Modified: Fri, 16 Jun 2023 02:35:22 GMT  
		Size: 13.3 MB (13333143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a9f35a1267eac739bb82daa33daa3a21960fb88acbc2177a8156f23b857239`  
		Last Modified: Fri, 16 Jun 2023 02:35:38 GMT  
		Size: 44.2 MB (44217375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c5a83ab3770b99e11c2b4445afb7ee1d926562a534194746e3288c6e0f2fc9b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96926153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c299a6b52971b8d036a8ccadd60c639e7831b2c4f677f2882df75e523a441b7f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:12:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a58a0b662b0d4d5e271c7c17f35795b5782a33c69a079e473f7c2303bee50024`  
		Last Modified: Fri, 16 Jun 2023 01:28:52 GMT  
		Size: 32.0 MB (32010412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6f165de89ef5a3a93777200dd180f02a8fc30051f7eb6267300a3e6f27ae1e`  
		Last Modified: Fri, 16 Jun 2023 01:28:48 GMT  
		Size: 15.8 MB (15841962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06312954ebad2b0995222a924fae1923e9b3c87aa73ff14beea981d9235b706d`  
		Last Modified: Fri, 16 Jun 2023 01:29:15 GMT  
		Size: 49.1 MB (49073779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1b75cd39b4b8028add596e3133c70e142effd651127b61c8b4819a154a3f6eb4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84499950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbb05763b63f79a573454ce88736b2c772cce3080193c277b1e194c26f5597d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
# Sat, 17 Jun 2023 09:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 17 Jun 2023 09:54:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:761ebd2058697796f2f98019cecedb81ef33759e6c1ec5a428e5bfcc3fe17d92`  
		Last Modified: Sat, 17 Jun 2023 10:02:12 GMT  
		Size: 26.2 MB (26245344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36084a86fb1b20f414b56d87cfcfa6dbc269df581ae9079da63a5c20f292984`  
		Last Modified: Sat, 17 Jun 2023 10:02:10 GMT  
		Size: 14.0 MB (14005266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9be9d6364c4e6a0cc7388e754f4dea89849b8149102ccc37c8849f51879091`  
		Last Modified: Sat, 17 Jun 2023 10:02:24 GMT  
		Size: 44.2 MB (44249340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
