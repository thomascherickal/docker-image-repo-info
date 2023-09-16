## `buildpack-deps:mantic-curl`

```console
$ docker pull buildpack-deps@sha256:b92247731f35c035c0d92cb7d6ccefb8378cbcfb5234b3257a5b4b8f6ebda2eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0690e8271400b2b84cdba67300aa4a0b61f6cadc99a59d26fba8b92a6484b754
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41973099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b709ebd2d56ad6b5bab1049d0842645e6f85ddf5960c005df816942b7475a65`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:44:28 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:44:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:44:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:44:28 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:44:30 GMT
ADD file:3eab7cbcee278ce63f29f9808cb781d2eb15c0ab34d32a3a96af0299bd7f8f57 in / 
# Tue, 12 Sep 2023 04:44:30 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:19:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de5bd8f63131b365a8b75ce84fcce99e78eb1a16bace032fb6b3436580aa3be5`  
		Last Modified: Sat, 16 Sep 2023 02:23:58 GMT  
		Size: 28.1 MB (28086986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d50b023cfbb59919320bc1707382e1cc5a96e00f043ae469ddbfe2aaab4c8b5`  
		Last Modified: Sat, 16 Sep 2023 02:23:58 GMT  
		Size: 13.9 MB (13886113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8f3a1dee32da0ae79df39f2642527bd4842bdf7520ca151267f5ec06cb2533e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38781152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3824b185896c1d76344218662b8ea0fac5a4f85ce613db6ec96c4318fb9fa95e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:51 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:52 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:57 GMT
ADD file:3b10dde790011a91258183d8ef7e8ed5e24986b2296e00417509565fdfd45e31 in / 
# Tue, 12 Sep 2023 04:43:57 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:43:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:901b7210b5b59d80ecd06f3107fe68dbe84f1a47ffd468aa90dd8894057f62b7`  
		Last Modified: Sat, 16 Sep 2023 02:49:15 GMT  
		Size: 26.1 MB (26068467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3b650c0e7bb6739dbe1082f6637079b42eebc467b66032c563599bf955dffe`  
		Last Modified: Sat, 16 Sep 2023 02:49:14 GMT  
		Size: 12.7 MB (12712685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a35f2e4c4edc26122cc7bb48671b725f5a138f38dc2e50c2d42f9451929c78af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40711601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771f90e63f543f31666dfce56d1c86c2da9dd775b4b77dd0501323e9ec8264b5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:46:07 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:46:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:46:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:46:08 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:46:15 GMT
ADD file:e7975e06b9483ac7786a825720e46167975054bca8b0679a3c001d143c325fbc in / 
# Tue, 12 Sep 2023 04:46:16 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:08:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8e30ad94028d16a73ba211f5c6c54cc5246b12575575b6c44c6c55b6f331994`  
		Last Modified: Sat, 16 Sep 2023 02:13:44 GMT  
		Size: 27.3 MB (27318189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb011cee5097836afefa9b1443d4ca56b7a28b4181bbba91dbe5f98c84c81a49`  
		Last Modified: Sat, 16 Sep 2023 02:13:43 GMT  
		Size: 13.4 MB (13393412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fe0bd580624852293b9c42c5c30fb115640c5dd387adc97bbf1d3fb51fbbfdc4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48305950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3b26e75da14484a514efa511e46edd95f4dc2c98a88162a0fda08e3314f7e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:47 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:50 GMT
ADD file:56d58cbb4273b81f0c1a0b6eaede82f6a7e5d79c78d54525361f0537566dc9ec in / 
# Tue, 12 Sep 2023 04:43:50 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:42:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd229c9aa7cae185d030f835d891646d81b863cdb9cb773e41f12ee940228d28`  
		Last Modified: Sat, 16 Sep 2023 02:50:16 GMT  
		Size: 32.4 MB (32367087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec9bbd29feb8adb47adfbfa6309c9d863f2e8ec5f80cf30563f27da97167973`  
		Last Modified: Sat, 16 Sep 2023 02:50:12 GMT  
		Size: 15.9 MB (15938863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:16b08c68447ece99161a3fc8ac1f810e1735cb0f687c914605fd843885e5bb32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41711254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d62e4cb304e230bfe9ef92a078c9ee886fc8a24a29add2c9bcc35ff793bbf029`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:45:06 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:45:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:45:08 GMT
ADD file:6724cd2c23f7ec57f0524a81125b059327cf367ea1f3387b48c3f642bddc82b9 in / 
# Tue, 12 Sep 2023 04:45:09 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 01:50:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac93ca815ee057f1083e81c9edcf7787c1047a557a07ded971abbb05fa515ca0`  
		Last Modified: Sat, 16 Sep 2023 01:55:18 GMT  
		Size: 27.5 MB (27458487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939194dd385d3eacfbb7f1bf5b9dcc18c16873f21f0cd06b02cceb11343c00ed`  
		Last Modified: Sat, 16 Sep 2023 01:55:16 GMT  
		Size: 14.3 MB (14252767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
