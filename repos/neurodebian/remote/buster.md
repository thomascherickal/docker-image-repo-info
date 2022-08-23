## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:71a2eae8a74514991dc69475e8ea75ed2a3c387d95755c13f9b821f821f273ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:ee2c68e9b6832fba5bf06ec089492493958657068ce57cccc7adbc59f61967f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61246561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dad9ac5a38a301180d4a38e1a47f2680657dc10354b71d4dc57b78e5a8f23a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f1f3483383008e9bdfdb0946317d5a1f06e96826631b67aad6ea88390f8f59`  
		Last Modified: Tue, 23 Aug 2022 03:57:13 GMT  
		Size: 10.5 MB (10501366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f071bb9ea0575e1048a0b93e7c9f6d2471dcb313b290eb2dc170274a5627995a`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30b909f6364845c06673d20a3679be820d2b7c92fa8fdc4ddee19421c2983e4`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cb4aa9dee1e926332df8474f45adde8fc0af961f37092953110a68b479fcf9`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 302.9 KB (302910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:8a5714488c5e8b7a754867d7ee61135da10dd8d42740155a6a1014e0bb5addb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59636766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c9ba384f3c57096357f1c97b80b7cab4076da999fd61c2972f5afa7120d06f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:49 GMT
ADD file:dfd7e3791fa0512f0f7c9cc8530233d6bc1b0a586a3656fd3950ea386754808a in / 
# Tue, 02 Aug 2022 00:40:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:07:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:07:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:07:56 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:71209d5eb534b9e48223962276993c68559f68e230f73c8a0efc2a2998362bd9`  
		Last Modified: Tue, 02 Aug 2022 00:46:28 GMT  
		Size: 49.2 MB (49229053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ad9175bab50a203372a0e5e18519ece155815088752e2900f451f9dd7792de`  
		Last Modified: Tue, 02 Aug 2022 04:12:21 GMT  
		Size: 10.3 MB (10297208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527a3912e4982e1d06db4d8b2f3d684833010e1d4cfc16801787b9fed69d31a`  
		Last Modified: Tue, 02 Aug 2022 04:12:20 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4199933e5d6634a8d460a6099aa3dbadee5483211ddc926a0da379fb5e417c26`  
		Last Modified: Tue, 02 Aug 2022 04:12:18 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9418e61ef8a7313b3cf88c397a2fb0a35dfc117517fa2d0ab5366dd3e54aa80`  
		Last Modified: Tue, 02 Aug 2022 04:12:18 GMT  
		Size: 108.5 KB (108521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; 386

```console
$ docker pull neurodebian@sha256:a708ad27908b311aad7f1b1d27134cbd2043ed3a5bea0037bd1ffc2dcf09fce7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a37832cbbb9aa939def4b2ef363c946e7ed92499feedef560c0110635c3e66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:31 GMT
ADD file:a25646092eaa55ba1e77da8bf292a71c17f8f54e6fa7a3cc057a8bd7d2febd63 in / 
# Tue, 02 Aug 2022 00:39:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:18:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:18:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:18:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87423d7294b9d02dc4a6174f8947a28436937897c107e94249f27f8c987b91b5`  
		Last Modified: Tue, 02 Aug 2022 00:45:43 GMT  
		Size: 51.2 MB (51204266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bde8b75add39bff8346a40cf19a696d90f83fc7b4d1e3c035b478656d7034b7`  
		Last Modified: Tue, 02 Aug 2022 16:21:22 GMT  
		Size: 10.7 MB (10669192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc885a3a4c2e7820a9531f2e81d8567cae93afa593b55a5463ca3a7ad84eb1`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5107873d404a90d6b95e3407b818195c97a7437da9b1681d920e70b2e94752fc`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b27a5bfa9663386e2233f61f36aafa47682e7e3a82789f89f624d252b95f3db`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 108.5 KB (108479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
