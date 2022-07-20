## `neurodebian:bionic`

```console
$ docker pull neurodebian@sha256:6c8eaab7cb8250fbf9dbe6e84d6a6cbb25054a4e65dea8edb663b4afeeec1063
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:375123cc33c1c024fb8429f011c99b58c87203c5a4a936adfaa84064dee99f3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31771462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3bbfb1b8f311ec84d7ab789e1111bcaf2f73b4ff6fb1611454c72a12352a8a4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:37:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:37:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:37:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2b3981bc62720e6e1f9f8b6fd2d4af6b8dc0d5d1d930cad27b75a30d93221`  
		Last Modified: Tue, 07 Jun 2022 00:39:28 GMT  
		Size: 4.8 MB (4817739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff80362b7a8a66dc0750954a4c03f08846b9241ac54372ec5bae9d12540d468`  
		Last Modified: Tue, 07 Jun 2022 00:39:27 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d453cada745b8af1182eb78a54478ae0375ac8f0b4b908d273b10429bcd7ec81`  
		Last Modified: Tue, 07 Jun 2022 00:39:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f79b6a697fd3011ea990d9d8ef464697221eacc2d053352e61632bcb16d3c3`  
		Last Modified: Tue, 07 Jun 2022 00:39:27 GMT  
		Size: 240.2 KB (240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:613072dfc32ef306ec8aae8a64695af0ca1164186a900f79671b015d194c4b3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28316062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eed32d420f4768d81e6ea3910355a98bdbf6c518f555961eb68bf22caefdae8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 19:59:33 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:59:34 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 19:59:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 21:48:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009ab87fd4a06ac89645cbadea8c07adc6caa451180c8b8c3fd2d1c0d104845a`  
		Last Modified: Tue, 19 Jul 2022 21:51:49 GMT  
		Size: 4.5 MB (4472162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb944c370a59f7da4037a84ab2defa07fa7ae4c51edc546d966187f61a12799`  
		Last Modified: Tue, 19 Jul 2022 21:51:48 GMT  
		Size: 1.6 KB (1643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac9f4e2fc8039ddafbac2fd5f3afc2ab083e51fbb9dc3a649be650623307437`  
		Last Modified: Tue, 19 Jul 2022 21:51:48 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11562ecd1d3e76035f89c4e9e66aabff4978f4dd96732c5977b0af816ce40c2e`  
		Last Modified: Tue, 19 Jul 2022 21:51:48 GMT  
		Size: 107.3 KB (107349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
