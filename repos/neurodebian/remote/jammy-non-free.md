## `neurodebian:jammy-non-free`

```console
$ docker pull neurodebian@sha256:d7287e2348eceea3b2b911a65384321424622979a231550087de6f98614cd496
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:1a93f10419ac3b2fc67d192cc0ac44a0b4cd51556eab43ba0c4fabadca032c5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34452470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08f4101d8a5968e24ab65ccdeb84396f73b292bd2d8cb6d9e36e5c7c7af8b831`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:41 GMT
ADD file:ba96f963bbfd429a0839c40603fdd7829eaca58f20adfa0d15e6beae8244bc08 in / 
# Tue, 25 Oct 2022 01:53:41 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:12:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:12:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 25 Oct 2022 04:12:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 25 Oct 2022 04:12:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:12:58 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:301a8b74f71f85f3a31e9c7e7fedd5b001ead5bcf895bc2911c1d260e06bd987`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 30.4 MB (30426374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a95832d3865df82237ee0ad7b128414b6968cb3a48f9b5d9278f861cff37f4`  
		Last Modified: Tue, 25 Oct 2022 04:15:40 GMT  
		Size: 3.8 MB (3766029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dc74395dc4ae2c9213d5892621dfcc1b1047040bf26d06c663d3a247fa850f`  
		Last Modified: Tue, 25 Oct 2022 04:15:39 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225bdbe83ccd5d9d6952146d2879be64c92e5a1402205bea9eeb6e2b8557f319`  
		Last Modified: Tue, 25 Oct 2022 04:15:39 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a2824a1ba1cdf637df4aa4b90c3632778328b23b3260e6ca613dbc3c76091`  
		Last Modified: Tue, 25 Oct 2022 04:15:39 GMT  
		Size: 257.8 KB (257793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793f5f160328e03e9c1b5ab285c2de333cb0cca1c369c736d53528b2d8450f51`  
		Last Modified: Tue, 25 Oct 2022 04:15:49 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:836593c6bc4045f774a159231de968402fb6cb74c71b0a7831ea7166640fe03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32092550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50c75f4d5587a358e178e8aae43b140ef11fa08b92df691c11f3739ffea93ad0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:57:59 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:00 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:01 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:08 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a74d96cddd31a9b0dcb858a34c9e4f2c2d1730679299ce66a44111af946c220`  
		Last Modified: Wed, 05 Oct 2022 04:02:08 GMT  
		Size: 3.6 MB (3593367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cab1a661086a3dc4eddc2627f2548445bd3185053ba7c024f9f03c9069e039`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c5bdf963687c93eca41e724d30263052cb0477c9b631dc4d14432142488855`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30638b5977520e4c36f1e8c72edd304b0be8f000dc6c349287ae1832ebb83b27`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 114.7 KB (114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d97faa1fa50fd30713bd4d7d1f5eda0123ce7a0b310dcac4ca92093e8040296`  
		Last Modified: Wed, 05 Oct 2022 04:02:18 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
