## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:4c257540388d8f475a1c36cfdb813fab9d57d75b2f8398be8ebbb750e11325ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:kinetic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0b2551248f1086732d36906ec7f55149069008c97869777676f03ed76a21d013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41677694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408d82ec57f366f2c54c2b25f4d36a1a598859997e84bb91bb75934e52bcbcac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:02:32 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:02:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:02:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:02:32 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:02:34 GMT
ADD file:f8bb312bf73c62343d91c9988d58945c5d0fced3f559b95c4dd21a19183d933d in / 
# Mon, 05 Jun 2023 17:02:34 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:42:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6cee4c55bd500a2c4a00a5b79538d4485726955d83a652dd23d53199e149efe2`  
		Last Modified: Fri, 16 Jun 2023 01:55:57 GMT  
		Size: 27.5 MB (27488513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6b0fb7f48d56947f4fb88d70beb688a4862300af9ea9a03aa6ebadbbe71f7e`  
		Last Modified: Fri, 16 Jun 2023 01:55:54 GMT  
		Size: 14.2 MB (14189181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f9d2ab3a6b2bfe19700d9a81e7879a756852897bb7e69ef593327222d0ff7a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39055297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b81c8de3b061bbd76bd5c96119fd3fdc21ae5a2825a6be253a88d2827b1adaa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:04:06 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:04:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:04:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:04:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:04:15 GMT
ADD file:615be72e62c21704af356d6cfd4e32a7df8dd4b93d0c3ee3ea2e1641127c54ea in / 
# Mon, 05 Jun 2023 17:04:16 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:45:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4bf34fad731c68e9e2b3f1ab9be267f88256224d876e0b36cd63ff42fe27225a`  
		Last Modified: Fri, 16 Jun 2023 00:58:56 GMT  
		Size: 25.9 MB (25914047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d88eb5459ee9fba90e6dc257e7e3002bdb40e23d679a15bf566ec317a366bb`  
		Last Modified: Fri, 16 Jun 2023 00:58:55 GMT  
		Size: 13.1 MB (13141250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d896a8ffbf96431c2e3625e5c0bf80b26d5575151162818bb96feadf987a21b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.5 MB (40454569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc7a6b4a947b78e2024599c7ed9884c9c3dcf7e77d3da0c19bd9593ca6f8ab4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:02:45 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:02:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:02:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:02:46 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:02:50 GMT
ADD file:b85182b4593c262faef116755e01baa608e8090e1cb697d735485ff0bd5b353e in / 
# Mon, 05 Jun 2023 17:02:50 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:20:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d08ab8ea3b2755ec06aa9ce6972e64da08c79b30281c9416cac92b6aa23a7d8`  
		Last Modified: Fri, 16 Jun 2023 02:34:35 GMT  
		Size: 26.7 MB (26727371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11fa3a4a444d42bc471027a78d4e890bb44584c98f6160625eb80e66f566049`  
		Last Modified: Fri, 16 Jun 2023 02:34:32 GMT  
		Size: 13.7 MB (13727198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:afde62e2338b4677dcd7c066530ac56c757d0c71c72e0b8c465f19b02e31625c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f880f87ce67ddc9c97e45502bb7b7982c49ddaf7e2d64e4ae7308bf8b59a7387`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:10:48 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:10:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:10:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:10:48 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:10:52 GMT
ADD file:48c30fe281554302bb6533dd33a43a0877851ac5ba59dc3aff3d3d9ceae6f8a9 in / 
# Mon, 05 Jun 2023 17:10:52 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e97b48410348d002f0aaa3d5e7df14543cadcf78a962c446f311040094d1348`  
		Last Modified: Fri, 16 Jun 2023 01:27:17 GMT  
		Size: 32.1 MB (32102208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf4d9ebe87a9f4a30cb3454f9146c64bf5f745c3afc33b5ef9066928de29bc3`  
		Last Modified: Fri, 16 Jun 2023 01:27:13 GMT  
		Size: 16.2 MB (16234116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:862409116dd6f88091fb63263981bdf73ea2710a45b847a8d15ca350f8fa2a3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40386032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c248d7339a9978200db26fe6ece5bf19a87a09faa0cb0db10982d373481692a7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:08:08 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:08:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:08:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:08:08 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:08:09 GMT
ADD file:df5733230d0258ecd0cbdcc7c2075865bc335200f2cafee8dacccfd082710b96 in / 
# Thu, 13 Apr 2023 13:08:10 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 23:46:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c450971bf0fd92eac91caf0b3126482e5fecadead22e59da08f9661a4b4f03be`  
		Last Modified: Fri, 14 Apr 2023 10:00:19 GMT  
		Size: 26.0 MB (26029287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f712e29cfb9c4e3fa37cc777de5ec3a547378889617b0615c8957c5af9efdc`  
		Last Modified: Tue, 16 May 2023 23:56:45 GMT  
		Size: 14.4 MB (14356745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
