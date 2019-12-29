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
$ docker pull spiped@sha256:2a0c088effed072cbb6b1360698a197bcadb8fc958fe23aa055589d6294c53d0
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
$ docker pull spiped@sha256:2cf538fc4e929a4f7752f04dba84eff585e55f4b3d2917b0be5026c5c4bd6763
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b2f2dc5a77cf488dd72ef7f27725c98ea07fb65e8bc7ad5f8937035964acaf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 21:22:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 21:22:39 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 21:22:40 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 21:22:41 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 21:22:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 21:23:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 21:23:04 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 21:23:06 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 21:23:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 21:23:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 21:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d952e6972b0b0e10480f9134e767317b4ebb43d95bb1f0c6f64d57f0c04ac90`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a10256d2b46c9ccd14f50c7c4b46fef55537f1d0ce4f06898dd6335112623e8`  
		Last Modified: Mon, 21 Oct 2019 21:23:22 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c5d994603f42e631ecaf880f370adb144c6a97c35dcaba51dbc7fcfc69f60`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 68.0 KB (67996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653ba5d9e38c1313f3ff7a9bab12b475ab946c16f75804c490b22c7c88937a9c`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9ab01a5c4ed2726234dbdd27d573389d7ceffefb755a56702ef9ee3c9107e8`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8d53b4b7f038a5f467947c6870d5a16755aa2ab4811ee0784d9ed43add40a555
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aeee6bb4f481dae47325d742926213ecf3535335e88ba9b89726a0bcac16a15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:27 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 18:59:29 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 18:59:29 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 18:59:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 18:59:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 18:59:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 18:59:49 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 18:59:50 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 18:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 18:59:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:59:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d2313cb7a0c630d04544d11bdfc9c4c6ce8b1d829859ad5979e5039d04088`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cffc8eafd0aceb1730887bba7f1acb5c73bd813fdd2e9042cc1df2ccc041b71`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 6.3 KB (6332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af125fcda923f6de641df7dc9dc690d787ad740d2e3bd986d1004ed392f0e4ab`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 61.7 KB (61735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50448ec145c854a7cb7d2e10a1b9f7657cb1cb7af192b9e982e411fe0dd9470`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f5168dfea15f92e2a0d251d1563414fbc837cbdf10c36e9a54df5850d0d6f`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6580ab79de2e4bf90f1bf52de091888b664bd3ddf48374a7f2eb3edb97893d03
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb7994cd03ffd946c304980aa3310a7d9219fe95c6def4971b93c5efe6cfcedf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:06:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 20:06:13 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 20:06:15 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 20:06:15 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 20:06:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 20:06:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 20:06:40 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 20:06:41 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 20:06:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 20:06:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 20:06:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38ff93b481cf454b2fc607b974ba1899df4439e8a0ae08468e0c5eefec44d0e`  
		Last Modified: Mon, 21 Oct 2019 20:06:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db9247f831f1f7777b45a65b2f966b57e440779c06ca4fefd591089ff688dee`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 6.3 KB (6331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838ed88fe613b7df202febe3fca960aa21461aaa42c6158b23d6994f1e73ac1e`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0269530c73671116af4ceea5fca7281e7d8e198d4d122785b33da02710d01f6e`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2635cd86a398ecb5bcfd1c559936eb34f893f03fe1500a12f18d440bdfc0a15b`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:d53d52793ee46984c55cf707831a7974a9ecf16b03f83ae8e21299ab2c28b5fd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2904995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de70dc1491d6e1379173730ae8168e0228422f490fbaa6ebd2ee6f58db459da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 17:52:55 GMT
ADD file:11a2dd0058b1642e9ee52239d03223819a53ca346fd42826eead7729c50e1257 in / 
# Mon, 21 Oct 2019 17:53:00 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:09:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 18:09:49 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 18:09:51 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 18:09:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 18:09:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 18:10:18 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 18:10:20 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 18:10:25 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 18:10:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 18:10:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:10:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd18d16ea896a0f0eb99be52a9722ffae9a5ac35cf28cb8b96f589352f8e71d6`  
		Last Modified: Mon, 21 Oct 2019 17:53:53 GMT  
		Size: 2.8 MB (2808504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc81e5fbc49d821c0cd761a7f65b6a5b4acc246f2c1c454e7cfa965481f6b237`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17be2e1a589388454ba4380fbd06922cd8dc86128e18674dcaaf357b8b82d706`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 6.3 KB (6345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c33a41f91074cec91700fa393db7cd9dd7c6b1968770366d7098b524fffc8b`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 88.4 KB (88387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3015d8d4eae4058e77bee61a793d5610fee03a400c198972223415eda977ae46`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb178c7733752e50663cc147a246de49a056643c6dbdbb84007d0ff88deb9d`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:a1e96b161f5f7bc255e69ee156c494b098a17d7a44f51d2d0ded776743acf44e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95680363b22cbce3f34bf7d0ef777bff0a52de97c310c32d3cf273329e9ef79c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:47:28 GMT
ADD file:49020543846e4f93b34d71c0e4234ade7bd6dde3f45cb73784aa73ce0522c8bc in / 
# Mon, 21 Oct 2019 16:47:29 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:04:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 17:04:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 17:04:24 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 17:04:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 17:04:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 17:04:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 17:04:39 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 17:04:40 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 17:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 17:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 17:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb7172052a60e640810f01efff381654bf9ed44082461455cfcc6306d192d541`  
		Last Modified: Mon, 21 Oct 2019 16:48:40 GMT  
		Size: 2.6 MB (2573587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaebdf88eda96fa6f50f9f5958ca8569cfe2f05389f0a222df9794d4d3ac9a56`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f66b2603678cfc75f9729f3f7ef29e81688c7414abbd14189e32cceae2777a2`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 6.3 KB (6332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6657aabc7269bfc77c4b56f781e5e58d35f980e67bd4b5758cd0a9837f1b9a4a`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 72.7 KB (72655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff231384e6bc2fc5dd6f78e144f649637a5b04a7e9b0dfb0ad531ee480cfd925`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d9818177198d42da9496befcfe71d56fb4b0b5f0175e107313959f868004f`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:2a0c088effed072cbb6b1360698a197bcadb8fc958fe23aa055589d6294c53d0
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
$ docker pull spiped@sha256:2cf538fc4e929a4f7752f04dba84eff585e55f4b3d2917b0be5026c5c4bd6763
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b2f2dc5a77cf488dd72ef7f27725c98ea07fb65e8bc7ad5f8937035964acaf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 21:22:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 21:22:39 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 21:22:40 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 21:22:41 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 21:22:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 21:23:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 21:23:04 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 21:23:06 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 21:23:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 21:23:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 21:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d952e6972b0b0e10480f9134e767317b4ebb43d95bb1f0c6f64d57f0c04ac90`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a10256d2b46c9ccd14f50c7c4b46fef55537f1d0ce4f06898dd6335112623e8`  
		Last Modified: Mon, 21 Oct 2019 21:23:22 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c5d994603f42e631ecaf880f370adb144c6a97c35dcaba51dbc7fcfc69f60`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 68.0 KB (67996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653ba5d9e38c1313f3ff7a9bab12b475ab946c16f75804c490b22c7c88937a9c`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9ab01a5c4ed2726234dbdd27d573389d7ceffefb755a56702ef9ee3c9107e8`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8d53b4b7f038a5f467947c6870d5a16755aa2ab4811ee0784d9ed43add40a555
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aeee6bb4f481dae47325d742926213ecf3535335e88ba9b89726a0bcac16a15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:27 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 18:59:29 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 18:59:29 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 18:59:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 18:59:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 18:59:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 18:59:49 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 18:59:50 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 18:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 18:59:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:59:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d2313cb7a0c630d04544d11bdfc9c4c6ce8b1d829859ad5979e5039d04088`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cffc8eafd0aceb1730887bba7f1acb5c73bd813fdd2e9042cc1df2ccc041b71`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 6.3 KB (6332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af125fcda923f6de641df7dc9dc690d787ad740d2e3bd986d1004ed392f0e4ab`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 61.7 KB (61735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50448ec145c854a7cb7d2e10a1b9f7657cb1cb7af192b9e982e411fe0dd9470`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f5168dfea15f92e2a0d251d1563414fbc837cbdf10c36e9a54df5850d0d6f`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6580ab79de2e4bf90f1bf52de091888b664bd3ddf48374a7f2eb3edb97893d03
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb7994cd03ffd946c304980aa3310a7d9219fe95c6def4971b93c5efe6cfcedf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:06:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 20:06:13 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 20:06:15 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 20:06:15 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 20:06:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 20:06:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 20:06:40 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 20:06:41 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 20:06:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 20:06:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 20:06:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38ff93b481cf454b2fc607b974ba1899df4439e8a0ae08468e0c5eefec44d0e`  
		Last Modified: Mon, 21 Oct 2019 20:06:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db9247f831f1f7777b45a65b2f966b57e440779c06ca4fefd591089ff688dee`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 6.3 KB (6331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838ed88fe613b7df202febe3fca960aa21461aaa42c6158b23d6994f1e73ac1e`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0269530c73671116af4ceea5fca7281e7d8e198d4d122785b33da02710d01f6e`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2635cd86a398ecb5bcfd1c559936eb34f893f03fe1500a12f18d440bdfc0a15b`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:d53d52793ee46984c55cf707831a7974a9ecf16b03f83ae8e21299ab2c28b5fd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2904995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de70dc1491d6e1379173730ae8168e0228422f490fbaa6ebd2ee6f58db459da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 17:52:55 GMT
ADD file:11a2dd0058b1642e9ee52239d03223819a53ca346fd42826eead7729c50e1257 in / 
# Mon, 21 Oct 2019 17:53:00 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:09:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 18:09:49 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 18:09:51 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 18:09:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 18:09:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 18:10:18 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 18:10:20 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 18:10:25 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 18:10:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 18:10:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:10:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd18d16ea896a0f0eb99be52a9722ffae9a5ac35cf28cb8b96f589352f8e71d6`  
		Last Modified: Mon, 21 Oct 2019 17:53:53 GMT  
		Size: 2.8 MB (2808504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc81e5fbc49d821c0cd761a7f65b6a5b4acc246f2c1c454e7cfa965481f6b237`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17be2e1a589388454ba4380fbd06922cd8dc86128e18674dcaaf357b8b82d706`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 6.3 KB (6345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c33a41f91074cec91700fa393db7cd9dd7c6b1968770366d7098b524fffc8b`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 88.4 KB (88387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3015d8d4eae4058e77bee61a793d5610fee03a400c198972223415eda977ae46`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb178c7733752e50663cc147a246de49a056643c6dbdbb84007d0ff88deb9d`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:a1e96b161f5f7bc255e69ee156c494b098a17d7a44f51d2d0ded776743acf44e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95680363b22cbce3f34bf7d0ef777bff0a52de97c310c32d3cf273329e9ef79c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:47:28 GMT
ADD file:49020543846e4f93b34d71c0e4234ade7bd6dde3f45cb73784aa73ce0522c8bc in / 
# Mon, 21 Oct 2019 16:47:29 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:04:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 17:04:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 17:04:24 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 17:04:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 17:04:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 17:04:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 17:04:39 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 17:04:40 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 17:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 17:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 17:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb7172052a60e640810f01efff381654bf9ed44082461455cfcc6306d192d541`  
		Last Modified: Mon, 21 Oct 2019 16:48:40 GMT  
		Size: 2.6 MB (2573587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaebdf88eda96fa6f50f9f5958ca8569cfe2f05389f0a222df9794d4d3ac9a56`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f66b2603678cfc75f9729f3f7ef29e81688c7414abbd14189e32cceae2777a2`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 6.3 KB (6332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6657aabc7269bfc77c4b56f781e5e58d35f980e67bd4b5758cd0a9837f1b9a4a`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 72.7 KB (72655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff231384e6bc2fc5dd6f78e144f649637a5b04a7e9b0dfb0ad531ee480cfd925`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d9818177198d42da9496befcfe71d56fb4b0b5f0175e107313959f868004f`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:2a0c088effed072cbb6b1360698a197bcadb8fc958fe23aa055589d6294c53d0
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
$ docker pull spiped@sha256:2cf538fc4e929a4f7752f04dba84eff585e55f4b3d2917b0be5026c5c4bd6763
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b2f2dc5a77cf488dd72ef7f27725c98ea07fb65e8bc7ad5f8937035964acaf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 21:22:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 21:22:39 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 21:22:40 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 21:22:41 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 21:22:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 21:23:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 21:23:04 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 21:23:06 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 21:23:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 21:23:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 21:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d952e6972b0b0e10480f9134e767317b4ebb43d95bb1f0c6f64d57f0c04ac90`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a10256d2b46c9ccd14f50c7c4b46fef55537f1d0ce4f06898dd6335112623e8`  
		Last Modified: Mon, 21 Oct 2019 21:23:22 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c5d994603f42e631ecaf880f370adb144c6a97c35dcaba51dbc7fcfc69f60`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 68.0 KB (67996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653ba5d9e38c1313f3ff7a9bab12b475ab946c16f75804c490b22c7c88937a9c`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9ab01a5c4ed2726234dbdd27d573389d7ceffefb755a56702ef9ee3c9107e8`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8d53b4b7f038a5f467947c6870d5a16755aa2ab4811ee0784d9ed43add40a555
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aeee6bb4f481dae47325d742926213ecf3535335e88ba9b89726a0bcac16a15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:27 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 18:59:29 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 18:59:29 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 18:59:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 18:59:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 18:59:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 18:59:49 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 18:59:50 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 18:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 18:59:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:59:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d2313cb7a0c630d04544d11bdfc9c4c6ce8b1d829859ad5979e5039d04088`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cffc8eafd0aceb1730887bba7f1acb5c73bd813fdd2e9042cc1df2ccc041b71`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 6.3 KB (6332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af125fcda923f6de641df7dc9dc690d787ad740d2e3bd986d1004ed392f0e4ab`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 61.7 KB (61735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50448ec145c854a7cb7d2e10a1b9f7657cb1cb7af192b9e982e411fe0dd9470`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f5168dfea15f92e2a0d251d1563414fbc837cbdf10c36e9a54df5850d0d6f`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6580ab79de2e4bf90f1bf52de091888b664bd3ddf48374a7f2eb3edb97893d03
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb7994cd03ffd946c304980aa3310a7d9219fe95c6def4971b93c5efe6cfcedf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:06:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 20:06:13 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 20:06:15 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 20:06:15 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 20:06:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 20:06:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 20:06:40 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 20:06:41 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 20:06:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 20:06:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 20:06:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38ff93b481cf454b2fc607b974ba1899df4439e8a0ae08468e0c5eefec44d0e`  
		Last Modified: Mon, 21 Oct 2019 20:06:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db9247f831f1f7777b45a65b2f966b57e440779c06ca4fefd591089ff688dee`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 6.3 KB (6331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838ed88fe613b7df202febe3fca960aa21461aaa42c6158b23d6994f1e73ac1e`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0269530c73671116af4ceea5fca7281e7d8e198d4d122785b33da02710d01f6e`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2635cd86a398ecb5bcfd1c559936eb34f893f03fe1500a12f18d440bdfc0a15b`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:d53d52793ee46984c55cf707831a7974a9ecf16b03f83ae8e21299ab2c28b5fd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2904995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de70dc1491d6e1379173730ae8168e0228422f490fbaa6ebd2ee6f58db459da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 17:52:55 GMT
ADD file:11a2dd0058b1642e9ee52239d03223819a53ca346fd42826eead7729c50e1257 in / 
# Mon, 21 Oct 2019 17:53:00 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:09:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 18:09:49 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 18:09:51 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 18:09:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 18:09:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 18:10:18 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 18:10:20 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 18:10:25 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 18:10:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 18:10:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:10:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd18d16ea896a0f0eb99be52a9722ffae9a5ac35cf28cb8b96f589352f8e71d6`  
		Last Modified: Mon, 21 Oct 2019 17:53:53 GMT  
		Size: 2.8 MB (2808504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc81e5fbc49d821c0cd761a7f65b6a5b4acc246f2c1c454e7cfa965481f6b237`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17be2e1a589388454ba4380fbd06922cd8dc86128e18674dcaaf357b8b82d706`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 6.3 KB (6345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c33a41f91074cec91700fa393db7cd9dd7c6b1968770366d7098b524fffc8b`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 88.4 KB (88387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3015d8d4eae4058e77bee61a793d5610fee03a400c198972223415eda977ae46`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb178c7733752e50663cc147a246de49a056643c6dbdbb84007d0ff88deb9d`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:a1e96b161f5f7bc255e69ee156c494b098a17d7a44f51d2d0ded776743acf44e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95680363b22cbce3f34bf7d0ef777bff0a52de97c310c32d3cf273329e9ef79c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:47:28 GMT
ADD file:49020543846e4f93b34d71c0e4234ade7bd6dde3f45cb73784aa73ce0522c8bc in / 
# Mon, 21 Oct 2019 16:47:29 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:04:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 17:04:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 17:04:24 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 17:04:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 17:04:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 17:04:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 17:04:39 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 17:04:40 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 17:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 17:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 17:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb7172052a60e640810f01efff381654bf9ed44082461455cfcc6306d192d541`  
		Last Modified: Mon, 21 Oct 2019 16:48:40 GMT  
		Size: 2.6 MB (2573587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaebdf88eda96fa6f50f9f5958ca8569cfe2f05389f0a222df9794d4d3ac9a56`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f66b2603678cfc75f9729f3f7ef29e81688c7414abbd14189e32cceae2777a2`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 6.3 KB (6332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6657aabc7269bfc77c4b56f781e5e58d35f980e67bd4b5758cd0a9837f1b9a4a`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 72.7 KB (72655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff231384e6bc2fc5dd6f78e144f649637a5b04a7e9b0dfb0ad531ee480cfd925`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d9818177198d42da9496befcfe71d56fb4b0b5f0175e107313959f868004f`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:2a0c088effed072cbb6b1360698a197bcadb8fc958fe23aa055589d6294c53d0
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
$ docker pull spiped@sha256:2cf538fc4e929a4f7752f04dba84eff585e55f4b3d2917b0be5026c5c4bd6763
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b2f2dc5a77cf488dd72ef7f27725c98ea07fb65e8bc7ad5f8937035964acaf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 21:22:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 21:22:39 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 21:22:40 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 21:22:41 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 21:22:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 21:23:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 21:23:04 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 21:23:06 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 21:23:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 21:23:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 21:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d952e6972b0b0e10480f9134e767317b4ebb43d95bb1f0c6f64d57f0c04ac90`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a10256d2b46c9ccd14f50c7c4b46fef55537f1d0ce4f06898dd6335112623e8`  
		Last Modified: Mon, 21 Oct 2019 21:23:22 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c5d994603f42e631ecaf880f370adb144c6a97c35dcaba51dbc7fcfc69f60`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 68.0 KB (67996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653ba5d9e38c1313f3ff7a9bab12b475ab946c16f75804c490b22c7c88937a9c`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9ab01a5c4ed2726234dbdd27d573389d7ceffefb755a56702ef9ee3c9107e8`  
		Last Modified: Mon, 21 Oct 2019 21:23:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8d53b4b7f038a5f467947c6870d5a16755aa2ab4811ee0784d9ed43add40a555
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aeee6bb4f481dae47325d742926213ecf3535335e88ba9b89726a0bcac16a15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:27 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 18:59:29 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 18:59:29 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 18:59:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 18:59:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 18:59:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 18:59:49 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 18:59:50 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 18:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 18:59:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:59:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d2313cb7a0c630d04544d11bdfc9c4c6ce8b1d829859ad5979e5039d04088`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cffc8eafd0aceb1730887bba7f1acb5c73bd813fdd2e9042cc1df2ccc041b71`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 6.3 KB (6332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af125fcda923f6de641df7dc9dc690d787ad740d2e3bd986d1004ed392f0e4ab`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 61.7 KB (61735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50448ec145c854a7cb7d2e10a1b9f7657cb1cb7af192b9e982e411fe0dd9470`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f5168dfea15f92e2a0d251d1563414fbc837cbdf10c36e9a54df5850d0d6f`  
		Last Modified: Mon, 21 Oct 2019 19:01:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6580ab79de2e4bf90f1bf52de091888b664bd3ddf48374a7f2eb3edb97893d03
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb7994cd03ffd946c304980aa3310a7d9219fe95c6def4971b93c5efe6cfcedf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:06:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 20:06:13 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 20:06:15 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 20:06:15 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 20:06:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 20:06:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 20:06:40 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 20:06:41 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 20:06:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 20:06:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 20:06:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38ff93b481cf454b2fc607b974ba1899df4439e8a0ae08468e0c5eefec44d0e`  
		Last Modified: Mon, 21 Oct 2019 20:06:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db9247f831f1f7777b45a65b2f966b57e440779c06ca4fefd591089ff688dee`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 6.3 KB (6331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838ed88fe613b7df202febe3fca960aa21461aaa42c6158b23d6994f1e73ac1e`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0269530c73671116af4ceea5fca7281e7d8e198d4d122785b33da02710d01f6e`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2635cd86a398ecb5bcfd1c559936eb34f893f03fe1500a12f18d440bdfc0a15b`  
		Last Modified: Mon, 21 Oct 2019 20:06:58 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:d53d52793ee46984c55cf707831a7974a9ecf16b03f83ae8e21299ab2c28b5fd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2904995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de70dc1491d6e1379173730ae8168e0228422f490fbaa6ebd2ee6f58db459da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 17:52:55 GMT
ADD file:11a2dd0058b1642e9ee52239d03223819a53ca346fd42826eead7729c50e1257 in / 
# Mon, 21 Oct 2019 17:53:00 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:09:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 18:09:49 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 18:09:51 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 18:09:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 18:09:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 18:10:18 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 18:10:20 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 18:10:25 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 18:10:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 18:10:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:10:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd18d16ea896a0f0eb99be52a9722ffae9a5ac35cf28cb8b96f589352f8e71d6`  
		Last Modified: Mon, 21 Oct 2019 17:53:53 GMT  
		Size: 2.8 MB (2808504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc81e5fbc49d821c0cd761a7f65b6a5b4acc246f2c1c454e7cfa965481f6b237`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17be2e1a589388454ba4380fbd06922cd8dc86128e18674dcaaf357b8b82d706`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 6.3 KB (6345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c33a41f91074cec91700fa393db7cd9dd7c6b1968770366d7098b524fffc8b`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 88.4 KB (88387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3015d8d4eae4058e77bee61a793d5610fee03a400c198972223415eda977ae46`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb178c7733752e50663cc147a246de49a056643c6dbdbb84007d0ff88deb9d`  
		Last Modified: Mon, 21 Oct 2019 18:11:01 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:a1e96b161f5f7bc255e69ee156c494b098a17d7a44f51d2d0ded776743acf44e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95680363b22cbce3f34bf7d0ef777bff0a52de97c310c32d3cf273329e9ef79c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 21 Oct 2019 16:47:28 GMT
ADD file:49020543846e4f93b34d71c0e4234ade7bd6dde3f45cb73784aa73ce0522c8bc in / 
# Mon, 21 Oct 2019 16:47:29 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:04:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 21 Oct 2019 17:04:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 21 Oct 2019 17:04:24 GMT
ENV SPIPED_VERSION=1.6.0
# Mon, 21 Oct 2019 17:04:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Mon, 21 Oct 2019 17:04:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Mon, 21 Oct 2019 17:04:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 21 Oct 2019 17:04:39 GMT
VOLUME [/spiped]
# Mon, 21 Oct 2019 17:04:40 GMT
WORKDIR /spiped
# Mon, 21 Oct 2019 17:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 21 Oct 2019 17:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 21 Oct 2019 17:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb7172052a60e640810f01efff381654bf9ed44082461455cfcc6306d192d541`  
		Last Modified: Mon, 21 Oct 2019 16:48:40 GMT  
		Size: 2.6 MB (2573587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaebdf88eda96fa6f50f9f5958ca8569cfe2f05389f0a222df9794d4d3ac9a56`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f66b2603678cfc75f9729f3f7ef29e81688c7414abbd14189e32cceae2777a2`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 6.3 KB (6332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6657aabc7269bfc77c4b56f781e5e58d35f980e67bd4b5758cd0a9837f1b9a4a`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 72.7 KB (72655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff231384e6bc2fc5dd6f78e144f649637a5b04a7e9b0dfb0ad531ee480cfd925`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d9818177198d42da9496befcfe71d56fb4b0b5f0175e107313959f868004f`  
		Last Modified: Mon, 21 Oct 2019 17:04:58 GMT  
		Size: 340.0 B  
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
