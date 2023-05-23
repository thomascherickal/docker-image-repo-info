## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:60a78434fdd546c8d2fc025282e6431fa3a5a5ec5dfb00ab19c7bf2c532572c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:c3cd2902ff137d947cf1183caee8e2e881476148001aea0c106652a0982d3310
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61299977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:757103b2b0ac7345e1a0dcb71a788028ccd7ab37e1a27cf53cb423724f8f4ab2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:21:12 GMT
ADD file:3b942ada2dbba1c073e568411a383d6ab987c117af5bbb011afd46549d64c4dc in / 
# Tue, 23 May 2023 01:21:12 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:23:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:23:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:23:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:29 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:8285c3e1284db51d7096ff9c9434e138a00153495c655a040787b10e562b7515`  
		Last Modified: Tue, 23 May 2023 01:25:36 GMT  
		Size: 49.3 MB (49289184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158a1759b167defe3ac364f8157c49f063c470a5a956e0d702fc47b0a929f38`  
		Last Modified: Tue, 23 May 2023 04:24:47 GMT  
		Size: 11.7 MB (11722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f37d696beaa9b72a35a3d14f54f0b856dcc0621888c8afb8cc7ddda831e3310`  
		Last Modified: Tue, 23 May 2023 04:24:45 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e94a7d5efaab58c44a59d954d27135a86f8e445818b065a841ac08f6f00544`  
		Last Modified: Tue, 23 May 2023 04:24:45 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b33126a764321fb1a50ada00da1192641da6f41c03432c227137e50acd8357`  
		Last Modified: Tue, 23 May 2023 04:24:46 GMT  
		Size: 286.3 KB (286314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c80b51ea09266240fd930629cb4fb877838167da0961769224e46b9843a810`  
		Last Modified: Tue, 23 May 2023 04:24:56 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:48c979657bcab083b5a181f205a8ba52a3218b18bed5b443ebeb4bc8cc33fafa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61311075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aa7f0542b4bfb7559aeef459dc4cc4d68c1a8b4ba610d3fafee39694f4623e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:48 GMT
ADD file:4608b82b211b6814e5bf372be706a6c01bd7a2a4841b59ac5430ec3a3f94468d in / 
# Tue, 23 May 2023 00:43:49 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:30:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:30:36 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:40 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5842d200e3f7df637a96b64f14e82ccb2c66e201137165f2d91447fbd3248a8c`  
		Last Modified: Tue, 23 May 2023 00:47:31 GMT  
		Size: 49.3 MB (49336298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5dc20c7009c0c4fb8fcc9510272b9663f770c650ec6a79065e104de65ae083`  
		Last Modified: Tue, 23 May 2023 02:31:55 GMT  
		Size: 11.7 MB (11685804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70e50d9fe81355ff8795fe4ebe3fa83df06646ae08c427d3ce1f270d69c679c`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b1dce6b21c52e13c5410c66209fa00c80743c2703fa7deb3e2a45c521dab`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ee43739ae5dd8545181114be4dc1eda914eac3630aaf0547acfc5fd4f213a9`  
		Last Modified: Tue, 23 May 2023 02:31:54 GMT  
		Size: 286.6 KB (286566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93ad45069d23343bb6311642e0f863b5900a8b9eea8b859b2bbe1721dff1f09`  
		Last Modified: Tue, 23 May 2023 02:32:02 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:6753b469ed406da38695358a52a1c87e179ebe14d42c59b452a6cf03dc178c54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62745547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d6d3c089bd7ecb7dece0a9305fb5900887130cddead11f80b1b13b0fb57b418`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:40:47 GMT
ADD file:33dd3eb2725f92170606ce015e99cc9496d244630b3f4844cb8f3f61b16e2eb0 in / 
# Tue, 23 May 2023 00:40:48 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:43:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:43:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:43:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:42 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:1034171b4bde64cf8e4ff854704a3bf68000eddcceb63b481197082dced785ba`  
		Last Modified: Tue, 23 May 2023 00:46:09 GMT  
		Size: 50.3 MB (50311497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb94666b190ba95be7fadf283441a70d7afa10a0b07170b8674ec2678968d429`  
		Last Modified: Tue, 23 May 2023 05:44:50 GMT  
		Size: 12.1 MB (12145347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf7364560006b36553ea625f2134dc9718506f9939d605cf9bbeffa03222aa8`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e68c126603fa53d236ac3cef352fb8266303d1f60ea86c338b5a104baa5a545`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fef25ab16b5c30aa387e5e2d002d54aff3c430bb03a10607bffcb018bc94d4`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 286.3 KB (286305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da399a07548054d441160ab6c71e0f30793cf8071685057f199a0590aba9ad84`  
		Last Modified: Tue, 23 May 2023 05:44:57 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
