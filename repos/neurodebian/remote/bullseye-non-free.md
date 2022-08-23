## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:8f46a81df71a6fd6eb3e8743319ce935638ff7d4f4ba25f48c5c796651410246
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:f865df23569ce8d81cc0f8ccd3e8b33d6ccc250ae34a26352f9161e0a074215a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66632140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b60780d8b2d8dd6b19f7afa2f9602864ccf2d9aa4ceb546623604bbbfb470b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:34 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:35 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:39 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:43 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da4c47f93a29385c466f0b8d06c34810d3c2fcf6a9fd424a039d0a9dd5ba91a`  
		Last Modified: Tue, 23 Aug 2022 03:57:33 GMT  
		Size: 11.3 MB (11310656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baadeaeeef9ec92fffddaf3f7991f97f2852ce3310c7e7115279778ce1b60c23`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6357f4e4c8211177f51c1526a9d04ce62e0dd0ed3eeb6745feda9f395463d`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb160502891152d59ef71771495e79282a1d437e3a848021655e73ad1c5e6e48`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 311.6 KB (311560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d754d80adef35e288ba8c81b0c1d43a68a7a9e9ea44bc4c28954e7006e4c2ec9`  
		Last Modified: Tue, 23 Aug 2022 03:57:44 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:4a4b0248eac44e958218d5cc595b06a281d5ec394de57a48e127631d166842f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64895258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fd53427e1b819b7fefedba74bd470e4361c2d66d6458836639fd8820cfb41d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:26 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff40e6a469794f9119b4074673af50f6e14202e8140c999b2934d90e5d334532`  
		Last Modified: Tue, 02 Aug 2022 04:12:56 GMT  
		Size: 11.1 MB (11104729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2a776b73fedde99a37ad1a5b4225e4cbc0b571fca2183b5ed2f22eb8808108`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28656afe730c0967736477f5ec1ed6f2366700ed354642dc492275fe287e71cb`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee0dbec7c4163720ac1f0d28a757f4e31c98305ec91f34c9e15dc034a6ad6b`  
		Last Modified: Tue, 02 Aug 2022 04:12:55 GMT  
		Size: 105.2 KB (105171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c0342191d269718b61134e36c597d1f0c21655afbd52d6ad48fdf07054b7e`  
		Last Modified: Tue, 02 Aug 2022 04:13:10 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:e98da7e376fde4c546e16b52735e663eb876819b1795a560666f1ee80330b929
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67609277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2aa7047da75911beb318e8f6a833147b12b661ba5dae09517fd3a378231cd6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:05 GMT
ADD file:ade7fe80dd06354b3eab9283f6c354047be2b94806dbe1dedee8d5a0f658f7be in / 
# Tue, 02 Aug 2022 00:39:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:32 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:84601b97875630e4b14ebdb276bc4c68f89eafe6d12dec64b54dbcaed7c0c802`  
		Last Modified: Tue, 02 Aug 2022 00:44:40 GMT  
		Size: 56.0 MB (56002231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27896781078532c6ddb430224d3c48f834d093e2ab3ae5ff4805af3597860da1`  
		Last Modified: Tue, 02 Aug 2022 16:21:46 GMT  
		Size: 11.5 MB (11499635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f1ce447767d12a4c29740ef298c72902b324eecc4f8f0f0c763e38c98bab6d`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a522090ef6aa533a52810a47e789f07e4c7ff1a06cd9c5191eb0feebd0fb5a`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b003d4600f8668923f8466f8795c15318ecc94ee07d7631411f57e6a5cb9e8b`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 105.1 KB (105064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b434f1dc0af5922193126a834695fe056c58896604f9207fe6f1224461fb59c`  
		Last Modified: Tue, 02 Aug 2022 16:22:01 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
