<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6.0`](#spiped160)
-	[`spiped:1.6.0-alpine`](#spiped160-alpine)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:f13723692b09cb16472b7385bcd6682310f42d55eb20afc3a6fa0a8aa35347e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:d7a527e63589d1c652349e10175e2a12410746fd315ffc22f049d68daa817703
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36250037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47598dabed088d23163d926cffc0dadc0d4ecde1121b8bba28ea72e5d6b51503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:24:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:24:08 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:24:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:24:43 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:24:43 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:24:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:24:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:24:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203702656f2bc38f30feb84f231409c6410c791f7cdbfbfbfced0542a244a0fd`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557fe75836e921d1614d4851bb548ea1c3461fd961fb1da808ecfcd64be0b783`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 2.1 MB (2128038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b46de8c6821819710736655000293f13ccd254c856c530ceb0284fd5bce051d`  
		Last Modified: Sat, 28 Dec 2019 15:25:05 GMT  
		Size: 7.0 MB (7027553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19abe18c9a99d59f8232801356dd34ef508a3ad98b3a9882942c72b57e1fbe28`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408ec0d81452b12c37407b4241dda1c7ceba349382dfdfa0a6e567d86fe325bb`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:f34e16bf7e1eb0e0ea66e777125e22a48addc445a562e779ea560c06027e1b81
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32143608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c98047f88a0ccc7bff1e53ba518e9151969fd8976b360ddda3d343c57d27e4fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:26:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 07:26:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:26:29 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 07:26:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 07:26:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 07:27:36 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 07:27:37 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 07:27:38 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 07:27:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 07:27:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 07:27:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c6e24c6e8419c0af6f6c6ab83019bbc2f0a11b6d859a39a2ab68804c7370c5`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7861630cbcb98d5220dc36843f7ccaa064bf7eeec94be5fb17ed5fc6cfc5ef78`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 1.8 MB (1839099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574a0ed773473e94c320b2f5b76c37b05fbbfa110ccf92ac273fe40835b8b3cc`  
		Last Modified: Sat, 28 Dec 2019 07:27:55 GMT  
		Size: 5.5 MB (5472684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335610f863ed9990600eba791bdbb9d06b5fff1adab04f447b59f2fc17114f3d`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a48dbcaae96bd7d53f5e3d7639aa585d05a3296e80215e2bac3360e39fe2a98`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:53546fd0ca5d9265f674627303daf9879bec4c478c7182dfee9350c7b9f03aa5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29739828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c544d9f76a3ab23c1a2e6b2d2c97fbd476433e5cda4706e1d75c9aeefadf551`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:30:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:30:20 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:30:21 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:30:22 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:30:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:31:14 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:31:15 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:31:16 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:31:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:31:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:31:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44760daed9bd7e053b8359b083d503784b8fa54a77c2be7e30d6992f9ec11566`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb7b11245dcb2b9280aa470c53ab1a1c1a1d6b59a3e1b11fb4af3efa32b71c6`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 1.8 MB (1759411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e75be9243e45729cbf888681603e935380cb319ee933cbe62e04cf0f12e019`  
		Last Modified: Sat, 28 Dec 2019 15:31:56 GMT  
		Size: 5.3 MB (5279087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e21e4371b999ea9ceb6793cbdf0d7b62277493902b3b0cce605296e2b0725`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850b607025feab0f31b7bfb898db73bab4ae1550f20e614914ff2295de16a7de`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:857577271f4befe4d3940908e4ae2e29df85185549e0a66be4df985eeb34efad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33760061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6e33753196bcfcd1535f691816ec9552d18a610496600fc3c1d269682ea3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 23:44:15 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 23:44:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:44:29 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 23:44:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 23:44:31 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 23:45:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 23:45:17 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 23:45:18 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 23:45:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 23:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 23:45:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8e852ce6071469cdfbd8efc7e96697a6f1f922e0ea51eddf67ef538683a610`  
		Last Modified: Sat, 28 Dec 2019 23:45:42 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e089395518f54f3841e117bf0160c8e54e58cc3fa7dc98353a11d8368175`  
		Last Modified: Sat, 28 Dec 2019 23:45:42 GMT  
		Size: 2.0 MB (2007805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415fef10a74ca9dc337d9f82164c3d6d300ca4138a1eeaa1babb81c18b320a04`  
		Last Modified: Sat, 28 Dec 2019 23:45:46 GMT  
		Size: 5.9 MB (5899346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfd645d4631682b8972cbe12c69e7dde2998de3c4f8f06fbd9b7ea25499c45`  
		Last Modified: Sat, 28 Dec 2019 23:45:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f56e3d1ee35f83a66fd9c5ca9107877c87495f78c23b16af227d6761537b743`  
		Last Modified: Sat, 28 Dec 2019 23:45:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:168c95178154bb1e3007e51f9c910ad7367f73450309133a6a1118c0b5c6894e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41504389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad94098493589622565beb5945d14d25b1238995924d460081359a9eddc6084`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:28:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:29:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:29:28 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:29:28 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:29:29 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:29:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:29:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:29:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5610f5ff45f97f75a7401ce4a1463a61b9ea809bc4b2df4b665d1b45da7f4e44`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32baf55cd2c6722002eb93fa3674d090b634b070ef3cee2948c82f93f117813`  
		Last Modified: Sat, 28 Dec 2019 15:29:43 GMT  
		Size: 2.1 MB (2132343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d4d4973ad3c749629aeafb4d317e50d51b3640ae7541caeeebe8f170013951`  
		Last Modified: Sat, 28 Dec 2019 15:29:47 GMT  
		Size: 11.6 MB (11622861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea27042f3d808f9ac5fbbf880d4b0344b788f6a1c84ab9475ab3cd18da68a1`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2918b4236946a4defd9202282444263536eeebe1c328c16a8c13fa59150817`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:1f623139620f5efe999cada98454214e9ece9afb73c3c7c70a20b0cebda9e132
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d926a33940447f241bbb066c2ec28711bc72bc6ef44d99f397a55211384b1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:26:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 06:26:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:26:52 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 06:26:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 06:27:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 06:31:38 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 06:31:44 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 06:31:48 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 06:31:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 06:31:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 06:32:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091450b7ecb8270a51ff0d82376735817c4d2d385d6a2404ee013107ab169d60`  
		Last Modified: Sat, 28 Dec 2019 06:32:26 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65aa680f52e6e9c4e23d4a4d80ebd560e04ca6ad64ffd04a010cde7cee481a`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 2.2 MB (2224902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5855143d6300ec32dd6b565f347fbefb95f61d20885d15d07363e49eb626d4`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 6.7 MB (6735504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280634de8f8748bdfa29b62191c582df919e9c849d1d5db2d82550d90f055765`  
		Last Modified: Sat, 28 Dec 2019 06:32:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95975ac48caf88db370d8e9f77cdfdb86eb82619f0d90b3d3c2213a9adf3f2f5`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:c8daf96755c80cd357de141bdb2118039c7d16653ea1e6766bdce7192a2fa2f5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33462729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e91fbf5ad53569e17c34629a2c6ae58fba1d4fe5b93965b5c53737e730643b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:05:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 07:05:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 07:05:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 07:05:24 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 07:05:25 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 07:05:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 07:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 07:05:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feba1cae3e4de6c9427a36923d1a4b6fdf8031ad008bbb2df647367b5a13adc`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5262978a84c64bb67475a813823814a00f94cd72ec62dfce286c0e0a755ca92`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 1.8 MB (1821612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cabcb44320636e61a59dbbfdea90f4d0bd14aea3536aab7e2f64ebad5c94de0`  
		Last Modified: Sat, 28 Dec 2019 07:05:41 GMT  
		Size: 5.9 MB (5933629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7553f30f2a3addf74102dfd9c8e6abe4c552d8572e2b2852c3cb233676ed8`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a30a29355212488d05b8ba9665d991231e0d9626a5e9d4b3f048f1b489e017a`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:f13723692b09cb16472b7385bcd6682310f42d55eb20afc3a6fa0a8aa35347e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:d7a527e63589d1c652349e10175e2a12410746fd315ffc22f049d68daa817703
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36250037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47598dabed088d23163d926cffc0dadc0d4ecde1121b8bba28ea72e5d6b51503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:24:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:24:08 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:24:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:24:43 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:24:43 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:24:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:24:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:24:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203702656f2bc38f30feb84f231409c6410c791f7cdbfbfbfced0542a244a0fd`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557fe75836e921d1614d4851bb548ea1c3461fd961fb1da808ecfcd64be0b783`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 2.1 MB (2128038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b46de8c6821819710736655000293f13ccd254c856c530ceb0284fd5bce051d`  
		Last Modified: Sat, 28 Dec 2019 15:25:05 GMT  
		Size: 7.0 MB (7027553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19abe18c9a99d59f8232801356dd34ef508a3ad98b3a9882942c72b57e1fbe28`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408ec0d81452b12c37407b4241dda1c7ceba349382dfdfa0a6e567d86fe325bb`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:f34e16bf7e1eb0e0ea66e777125e22a48addc445a562e779ea560c06027e1b81
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32143608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c98047f88a0ccc7bff1e53ba518e9151969fd8976b360ddda3d343c57d27e4fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:26:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 07:26:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:26:29 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 07:26:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 07:26:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 07:27:36 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 07:27:37 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 07:27:38 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 07:27:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 07:27:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 07:27:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c6e24c6e8419c0af6f6c6ab83019bbc2f0a11b6d859a39a2ab68804c7370c5`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7861630cbcb98d5220dc36843f7ccaa064bf7eeec94be5fb17ed5fc6cfc5ef78`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 1.8 MB (1839099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574a0ed773473e94c320b2f5b76c37b05fbbfa110ccf92ac273fe40835b8b3cc`  
		Last Modified: Sat, 28 Dec 2019 07:27:55 GMT  
		Size: 5.5 MB (5472684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335610f863ed9990600eba791bdbb9d06b5fff1adab04f447b59f2fc17114f3d`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a48dbcaae96bd7d53f5e3d7639aa585d05a3296e80215e2bac3360e39fe2a98`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:53546fd0ca5d9265f674627303daf9879bec4c478c7182dfee9350c7b9f03aa5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29739828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c544d9f76a3ab23c1a2e6b2d2c97fbd476433e5cda4706e1d75c9aeefadf551`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:30:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:30:20 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:30:21 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:30:22 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:30:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:31:14 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:31:15 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:31:16 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:31:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:31:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:31:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44760daed9bd7e053b8359b083d503784b8fa54a77c2be7e30d6992f9ec11566`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb7b11245dcb2b9280aa470c53ab1a1c1a1d6b59a3e1b11fb4af3efa32b71c6`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 1.8 MB (1759411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e75be9243e45729cbf888681603e935380cb319ee933cbe62e04cf0f12e019`  
		Last Modified: Sat, 28 Dec 2019 15:31:56 GMT  
		Size: 5.3 MB (5279087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e21e4371b999ea9ceb6793cbdf0d7b62277493902b3b0cce605296e2b0725`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850b607025feab0f31b7bfb898db73bab4ae1550f20e614914ff2295de16a7de`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:857577271f4befe4d3940908e4ae2e29df85185549e0a66be4df985eeb34efad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33760061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6e33753196bcfcd1535f691816ec9552d18a610496600fc3c1d269682ea3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 23:44:15 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 23:44:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:44:29 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 23:44:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 23:44:31 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 23:45:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 23:45:17 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 23:45:18 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 23:45:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 23:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 23:45:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8e852ce6071469cdfbd8efc7e96697a6f1f922e0ea51eddf67ef538683a610`  
		Last Modified: Sat, 28 Dec 2019 23:45:42 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e089395518f54f3841e117bf0160c8e54e58cc3fa7dc98353a11d8368175`  
		Last Modified: Sat, 28 Dec 2019 23:45:42 GMT  
		Size: 2.0 MB (2007805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415fef10a74ca9dc337d9f82164c3d6d300ca4138a1eeaa1babb81c18b320a04`  
		Last Modified: Sat, 28 Dec 2019 23:45:46 GMT  
		Size: 5.9 MB (5899346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfd645d4631682b8972cbe12c69e7dde2998de3c4f8f06fbd9b7ea25499c45`  
		Last Modified: Sat, 28 Dec 2019 23:45:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f56e3d1ee35f83a66fd9c5ca9107877c87495f78c23b16af227d6761537b743`  
		Last Modified: Sat, 28 Dec 2019 23:45:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:168c95178154bb1e3007e51f9c910ad7367f73450309133a6a1118c0b5c6894e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41504389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad94098493589622565beb5945d14d25b1238995924d460081359a9eddc6084`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:28:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:29:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:29:28 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:29:28 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:29:29 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:29:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:29:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:29:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5610f5ff45f97f75a7401ce4a1463a61b9ea809bc4b2df4b665d1b45da7f4e44`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32baf55cd2c6722002eb93fa3674d090b634b070ef3cee2948c82f93f117813`  
		Last Modified: Sat, 28 Dec 2019 15:29:43 GMT  
		Size: 2.1 MB (2132343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d4d4973ad3c749629aeafb4d317e50d51b3640ae7541caeeebe8f170013951`  
		Last Modified: Sat, 28 Dec 2019 15:29:47 GMT  
		Size: 11.6 MB (11622861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea27042f3d808f9ac5fbbf880d4b0344b788f6a1c84ab9475ab3cd18da68a1`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2918b4236946a4defd9202282444263536eeebe1c328c16a8c13fa59150817`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:1f623139620f5efe999cada98454214e9ece9afb73c3c7c70a20b0cebda9e132
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d926a33940447f241bbb066c2ec28711bc72bc6ef44d99f397a55211384b1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:26:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 06:26:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:26:52 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 06:26:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 06:27:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 06:31:38 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 06:31:44 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 06:31:48 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 06:31:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 06:31:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 06:32:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091450b7ecb8270a51ff0d82376735817c4d2d385d6a2404ee013107ab169d60`  
		Last Modified: Sat, 28 Dec 2019 06:32:26 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65aa680f52e6e9c4e23d4a4d80ebd560e04ca6ad64ffd04a010cde7cee481a`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 2.2 MB (2224902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5855143d6300ec32dd6b565f347fbefb95f61d20885d15d07363e49eb626d4`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 6.7 MB (6735504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280634de8f8748bdfa29b62191c582df919e9c849d1d5db2d82550d90f055765`  
		Last Modified: Sat, 28 Dec 2019 06:32:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95975ac48caf88db370d8e9f77cdfdb86eb82619f0d90b3d3c2213a9adf3f2f5`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:c8daf96755c80cd357de141bdb2118039c7d16653ea1e6766bdce7192a2fa2f5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33462729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e91fbf5ad53569e17c34629a2c6ae58fba1d4fe5b93965b5c53737e730643b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:05:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 07:05:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 07:05:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 07:05:24 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 07:05:25 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 07:05:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 07:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 07:05:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feba1cae3e4de6c9427a36923d1a4b6fdf8031ad008bbb2df647367b5a13adc`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5262978a84c64bb67475a813823814a00f94cd72ec62dfce286c0e0a755ca92`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 1.8 MB (1821612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cabcb44320636e61a59dbbfdea90f4d0bd14aea3536aab7e2f64ebad5c94de0`  
		Last Modified: Sat, 28 Dec 2019 07:05:41 GMT  
		Size: 5.9 MB (5933629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7553f30f2a3addf74102dfd9c8e6abe4c552d8572e2b2852c3cb233676ed8`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a30a29355212488d05b8ba9665d991231e0d9626a5e9d4b3f048f1b489e017a`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.0`

```console
$ docker pull spiped@sha256:f13723692b09cb16472b7385bcd6682310f42d55eb20afc3a6fa0a8aa35347e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.0` - linux; amd64

```console
$ docker pull spiped@sha256:d7a527e63589d1c652349e10175e2a12410746fd315ffc22f049d68daa817703
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36250037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47598dabed088d23163d926cffc0dadc0d4ecde1121b8bba28ea72e5d6b51503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:24:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:24:08 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:24:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:24:43 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:24:43 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:24:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:24:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:24:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203702656f2bc38f30feb84f231409c6410c791f7cdbfbfbfced0542a244a0fd`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557fe75836e921d1614d4851bb548ea1c3461fd961fb1da808ecfcd64be0b783`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 2.1 MB (2128038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b46de8c6821819710736655000293f13ccd254c856c530ceb0284fd5bce051d`  
		Last Modified: Sat, 28 Dec 2019 15:25:05 GMT  
		Size: 7.0 MB (7027553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19abe18c9a99d59f8232801356dd34ef508a3ad98b3a9882942c72b57e1fbe28`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408ec0d81452b12c37407b4241dda1c7ceba349382dfdfa0a6e567d86fe325bb`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; arm variant v5

```console
$ docker pull spiped@sha256:f34e16bf7e1eb0e0ea66e777125e22a48addc445a562e779ea560c06027e1b81
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32143608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c98047f88a0ccc7bff1e53ba518e9151969fd8976b360ddda3d343c57d27e4fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:26:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 07:26:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:26:29 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 07:26:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 07:26:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 07:27:36 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 07:27:37 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 07:27:38 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 07:27:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 07:27:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 07:27:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c6e24c6e8419c0af6f6c6ab83019bbc2f0a11b6d859a39a2ab68804c7370c5`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7861630cbcb98d5220dc36843f7ccaa064bf7eeec94be5fb17ed5fc6cfc5ef78`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 1.8 MB (1839099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574a0ed773473e94c320b2f5b76c37b05fbbfa110ccf92ac273fe40835b8b3cc`  
		Last Modified: Sat, 28 Dec 2019 07:27:55 GMT  
		Size: 5.5 MB (5472684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335610f863ed9990600eba791bdbb9d06b5fff1adab04f447b59f2fc17114f3d`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a48dbcaae96bd7d53f5e3d7639aa585d05a3296e80215e2bac3360e39fe2a98`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; arm variant v7

```console
$ docker pull spiped@sha256:53546fd0ca5d9265f674627303daf9879bec4c478c7182dfee9350c7b9f03aa5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29739828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c544d9f76a3ab23c1a2e6b2d2c97fbd476433e5cda4706e1d75c9aeefadf551`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:30:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:30:20 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:30:21 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:30:22 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:30:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:31:14 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:31:15 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:31:16 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:31:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:31:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:31:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44760daed9bd7e053b8359b083d503784b8fa54a77c2be7e30d6992f9ec11566`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb7b11245dcb2b9280aa470c53ab1a1c1a1d6b59a3e1b11fb4af3efa32b71c6`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 1.8 MB (1759411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e75be9243e45729cbf888681603e935380cb319ee933cbe62e04cf0f12e019`  
		Last Modified: Sat, 28 Dec 2019 15:31:56 GMT  
		Size: 5.3 MB (5279087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e21e4371b999ea9ceb6793cbdf0d7b62277493902b3b0cce605296e2b0725`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850b607025feab0f31b7bfb898db73bab4ae1550f20e614914ff2295de16a7de`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:857577271f4befe4d3940908e4ae2e29df85185549e0a66be4df985eeb34efad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33760061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6e33753196bcfcd1535f691816ec9552d18a610496600fc3c1d269682ea3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 23:44:15 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 23:44:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:44:29 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 23:44:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 23:44:31 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 23:45:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 23:45:17 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 23:45:18 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 23:45:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 23:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 23:45:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8e852ce6071469cdfbd8efc7e96697a6f1f922e0ea51eddf67ef538683a610`  
		Last Modified: Sat, 28 Dec 2019 23:45:42 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e089395518f54f3841e117bf0160c8e54e58cc3fa7dc98353a11d8368175`  
		Last Modified: Sat, 28 Dec 2019 23:45:42 GMT  
		Size: 2.0 MB (2007805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415fef10a74ca9dc337d9f82164c3d6d300ca4138a1eeaa1babb81c18b320a04`  
		Last Modified: Sat, 28 Dec 2019 23:45:46 GMT  
		Size: 5.9 MB (5899346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfd645d4631682b8972cbe12c69e7dde2998de3c4f8f06fbd9b7ea25499c45`  
		Last Modified: Sat, 28 Dec 2019 23:45:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f56e3d1ee35f83a66fd9c5ca9107877c87495f78c23b16af227d6761537b743`  
		Last Modified: Sat, 28 Dec 2019 23:45:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; 386

```console
$ docker pull spiped@sha256:168c95178154bb1e3007e51f9c910ad7367f73450309133a6a1118c0b5c6894e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41504389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad94098493589622565beb5945d14d25b1238995924d460081359a9eddc6084`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:28:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:29:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:29:28 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:29:28 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:29:29 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:29:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:29:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:29:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5610f5ff45f97f75a7401ce4a1463a61b9ea809bc4b2df4b665d1b45da7f4e44`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32baf55cd2c6722002eb93fa3674d090b634b070ef3cee2948c82f93f117813`  
		Last Modified: Sat, 28 Dec 2019 15:29:43 GMT  
		Size: 2.1 MB (2132343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d4d4973ad3c749629aeafb4d317e50d51b3640ae7541caeeebe8f170013951`  
		Last Modified: Sat, 28 Dec 2019 15:29:47 GMT  
		Size: 11.6 MB (11622861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea27042f3d808f9ac5fbbf880d4b0344b788f6a1c84ab9475ab3cd18da68a1`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2918b4236946a4defd9202282444263536eeebe1c328c16a8c13fa59150817`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; ppc64le

```console
$ docker pull spiped@sha256:1f623139620f5efe999cada98454214e9ece9afb73c3c7c70a20b0cebda9e132
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d926a33940447f241bbb066c2ec28711bc72bc6ef44d99f397a55211384b1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:26:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 06:26:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:26:52 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 06:26:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 06:27:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 06:31:38 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 06:31:44 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 06:31:48 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 06:31:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 06:31:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 06:32:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091450b7ecb8270a51ff0d82376735817c4d2d385d6a2404ee013107ab169d60`  
		Last Modified: Sat, 28 Dec 2019 06:32:26 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65aa680f52e6e9c4e23d4a4d80ebd560e04ca6ad64ffd04a010cde7cee481a`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 2.2 MB (2224902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5855143d6300ec32dd6b565f347fbefb95f61d20885d15d07363e49eb626d4`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 6.7 MB (6735504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280634de8f8748bdfa29b62191c582df919e9c849d1d5db2d82550d90f055765`  
		Last Modified: Sat, 28 Dec 2019 06:32:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95975ac48caf88db370d8e9f77cdfdb86eb82619f0d90b3d3c2213a9adf3f2f5`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; s390x

```console
$ docker pull spiped@sha256:c8daf96755c80cd357de141bdb2118039c7d16653ea1e6766bdce7192a2fa2f5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33462729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e91fbf5ad53569e17c34629a2c6ae58fba1d4fe5b93965b5c53737e730643b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:05:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 07:05:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 07:05:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 07:05:24 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 07:05:25 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 07:05:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 07:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 07:05:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feba1cae3e4de6c9427a36923d1a4b6fdf8031ad008bbb2df647367b5a13adc`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5262978a84c64bb67475a813823814a00f94cd72ec62dfce286c0e0a755ca92`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 1.8 MB (1821612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cabcb44320636e61a59dbbfdea90f4d0bd14aea3536aab7e2f64ebad5c94de0`  
		Last Modified: Sat, 28 Dec 2019 07:05:41 GMT  
		Size: 5.9 MB (5933629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7553f30f2a3addf74102dfd9c8e6abe4c552d8572e2b2852c3cb233676ed8`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a30a29355212488d05b8ba9665d991231e0d9626a5e9d4b3f048f1b489e017a`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.0-alpine`

```console
$ docker pull spiped@sha256:088d5ea43f5f03d8f0e7f8d7cc7f408c051e96d9bf857a700813f9e7784df61e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.0-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:72e22523884276e22a39cb4ca1565ad39fb6d4022bbf8dc95c2ca971837d2076
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2874547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5651969446d1f1cc825c8b9ba7dc1e5801199fd64ed74c8d9599ea384919c48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:03:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 22:03:35 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 22:03:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 22:03:45 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 22:03:45 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 22:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 22:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 22:03:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f06f6c021497e75da7d87b6915a230626924c07991053d9a549fe400002cd18`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a4c78135aa6f75a6b5c923dada0201438e732b2ec25d5ae4be29cc120ca65c`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 6.3 KB (6315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e663e994236beda0de3f4f37acce0c41beca2e1aae2ba383534a5028103a5b6e`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 79.4 KB (79404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657a50cf15a9d8436f360d957ff17c290cef5b2a33dc2da440eccd93b5ad2f0`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e8488c4af15837a96b0fd48f4b5818da4056d3d8c253457edc7e915db76f42`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3ae91669334784f7b06ff519d1493b018d6b1946da07f9538b9ce403ba6a806c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66aceefd2fe95659d0e866344c41b8ab59a1f5edea0d9b102bcfb102808402ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 21:07:16 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 21:07:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 21:07:18 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 21:07:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 21:07:40 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 21:07:41 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 21:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:07:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 21:07:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ca77a0d6c23ca1ab7a1d6247b2f6058a74967635d48c6436eddb9c4ab9dc8b`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 68.0 KB (67990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecc30ce77974a56c9958f85075516bf23a4d87f452a99f0994ba66bbdff2b2f`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d253ce677e060437c999efb2094afda12da7234d44582a95187be47777394`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf6bfcf29967c12ef7c3749eefef9078bd45f60bd4c88f76c983108a3d464f42
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccadcaa5909aa00e88b17bf5880f652201851d3584c86fff7fcb9fa620424043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:56:51 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:57:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:57:11 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:57:11 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:57:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:57:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b88556cd7e307bd7aae61fbb97a5a495fd194bc5ca395dae82b60e890550492`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 61.7 KB (61746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb7e64f07324c2b74ff72e4b59b8a1693e42d453bf3e54a36e830699e3726c1`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39643304907003481036d0a383c8fc76114ab8f7ef02e7ae8513c2c1d30bfb56`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:20b57cf601ee060aeaf921435a00e6a82a6530d41dd56dcd9e39c61ff91f43ef
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1480c1b012f4040b28851a83b09229b746c3f91b19b26a23903e7efe854c889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 23:03:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 23:03:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 23:03:43 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 23:03:44 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 23:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:03:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 23:03:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29117a9c36d3c0a533610608811d712072dc8a92ea2d334dbc8fa9c76ef7c9bf`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270709957b90da9fa027a60063ec540960b2cd6f61f5bb3c36a4abadc5bf7311`  
		Last Modified: Thu, 23 Jan 2020 23:04:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e244e62f2ba142b8261afd7ec620d1587573e07661176f4a5cd231fddbd819`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; 386

```console
$ docker pull spiped@sha256:e9c4ae1dc83879060dc9cadee45f066036b3adb8b462aae492328d4c15052bba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2881685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f909eefbeba4e3dbafbf3eb50713011e20fca2f07f23aad79c3fca70e4dc4358`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Tue, 22 Oct 2019 01:21:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Oct 2019 01:21:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_VERSION=1.6.0
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Tue, 22 Oct 2019 01:21:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Tue, 22 Oct 2019 01:21:42 GMT
VOLUME [/spiped]
# Tue, 22 Oct 2019 01:21:42 GMT
WORKDIR /spiped
# Tue, 22 Oct 2019 01:21:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 22 Oct 2019 01:21:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Oct 2019 01:21:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca02e7557b46d0793d3e195e66b7d004e968f3f2496a996c3630f7112578b60`  
		Last Modified: Tue, 22 Oct 2019 01:21:57 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9e359b6b92862eed2520f4a63b8c940a6a69549f09658f891cc12c63596b21`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a1102fb9a96a1625137d6099791ed3dc8c283dc657362a66143b2b61d5a9a`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 87.7 KB (87713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f321a157cbffcf6ea386fdc2753279e72f3d7fe279f2a7d6791e77da4d3d01`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e878ac125de628350bdd8ca1c536d8b73fb4cbd350e62251f7924a434411be2`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:45fde12ba87e9485fa2492800f06b5be74389f0cf0479a9e332b6a5a7c39d354
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2905035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dc34cf420e2d6d3376211c900f10d023d74c8aa156616f5de04e90a125b4044`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 22:49:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 22:49:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 22:49:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 22:49:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 22:49:29 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 22:49:31 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 22:49:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 22:49:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ca9988558a5eacce7c90cdc4e47bdbb211376da49463c155923430de39d4a`  
		Last Modified: Thu, 23 Jan 2020 22:49:55 GMT  
		Size: 88.4 KB (88392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf498a32c132740eb11d320a6bef7c1930ccbf579ab6215758fc79ea8a84bc4`  
		Last Modified: Thu, 23 Jan 2020 22:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5475460c54abc8555bf4d0cbd75e770a399cd70c60d4e0108a0a7b8290031c17`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:488a2de17ec852acfc64aaa85eda6f96d871735c6d4e81b7c623a708823f1618
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e0a04dece66804c096550d7b0f2d118b9fc71ba20a8286b2e2b01c10cc9d53b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:10:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:10:07 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:10:07 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:10:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:10:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42bb1f437036a8001e843fa5970d110834f88eab3f52e0117394eb55dfd5717`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad352e7500492b9a55f564319ec4901c35391305ea2d03122f0b2b4d6e53c97`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6ef0b43b14cc42f0b136a8abbef558d32eb7b3e367fd97369ec774dc82090`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:088d5ea43f5f03d8f0e7f8d7cc7f408c051e96d9bf857a700813f9e7784df61e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:72e22523884276e22a39cb4ca1565ad39fb6d4022bbf8dc95c2ca971837d2076
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2874547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5651969446d1f1cc825c8b9ba7dc1e5801199fd64ed74c8d9599ea384919c48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:03:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 22:03:35 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 22:03:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 22:03:45 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 22:03:45 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 22:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 22:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 22:03:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f06f6c021497e75da7d87b6915a230626924c07991053d9a549fe400002cd18`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a4c78135aa6f75a6b5c923dada0201438e732b2ec25d5ae4be29cc120ca65c`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 6.3 KB (6315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e663e994236beda0de3f4f37acce0c41beca2e1aae2ba383534a5028103a5b6e`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 79.4 KB (79404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657a50cf15a9d8436f360d957ff17c290cef5b2a33dc2da440eccd93b5ad2f0`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e8488c4af15837a96b0fd48f4b5818da4056d3d8c253457edc7e915db76f42`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3ae91669334784f7b06ff519d1493b018d6b1946da07f9538b9ce403ba6a806c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66aceefd2fe95659d0e866344c41b8ab59a1f5edea0d9b102bcfb102808402ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 21:07:16 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 21:07:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 21:07:18 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 21:07:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 21:07:40 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 21:07:41 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 21:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:07:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 21:07:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ca77a0d6c23ca1ab7a1d6247b2f6058a74967635d48c6436eddb9c4ab9dc8b`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 68.0 KB (67990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecc30ce77974a56c9958f85075516bf23a4d87f452a99f0994ba66bbdff2b2f`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d253ce677e060437c999efb2094afda12da7234d44582a95187be47777394`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf6bfcf29967c12ef7c3749eefef9078bd45f60bd4c88f76c983108a3d464f42
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccadcaa5909aa00e88b17bf5880f652201851d3584c86fff7fcb9fa620424043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:56:51 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:57:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:57:11 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:57:11 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:57:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:57:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b88556cd7e307bd7aae61fbb97a5a495fd194bc5ca395dae82b60e890550492`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 61.7 KB (61746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb7e64f07324c2b74ff72e4b59b8a1693e42d453bf3e54a36e830699e3726c1`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39643304907003481036d0a383c8fc76114ab8f7ef02e7ae8513c2c1d30bfb56`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:20b57cf601ee060aeaf921435a00e6a82a6530d41dd56dcd9e39c61ff91f43ef
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1480c1b012f4040b28851a83b09229b746c3f91b19b26a23903e7efe854c889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 23:03:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 23:03:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 23:03:43 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 23:03:44 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 23:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:03:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 23:03:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29117a9c36d3c0a533610608811d712072dc8a92ea2d334dbc8fa9c76ef7c9bf`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270709957b90da9fa027a60063ec540960b2cd6f61f5bb3c36a4abadc5bf7311`  
		Last Modified: Thu, 23 Jan 2020 23:04:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e244e62f2ba142b8261afd7ec620d1587573e07661176f4a5cd231fddbd819`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:e9c4ae1dc83879060dc9cadee45f066036b3adb8b462aae492328d4c15052bba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2881685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f909eefbeba4e3dbafbf3eb50713011e20fca2f07f23aad79c3fca70e4dc4358`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Tue, 22 Oct 2019 01:21:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Oct 2019 01:21:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_VERSION=1.6.0
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Tue, 22 Oct 2019 01:21:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Tue, 22 Oct 2019 01:21:42 GMT
VOLUME [/spiped]
# Tue, 22 Oct 2019 01:21:42 GMT
WORKDIR /spiped
# Tue, 22 Oct 2019 01:21:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 22 Oct 2019 01:21:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Oct 2019 01:21:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca02e7557b46d0793d3e195e66b7d004e968f3f2496a996c3630f7112578b60`  
		Last Modified: Tue, 22 Oct 2019 01:21:57 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9e359b6b92862eed2520f4a63b8c940a6a69549f09658f891cc12c63596b21`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a1102fb9a96a1625137d6099791ed3dc8c283dc657362a66143b2b61d5a9a`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 87.7 KB (87713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f321a157cbffcf6ea386fdc2753279e72f3d7fe279f2a7d6791e77da4d3d01`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e878ac125de628350bdd8ca1c536d8b73fb4cbd350e62251f7924a434411be2`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:45fde12ba87e9485fa2492800f06b5be74389f0cf0479a9e332b6a5a7c39d354
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2905035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dc34cf420e2d6d3376211c900f10d023d74c8aa156616f5de04e90a125b4044`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 22:49:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 22:49:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 22:49:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 22:49:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 22:49:29 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 22:49:31 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 22:49:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 22:49:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ca9988558a5eacce7c90cdc4e47bdbb211376da49463c155923430de39d4a`  
		Last Modified: Thu, 23 Jan 2020 22:49:55 GMT  
		Size: 88.4 KB (88392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf498a32c132740eb11d320a6bef7c1930ccbf579ab6215758fc79ea8a84bc4`  
		Last Modified: Thu, 23 Jan 2020 22:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5475460c54abc8555bf4d0cbd75e770a399cd70c60d4e0108a0a7b8290031c17`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:488a2de17ec852acfc64aaa85eda6f96d871735c6d4e81b7c623a708823f1618
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e0a04dece66804c096550d7b0f2d118b9fc71ba20a8286b2e2b01c10cc9d53b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:10:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:10:07 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:10:07 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:10:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:10:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42bb1f437036a8001e843fa5970d110834f88eab3f52e0117394eb55dfd5717`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad352e7500492b9a55f564319ec4901c35391305ea2d03122f0b2b4d6e53c97`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6ef0b43b14cc42f0b136a8abbef558d32eb7b3e367fd97369ec774dc82090`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:088d5ea43f5f03d8f0e7f8d7cc7f408c051e96d9bf857a700813f9e7784df61e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:72e22523884276e22a39cb4ca1565ad39fb6d4022bbf8dc95c2ca971837d2076
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2874547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5651969446d1f1cc825c8b9ba7dc1e5801199fd64ed74c8d9599ea384919c48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:03:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 22:03:35 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 22:03:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 22:03:45 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 22:03:45 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 22:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 22:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 22:03:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f06f6c021497e75da7d87b6915a230626924c07991053d9a549fe400002cd18`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a4c78135aa6f75a6b5c923dada0201438e732b2ec25d5ae4be29cc120ca65c`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 6.3 KB (6315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e663e994236beda0de3f4f37acce0c41beca2e1aae2ba383534a5028103a5b6e`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 79.4 KB (79404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657a50cf15a9d8436f360d957ff17c290cef5b2a33dc2da440eccd93b5ad2f0`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e8488c4af15837a96b0fd48f4b5818da4056d3d8c253457edc7e915db76f42`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3ae91669334784f7b06ff519d1493b018d6b1946da07f9538b9ce403ba6a806c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66aceefd2fe95659d0e866344c41b8ab59a1f5edea0d9b102bcfb102808402ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 21:07:16 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 21:07:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 21:07:18 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 21:07:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 21:07:40 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 21:07:41 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 21:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:07:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 21:07:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ca77a0d6c23ca1ab7a1d6247b2f6058a74967635d48c6436eddb9c4ab9dc8b`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 68.0 KB (67990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecc30ce77974a56c9958f85075516bf23a4d87f452a99f0994ba66bbdff2b2f`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d253ce677e060437c999efb2094afda12da7234d44582a95187be47777394`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf6bfcf29967c12ef7c3749eefef9078bd45f60bd4c88f76c983108a3d464f42
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccadcaa5909aa00e88b17bf5880f652201851d3584c86fff7fcb9fa620424043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:56:51 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:57:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:57:11 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:57:11 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:57:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:57:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b88556cd7e307bd7aae61fbb97a5a495fd194bc5ca395dae82b60e890550492`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 61.7 KB (61746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb7e64f07324c2b74ff72e4b59b8a1693e42d453bf3e54a36e830699e3726c1`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39643304907003481036d0a383c8fc76114ab8f7ef02e7ae8513c2c1d30bfb56`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:20b57cf601ee060aeaf921435a00e6a82a6530d41dd56dcd9e39c61ff91f43ef
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1480c1b012f4040b28851a83b09229b746c3f91b19b26a23903e7efe854c889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 23:03:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 23:03:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 23:03:43 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 23:03:44 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 23:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:03:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 23:03:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29117a9c36d3c0a533610608811d712072dc8a92ea2d334dbc8fa9c76ef7c9bf`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270709957b90da9fa027a60063ec540960b2cd6f61f5bb3c36a4abadc5bf7311`  
		Last Modified: Thu, 23 Jan 2020 23:04:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e244e62f2ba142b8261afd7ec620d1587573e07661176f4a5cd231fddbd819`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:e9c4ae1dc83879060dc9cadee45f066036b3adb8b462aae492328d4c15052bba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2881685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f909eefbeba4e3dbafbf3eb50713011e20fca2f07f23aad79c3fca70e4dc4358`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Tue, 22 Oct 2019 01:21:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Oct 2019 01:21:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_VERSION=1.6.0
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Tue, 22 Oct 2019 01:21:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Tue, 22 Oct 2019 01:21:42 GMT
VOLUME [/spiped]
# Tue, 22 Oct 2019 01:21:42 GMT
WORKDIR /spiped
# Tue, 22 Oct 2019 01:21:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 22 Oct 2019 01:21:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Oct 2019 01:21:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca02e7557b46d0793d3e195e66b7d004e968f3f2496a996c3630f7112578b60`  
		Last Modified: Tue, 22 Oct 2019 01:21:57 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9e359b6b92862eed2520f4a63b8c940a6a69549f09658f891cc12c63596b21`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a1102fb9a96a1625137d6099791ed3dc8c283dc657362a66143b2b61d5a9a`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 87.7 KB (87713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f321a157cbffcf6ea386fdc2753279e72f3d7fe279f2a7d6791e77da4d3d01`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e878ac125de628350bdd8ca1c536d8b73fb4cbd350e62251f7924a434411be2`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:45fde12ba87e9485fa2492800f06b5be74389f0cf0479a9e332b6a5a7c39d354
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2905035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dc34cf420e2d6d3376211c900f10d023d74c8aa156616f5de04e90a125b4044`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 22:49:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 22:49:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 22:49:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 22:49:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 22:49:29 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 22:49:31 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 22:49:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 22:49:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ca9988558a5eacce7c90cdc4e47bdbb211376da49463c155923430de39d4a`  
		Last Modified: Thu, 23 Jan 2020 22:49:55 GMT  
		Size: 88.4 KB (88392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf498a32c132740eb11d320a6bef7c1930ccbf579ab6215758fc79ea8a84bc4`  
		Last Modified: Thu, 23 Jan 2020 22:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5475460c54abc8555bf4d0cbd75e770a399cd70c60d4e0108a0a7b8290031c17`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:488a2de17ec852acfc64aaa85eda6f96d871735c6d4e81b7c623a708823f1618
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e0a04dece66804c096550d7b0f2d118b9fc71ba20a8286b2e2b01c10cc9d53b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:10:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:10:07 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:10:07 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:10:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:10:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42bb1f437036a8001e843fa5970d110834f88eab3f52e0117394eb55dfd5717`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad352e7500492b9a55f564319ec4901c35391305ea2d03122f0b2b4d6e53c97`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6ef0b43b14cc42f0b136a8abbef558d32eb7b3e367fd97369ec774dc82090`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:088d5ea43f5f03d8f0e7f8d7cc7f408c051e96d9bf857a700813f9e7784df61e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:72e22523884276e22a39cb4ca1565ad39fb6d4022bbf8dc95c2ca971837d2076
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2874547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5651969446d1f1cc825c8b9ba7dc1e5801199fd64ed74c8d9599ea384919c48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:03:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 22:03:35 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 22:03:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 22:03:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 22:03:45 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 22:03:45 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 22:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 22:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 22:03:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f06f6c021497e75da7d87b6915a230626924c07991053d9a549fe400002cd18`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a4c78135aa6f75a6b5c923dada0201438e732b2ec25d5ae4be29cc120ca65c`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 6.3 KB (6315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e663e994236beda0de3f4f37acce0c41beca2e1aae2ba383534a5028103a5b6e`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 79.4 KB (79404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657a50cf15a9d8436f360d957ff17c290cef5b2a33dc2da440eccd93b5ad2f0`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e8488c4af15837a96b0fd48f4b5818da4056d3d8c253457edc7e915db76f42`  
		Last Modified: Mon, 21 Oct 2019 22:03:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3ae91669334784f7b06ff519d1493b018d6b1946da07f9538b9ce403ba6a806c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66aceefd2fe95659d0e866344c41b8ab59a1f5edea0d9b102bcfb102808402ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 21:07:16 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 21:07:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 21:07:18 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 21:07:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 21:07:40 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 21:07:41 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 21:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:07:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 21:07:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ca77a0d6c23ca1ab7a1d6247b2f6058a74967635d48c6436eddb9c4ab9dc8b`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 68.0 KB (67990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecc30ce77974a56c9958f85075516bf23a4d87f452a99f0994ba66bbdff2b2f`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d253ce677e060437c999efb2094afda12da7234d44582a95187be47777394`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf6bfcf29967c12ef7c3749eefef9078bd45f60bd4c88f76c983108a3d464f42
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccadcaa5909aa00e88b17bf5880f652201851d3584c86fff7fcb9fa620424043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:56:51 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:57:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:57:11 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:57:11 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:57:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:57:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b88556cd7e307bd7aae61fbb97a5a495fd194bc5ca395dae82b60e890550492`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 61.7 KB (61746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb7e64f07324c2b74ff72e4b59b8a1693e42d453bf3e54a36e830699e3726c1`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39643304907003481036d0a383c8fc76114ab8f7ef02e7ae8513c2c1d30bfb56`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:20b57cf601ee060aeaf921435a00e6a82a6530d41dd56dcd9e39c61ff91f43ef
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1480c1b012f4040b28851a83b09229b746c3f91b19b26a23903e7efe854c889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 23:03:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 23:03:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 23:03:43 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 23:03:44 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 23:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:03:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 23:03:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29117a9c36d3c0a533610608811d712072dc8a92ea2d334dbc8fa9c76ef7c9bf`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270709957b90da9fa027a60063ec540960b2cd6f61f5bb3c36a4abadc5bf7311`  
		Last Modified: Thu, 23 Jan 2020 23:04:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e244e62f2ba142b8261afd7ec620d1587573e07661176f4a5cd231fddbd819`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:e9c4ae1dc83879060dc9cadee45f066036b3adb8b462aae492328d4c15052bba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2881685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f909eefbeba4e3dbafbf3eb50713011e20fca2f07f23aad79c3fca70e4dc4358`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Tue, 22 Oct 2019 01:21:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Oct 2019 01:21:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_VERSION=1.6.0
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Tue, 22 Oct 2019 01:21:31 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Tue, 22 Oct 2019 01:21:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Tue, 22 Oct 2019 01:21:42 GMT
VOLUME [/spiped]
# Tue, 22 Oct 2019 01:21:42 GMT
WORKDIR /spiped
# Tue, 22 Oct 2019 01:21:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 22 Oct 2019 01:21:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Oct 2019 01:21:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca02e7557b46d0793d3e195e66b7d004e968f3f2496a996c3630f7112578b60`  
		Last Modified: Tue, 22 Oct 2019 01:21:57 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9e359b6b92862eed2520f4a63b8c940a6a69549f09658f891cc12c63596b21`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a1102fb9a96a1625137d6099791ed3dc8c283dc657362a66143b2b61d5a9a`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 87.7 KB (87713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f321a157cbffcf6ea386fdc2753279e72f3d7fe279f2a7d6791e77da4d3d01`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e878ac125de628350bdd8ca1c536d8b73fb4cbd350e62251f7924a434411be2`  
		Last Modified: Tue, 22 Oct 2019 01:21:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:45fde12ba87e9485fa2492800f06b5be74389f0cf0479a9e332b6a5a7c39d354
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2905035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dc34cf420e2d6d3376211c900f10d023d74c8aa156616f5de04e90a125b4044`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 22:49:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 22:49:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 22:49:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 22:49:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 22:49:29 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 22:49:31 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 22:49:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 22:49:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ca9988558a5eacce7c90cdc4e47bdbb211376da49463c155923430de39d4a`  
		Last Modified: Thu, 23 Jan 2020 22:49:55 GMT  
		Size: 88.4 KB (88392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf498a32c132740eb11d320a6bef7c1930ccbf579ab6215758fc79ea8a84bc4`  
		Last Modified: Thu, 23 Jan 2020 22:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5475460c54abc8555bf4d0cbd75e770a399cd70c60d4e0108a0a7b8290031c17`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:488a2de17ec852acfc64aaa85eda6f96d871735c6d4e81b7c623a708823f1618
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e0a04dece66804c096550d7b0f2d118b9fc71ba20a8286b2e2b01c10cc9d53b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:10:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:10:07 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:10:07 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:10:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:10:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42bb1f437036a8001e843fa5970d110834f88eab3f52e0117394eb55dfd5717`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad352e7500492b9a55f564319ec4901c35391305ea2d03122f0b2b4d6e53c97`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6ef0b43b14cc42f0b136a8abbef558d32eb7b3e367fd97369ec774dc82090`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:f13723692b09cb16472b7385bcd6682310f42d55eb20afc3a6fa0a8aa35347e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:d7a527e63589d1c652349e10175e2a12410746fd315ffc22f049d68daa817703
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36250037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47598dabed088d23163d926cffc0dadc0d4ecde1121b8bba28ea72e5d6b51503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:24:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:24:08 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:24:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:24:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:24:43 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:24:43 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:24:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:24:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:24:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203702656f2bc38f30feb84f231409c6410c791f7cdbfbfbfced0542a244a0fd`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557fe75836e921d1614d4851bb548ea1c3461fd961fb1da808ecfcd64be0b783`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 2.1 MB (2128038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b46de8c6821819710736655000293f13ccd254c856c530ceb0284fd5bce051d`  
		Last Modified: Sat, 28 Dec 2019 15:25:05 GMT  
		Size: 7.0 MB (7027553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19abe18c9a99d59f8232801356dd34ef508a3ad98b3a9882942c72b57e1fbe28`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408ec0d81452b12c37407b4241dda1c7ceba349382dfdfa0a6e567d86fe325bb`  
		Last Modified: Sat, 28 Dec 2019 15:25:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:f34e16bf7e1eb0e0ea66e777125e22a48addc445a562e779ea560c06027e1b81
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32143608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c98047f88a0ccc7bff1e53ba518e9151969fd8976b360ddda3d343c57d27e4fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:26:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 07:26:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:26:29 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 07:26:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 07:26:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 07:27:36 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 07:27:37 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 07:27:38 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 07:27:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 07:27:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 07:27:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c6e24c6e8419c0af6f6c6ab83019bbc2f0a11b6d859a39a2ab68804c7370c5`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7861630cbcb98d5220dc36843f7ccaa064bf7eeec94be5fb17ed5fc6cfc5ef78`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 1.8 MB (1839099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574a0ed773473e94c320b2f5b76c37b05fbbfa110ccf92ac273fe40835b8b3cc`  
		Last Modified: Sat, 28 Dec 2019 07:27:55 GMT  
		Size: 5.5 MB (5472684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335610f863ed9990600eba791bdbb9d06b5fff1adab04f447b59f2fc17114f3d`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a48dbcaae96bd7d53f5e3d7639aa585d05a3296e80215e2bac3360e39fe2a98`  
		Last Modified: Sat, 28 Dec 2019 07:27:53 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:53546fd0ca5d9265f674627303daf9879bec4c478c7182dfee9350c7b9f03aa5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29739828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c544d9f76a3ab23c1a2e6b2d2c97fbd476433e5cda4706e1d75c9aeefadf551`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:30:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:30:20 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:30:21 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:30:22 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:30:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:31:14 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:31:15 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:31:16 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:31:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:31:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:31:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44760daed9bd7e053b8359b083d503784b8fa54a77c2be7e30d6992f9ec11566`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb7b11245dcb2b9280aa470c53ab1a1c1a1d6b59a3e1b11fb4af3efa32b71c6`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 1.8 MB (1759411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e75be9243e45729cbf888681603e935380cb319ee933cbe62e04cf0f12e019`  
		Last Modified: Sat, 28 Dec 2019 15:31:56 GMT  
		Size: 5.3 MB (5279087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e21e4371b999ea9ceb6793cbdf0d7b62277493902b3b0cce605296e2b0725`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850b607025feab0f31b7bfb898db73bab4ae1550f20e614914ff2295de16a7de`  
		Last Modified: Sat, 28 Dec 2019 15:31:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:857577271f4befe4d3940908e4ae2e29df85185549e0a66be4df985eeb34efad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33760061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6e33753196bcfcd1535f691816ec9552d18a610496600fc3c1d269682ea3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 23:44:15 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 23:44:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:44:29 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 23:44:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 23:44:31 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 23:45:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 23:45:17 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 23:45:18 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 23:45:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 23:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 23:45:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8e852ce6071469cdfbd8efc7e96697a6f1f922e0ea51eddf67ef538683a610`  
		Last Modified: Sat, 28 Dec 2019 23:45:42 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e089395518f54f3841e117bf0160c8e54e58cc3fa7dc98353a11d8368175`  
		Last Modified: Sat, 28 Dec 2019 23:45:42 GMT  
		Size: 2.0 MB (2007805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415fef10a74ca9dc337d9f82164c3d6d300ca4138a1eeaa1babb81c18b320a04`  
		Last Modified: Sat, 28 Dec 2019 23:45:46 GMT  
		Size: 5.9 MB (5899346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfd645d4631682b8972cbe12c69e7dde2998de3c4f8f06fbd9b7ea25499c45`  
		Last Modified: Sat, 28 Dec 2019 23:45:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f56e3d1ee35f83a66fd9c5ca9107877c87495f78c23b16af227d6761537b743`  
		Last Modified: Sat, 28 Dec 2019 23:45:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:168c95178154bb1e3007e51f9c910ad7367f73450309133a6a1118c0b5c6894e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41504389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad94098493589622565beb5945d14d25b1238995924d460081359a9eddc6084`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:28:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 15:29:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 15:29:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 15:29:28 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 15:29:28 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 15:29:29 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 15:29:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:29:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:29:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5610f5ff45f97f75a7401ce4a1463a61b9ea809bc4b2df4b665d1b45da7f4e44`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32baf55cd2c6722002eb93fa3674d090b634b070ef3cee2948c82f93f117813`  
		Last Modified: Sat, 28 Dec 2019 15:29:43 GMT  
		Size: 2.1 MB (2132343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d4d4973ad3c749629aeafb4d317e50d51b3640ae7541caeeebe8f170013951`  
		Last Modified: Sat, 28 Dec 2019 15:29:47 GMT  
		Size: 11.6 MB (11622861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea27042f3d808f9ac5fbbf880d4b0344b788f6a1c84ab9475ab3cd18da68a1`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2918b4236946a4defd9202282444263536eeebe1c328c16a8c13fa59150817`  
		Last Modified: Sat, 28 Dec 2019 15:29:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:1f623139620f5efe999cada98454214e9ece9afb73c3c7c70a20b0cebda9e132
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d926a33940447f241bbb066c2ec28711bc72bc6ef44d99f397a55211384b1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:26:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 06:26:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:26:52 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 06:26:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 06:27:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 06:31:38 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 06:31:44 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 06:31:48 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 06:31:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 06:31:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 06:32:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091450b7ecb8270a51ff0d82376735817c4d2d385d6a2404ee013107ab169d60`  
		Last Modified: Sat, 28 Dec 2019 06:32:26 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65aa680f52e6e9c4e23d4a4d80ebd560e04ca6ad64ffd04a010cde7cee481a`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 2.2 MB (2224902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5855143d6300ec32dd6b565f347fbefb95f61d20885d15d07363e49eb626d4`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 6.7 MB (6735504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280634de8f8748bdfa29b62191c582df919e9c849d1d5db2d82550d90f055765`  
		Last Modified: Sat, 28 Dec 2019 06:32:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95975ac48caf88db370d8e9f77cdfdb86eb82619f0d90b3d3c2213a9adf3f2f5`  
		Last Modified: Sat, 28 Dec 2019 06:32:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:c8daf96755c80cd357de141bdb2118039c7d16653ea1e6766bdce7192a2fa2f5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33462729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e91fbf5ad53569e17c34629a2c6ae58fba1d4fe5b93965b5c53737e730643b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:05:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 Dec 2019 07:05:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 28 Dec 2019 07:05:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 28 Dec 2019 07:05:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 07:05:24 GMT
VOLUME [/spiped]
# Sat, 28 Dec 2019 07:05:25 GMT
WORKDIR /spiped
# Sat, 28 Dec 2019 07:05:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Dec 2019 07:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 07:05:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feba1cae3e4de6c9427a36923d1a4b6fdf8031ad008bbb2df647367b5a13adc`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5262978a84c64bb67475a813823814a00f94cd72ec62dfce286c0e0a755ca92`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 1.8 MB (1821612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cabcb44320636e61a59dbbfdea90f4d0bd14aea3536aab7e2f64ebad5c94de0`  
		Last Modified: Sat, 28 Dec 2019 07:05:41 GMT  
		Size: 5.9 MB (5933629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7553f30f2a3addf74102dfd9c8e6abe4c552d8572e2b2852c3cb233676ed8`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a30a29355212488d05b8ba9665d991231e0d9626a5e9d4b3f048f1b489e017a`  
		Last Modified: Sat, 28 Dec 2019 07:05:40 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
