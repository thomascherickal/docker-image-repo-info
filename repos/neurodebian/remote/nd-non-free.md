## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:81280c9b90b55267fcd5d76144088664479223b24fac457ea232c971fd200fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:3e1fda817390144cf38a8ad2261957ecaf31672324e8ebf505ea503b8c18acae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03316cf4967259749fc22171bdee854ef9b9aff3303b43444791690fb75e0d6d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:42 GMT
ADD file:6261ecb921e04d2b3f6fd44e5dcb5683154bc0beee4f26913c2be9395a060489 in / 
# Tue, 02 May 2023 23:47:43 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:26:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:26:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:26:08 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:26:12 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:26:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ae396e350f30e1defad1bfa67a84b97389d42cf3442551e39a0e2bab6b53a50c`  
		Last Modified: Tue, 02 May 2023 23:51:56 GMT  
		Size: 49.3 MB (49299270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07001fa6af159175c58303f7752dd97019fd06951e7055bcb076e5194afa064f`  
		Last Modified: Wed, 03 May 2023 21:27:50 GMT  
		Size: 11.7 MB (11719904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdf86d32a3b26b1c1bd693d70bc6115b98a87379e31ff8b6f6b9f7ed9009fe3`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dee1f3f9a40aee303f152160ad22cf80424301d6e75afcd194d8f83d27543`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745484e4809d3b3760d3a506060c0d4454cf63ff0de190c172235e7f825eaa2f`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 284.6 KB (284611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8500a41f7e728906fca7f1d637852202a87f9ea250eec4cfdf14f4a10d85694`  
		Last Modified: Wed, 03 May 2023 21:27:58 GMT  
		Size: 397.0 B  
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
$ docker pull neurodebian@sha256:3b55d7527f746dda6b623936b102556d07bb27844f33f3b3a73f3fd4d4cc287b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62752686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a3f168461765aee166a808516f45328083a8569d9221c64fbe2fd8c2ab84650`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:59 GMT
ADD file:4abf127b0d4037b2d94457a8ef168165ed6946fec0635fdaa845ed4ee8f74681 in / 
# Wed, 03 May 2023 00:02:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:17:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:17:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:34 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:125509149936f5c9fc010cb99811f5cb23108af74e034fcf0903d3f2cc08d893`  
		Last Modified: Wed, 03 May 2023 00:06:56 GMT  
		Size: 50.3 MB (50321774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03401a139b285d7dbabf9bf47070d8513369654c65656e0c9d884753d539277f`  
		Last Modified: Wed, 03 May 2023 23:18:43 GMT  
		Size: 12.1 MB (12143791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5281eb68b6af5d72745e5c9b4b79dd83518a7577dc0fe9d915aded3a47e043`  
		Last Modified: Wed, 03 May 2023 23:18:41 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d185612295077c05c7f4013d0363a5a2d03ec6b9616cdd174458890a2a4a127b`  
		Last Modified: Wed, 03 May 2023 23:18:41 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab7c155e27703e280eaf8bb7af29a7e4811f8eff90e33735e85d08540012bcd`  
		Last Modified: Wed, 03 May 2023 23:18:42 GMT  
		Size: 284.7 KB (284722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5fa32322a1c07f34e547f4775540f6eab3c1d3464b5a006bd5c2449a0bced3`  
		Last Modified: Wed, 03 May 2023 23:18:51 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
