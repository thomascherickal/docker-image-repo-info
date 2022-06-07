## `neurodebian:bionic`

```console
$ docker pull neurodebian@sha256:24dbb94d281291cb1e04b6108e5eaca921dfee07b976021bf1dccd7d516833b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

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
