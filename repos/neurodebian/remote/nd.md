## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:3076bd759dcaaf48c55bfbe851b186199c007138b2ffa6878b99d549c0f4cb33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:72eaa2172d7b06d9cf398c5cfebb9f5ed0ead79a19f217572c987ecc980250bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64245379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bba5e2b1186af02ec519fbc2894ba188c724776fa994fc49a039a0239492991`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:05 GMT
ADD file:0e0fcf0b6bc9c9794502332cd0f45625ac991c8a06ab284afd8673f8d5ab789c in / 
# Tue, 19 Dec 2023 01:22:06 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:26:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:26:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:26:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:716f2525263989014ccf51727e00b6ee9f74018b7b13e996b0e06409e58a44a3`  
		Last Modified: Tue, 19 Dec 2023 01:27:57 GMT  
		Size: 52.2 MB (52246819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46595495b42823cfd778cfc3563c43755220822555cb22afac60d826272f92b`  
		Last Modified: Tue, 19 Dec 2023 17:28:13 GMT  
		Size: 11.7 MB (11710401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4996e7c637126b150a9569e1dd22c978b1c1e339a6e7d0853831f7d4b7cff2d5`  
		Last Modified: Tue, 19 Dec 2023 17:28:11 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1681fc2520614d5bf50a4f35cb2b68d40484e39379bf891fbdaea3a4a8fb426d`  
		Last Modified: Tue, 19 Dec 2023 17:28:11 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10da9506cdc97636bf343b88b8f41f346687505451481b89bda91ccd5edb191`  
		Last Modified: Tue, 19 Dec 2023 17:28:12 GMT  
		Size: 286.1 KB (286148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:dc92210bca05150670c4b103f4248092b98dc9d3ea8d8950d4b449472528f49b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7beb2b34e8aab8e7bf6e1a2736a1884f078694989962ddcfc1b9c3c1a1369b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:13 GMT
ADD file:b95bf5556d43a8a1d79a2dbf26ab8a4a912869d65cc1b76a372ca80259a65b7b in / 
# Tue, 19 Dec 2023 01:42:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f38ee39d2143cc6781c8d40b267519e59c558f7902df442f2e5ecfcefb01689`  
		Last Modified: Tue, 19 Dec 2023 01:47:24 GMT  
		Size: 49.7 MB (49689786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e289d2bd50130a54f42a5188139efd22f1e4f872bf3d2ea9ee64df6bbe8a2d`  
		Last Modified: Tue, 19 Dec 2023 03:08:14 GMT  
		Size: 14.2 MB (14163608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6592770f5ba6afac48334ec1e5b9f57d99a6972ab6ea31b37e445e6ed7836a81`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b92ab013a67f046cd17d84ea7ab3e4f6eedba968eef8b8e56083974801edbb4`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c053063e1b60822a02be21a864c0d45e978a421c861555ff8a276300ea58b7`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 286.7 KB (286688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; 386

```console
$ docker pull neurodebian@sha256:d7d1f07c58b1aae651c695df84e0da0a5f8422df9601b840a9901f84e8d33a22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65577251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f217e36f8007ed868e04aabe3583cda7a03dd90f9a32f5b29e6b88c8bd7c86e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:40:47 GMT
ADD file:736d4b14c103f5161855a9c14b05565523005af03b61bcfb3d6bfaddee9431f3 in / 
# Tue, 19 Dec 2023 01:40:47 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:52:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:567001fd97421e53b722a950bba83f44d7635056bc895f0b4f77b68d779fc15e`  
		Last Modified: Tue, 19 Dec 2023 01:46:59 GMT  
		Size: 50.6 MB (50559243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d5db5fdec42c82bcc5337d39f7bf6b089a42b3787d180eedd48aaf4d4a2bb`  
		Last Modified: Tue, 19 Dec 2023 03:53:24 GMT  
		Size: 14.7 MB (14729998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9aec2cefffd0c64a74a6846300482dea9046c877c1c1559aae5523f25d8610`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58ce81bf04c62ba5934917b776534fb6478af6e9325c3ee241a2345c0d800d5`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00decda9d198acc08dcefd5412a863c2625149c3aca917edadf313f6696f075`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 286.0 KB (285999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
