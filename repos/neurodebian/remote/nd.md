## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:1bce594172fe668a076d83fe777240c4b60a9ceac8297d5ddc1ac1c605db5eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:4133b5b6d77a540ca2de79f0a7bca7b0c68c219193164bb435305820858cc2e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64076847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe80a908421046f1e39e1c01017388339535db844e8a0f5195bae8f72ebde7e7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:36:29 GMT
ADD file:0301a32b2b2f0af81dd4277b61ab0069818663e8ad39e59dec42f2a74e027eda in / 
# Wed, 11 Oct 2023 18:36:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:04:52 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:04:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 12 Oct 2023 00:04:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 12 Oct 2023 00:04:57 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3997a52aa0dcbfc5a01686dece23fdbb32f74ea998359451f16034544761414c`  
		Last Modified: Wed, 11 Oct 2023 18:42:29 GMT  
		Size: 49.5 MB (49503645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc64fa2e37f8989a74e99ffb107aad254e7976873443f8a4bd5c99735c327a87`  
		Last Modified: Thu, 12 Oct 2023 00:06:36 GMT  
		Size: 14.3 MB (14287000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11c551cc6c41f9b4547f1e21c0a2dd4e7ab58e7eb543916c529698ec68c2115`  
		Last Modified: Thu, 12 Oct 2023 00:06:34 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1870f67e592e0be20d08c2bf9b688a27ae99d26899b2b7122dcd50d11cfd7b09`  
		Last Modified: Thu, 12 Oct 2023 00:06:34 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2285a1d3c3065086a0887974ed20b67a06b7d10ecbe3c5a53d6a353f776645`  
		Last Modified: Thu, 12 Oct 2023 00:06:34 GMT  
		Size: 284.2 KB (284194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:173008b551278ce730b2a5fb927628155315bcad2903e1933b35a1924e60b311
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63895553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d64895a65ed15e20fe3cb3670bdb7458b07b9c880134e662ce3ae1f4b8cb6a23`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:56 GMT
ADD file:c18e09bd64c99d045a504c333efaa05322c76b488039b206edcf75aa2a1a3812 in / 
# Wed, 11 Oct 2023 18:25:57 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:45:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:45:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 11 Oct 2023 22:45:41 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 11 Oct 2023 22:45:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d2c869ca968be69328dfec29874eb48a467a69cd422adc8efeb8becda0764bd`  
		Last Modified: Wed, 11 Oct 2023 18:31:12 GMT  
		Size: 49.5 MB (49505948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844bb225a5a348ff23686694fbf59eaf37068ed24819e02d30c61bec857c081`  
		Last Modified: Wed, 11 Oct 2023 22:47:18 GMT  
		Size: 14.1 MB (14102923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8044ce3ea04c5947d141f918d281ac9008eeacac3f25ad93c15a863417945d9`  
		Last Modified: Wed, 11 Oct 2023 22:47:16 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64155e7810b4ad02035c50e244dc6333dbe0d31f00bfd84e224b6be053441b5b`  
		Last Modified: Wed, 11 Oct 2023 22:47:16 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ede91c5e4d86e0c7fa3ba7728a20d98e6f941def37db7cdd07f5740a5156cf`  
		Last Modified: Wed, 11 Oct 2023 22:47:17 GMT  
		Size: 284.7 KB (284674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; 386

```console
$ docker pull neurodebian@sha256:df3fe553c03f6cfd0da6a5d1aa6438189421e533bf02e9a9771dee9cb7132184
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65462536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a90070d3279d13d50e8c35865d0f3aa59f553833408927be212ca71b9938aaf9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:e8e1c13db04ddce5a6b3f4e29283e75eeecf85f213c2433ccb342a253457abc1 in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 13:32:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 13:32:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 12 Oct 2023 13:32:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 12 Oct 2023 13:32:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b15be2fd60b9adae282f32076fd2c71211d17ebbacfcd05f447fd925da0b81a7`  
		Last Modified: Wed, 11 Oct 2023 17:49:04 GMT  
		Size: 50.5 MB (50485267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e1b5c50d0eae63b22a19358100cdf59b202c84384683ac8aba451def7e4788`  
		Last Modified: Thu, 12 Oct 2023 13:34:09 GMT  
		Size: 14.7 MB (14691175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368d8bb9e3ee0f001af8e4687c69db619d8d97a18557427e30bd3df111808e69`  
		Last Modified: Thu, 12 Oct 2023 13:34:07 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8871ccd7ab3dfdecca636df48b9b597abf19cd53a667ec4a852c3e5233443ebe`  
		Last Modified: Thu, 12 Oct 2023 13:34:07 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94463383b7640cfd04fd8da81e0c9bf672266a85f032b7d676d8833f9df3695c`  
		Last Modified: Thu, 12 Oct 2023 13:34:07 GMT  
		Size: 284.1 KB (284083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
