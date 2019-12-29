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
