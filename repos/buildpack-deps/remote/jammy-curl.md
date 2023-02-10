## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:529f22a39ce7033647bdc06ddae1d1ef6c4fbed46078824eba2550a58624f19d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:jammy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f5e6509df320f7774bd73272759602386e5d645fe971116c7dbed0f38e5fdd9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37778730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2441c30f4b69d5096de28028237f2028653245ec5675b95f2d0ba43db75d04bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:48:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec15466900398b5d701c68ab4f91684333cee7a531fee222d5fcb8a8a7b20d`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.8 MB (3788240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91ea6918177a2aa7ef5f879923eaccfb2e1ddaca74cc714d50e7132ffe71309`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.6 MB (3561486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a35738e183ce48bf2a3accbf8c23c84f5906743684d156e7e795e38cbb8df0e3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34274768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b94e1000749d94d59108d4594c340236e2fc54f20acc42fea2656601f2468bef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:58:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d0210273e3495988f639f6164118a5bba55666799ba86ac3e60a001cf7be3b31`  
		Last Modified: Thu, 26 Jan 2023 18:27:33 GMT  
		Size: 27.0 MB (27022323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf8c983748e75df464cf82dd94773e444405eb78ac8a28682a768205b5831f3`  
		Last Modified: Tue, 31 Jan 2023 18:16:29 GMT  
		Size: 3.5 MB (3539123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03d1b1bbe92d48273b3f90d94b0757bbc7f6b57061458b0fef417e2f6ff372b`  
		Last Modified: Tue, 31 Jan 2023 18:16:29 GMT  
		Size: 3.7 MB (3713322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:32acc0bceb4b1c5c72adca26c93d797456c8c103acfbd50cd2eda82ee7dbb3f9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35683834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bdaf7c5d9feef034d451541b098820f1836d948fcfe9d0503d7eecc5f27526`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:19:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:19:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157508d48eacd7b747f0b9c99ce627da62dd75af25ef8cae0d4a18512f51295`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.8 MB (3761409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53567c3f9bdfe731ccd25b9ed68fb667d0fcde2958e4503859e5d2ad3373d169`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.5 MB (3537451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b739e985cfa01beb77701e6fda59cbee4cac87054300d98a262a007bc00307fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44205386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f056e39bef72c9a8e678fd7d9cf620857f579ef83f6b5249fddeb1b5edaec956`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:53:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b919bd9d6c8a596b3ac4fb9ee1cc6727efdd1f1b05e5c130efec5deaae53ae60`  
		Last Modified: Tue, 31 Jan 2023 17:52:02 GMT  
		Size: 35.7 MB (35708930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59507b6d89bb36f24882056a420b04435132767ba96bd9396f58bc20ed960488`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.3 MB (4261748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc075be4c307553b270bec14a982c75e55b12a8be0e1232b459d394d27745b9`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.2 MB (4234708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:64c9f347cc5b6931002286f26b60966f7c186b2cde74c1a07cf6a9fbf4d4377d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35906690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e80805a3881c6a17e1e4319a43ce51e28dd9e4c9c2d2fe2e6264526e9a854082`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:42:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d244ff6bc0f1d8aab1af2badfb1f1ea2f619ca2316288c519afed909e08b35`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.8 MB (3792000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165dd3ed55b51c4b79b3be0051fe345d5b7e6bedbac65941ff7793e50e07420f`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.5 MB (3472764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
