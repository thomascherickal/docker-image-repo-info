## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:d2a2ae1159e5e98fab23316b1c87251ab3148fa02bd8dc35e0b4fec3425b510c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:7273039834b88053ebeca3c10c991a96e3c9527884c5b2327829dccf9327a076
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64714411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a8a2facbac503153a56869752b3dc14c8ef1ea00d9f784e8e6720fdd67336b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:56:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:56:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:56:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:56:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154f30b7649dd9ff36175e6592055cf8360c6e985876034a2272424287be1cd7`  
		Last Modified: Tue, 23 Aug 2022 03:58:18 GMT  
		Size: 11.7 MB (11650922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c00af28db2666c58eba10693268b55f170ca7e71d33f6cfe0d665fca65b1b7`  
		Last Modified: Tue, 23 Aug 2022 03:58:16 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f335f65a3d201956ff81ba9ecd2c1f5355df35fc67a4b449123d4d0d3dbf09`  
		Last Modified: Tue, 23 Aug 2022 03:58:17 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4abb7659ae1e8863abcaf9faf27843788a20b3d8a6ab97236c67a4ab6ae8e3`  
		Last Modified: Tue, 23 Aug 2022 03:58:17 GMT  
		Size: 292.7 KB (292697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:298d06f9fede57c37c75a2a15c45e367cfc4bf149b6b161348973624740271ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64856469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3ba2c11ffb710e401d30c92bd6e56a7d6169bb48780f8039be0ce102939a6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:38 GMT
ADD file:477966410dd9e274b01740d7af857db5c024b4c4e53a5e83b5da6854d5b0c209 in / 
# Tue, 02 Aug 2022 00:41:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:09:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:09:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:09:09 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:09:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17bcb8e39c7f35480d4c2e5b46b6c0a58dac180206453cc49052707aa8053632`  
		Last Modified: Tue, 02 Aug 2022 00:48:00 GMT  
		Size: 53.3 MB (53311787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b23f22c8c00046bbf67cd59cd4f2af07dce5c5fa7a24ab5543ae0bb3564f4aa`  
		Last Modified: Tue, 02 Aug 2022 04:13:49 GMT  
		Size: 11.4 MB (11445839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155e679260259d507584bee8d944d898d1181db2db8ee4e81b619ee20fe55dd0`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe48f40923db8199277d01e875d32310e9fc5ebbf9e02ea16c1397f9c07f2479`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707dc6bc4aa4606f4136b46e3735effc8020caaff4770ef7e70e7cfdc6946bd2`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 96.9 KB (96860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; 386

```console
$ docker pull neurodebian@sha256:376dad16c227357a26b95fa5af0a5b8386173d1e79fd72c29b8796d920a58823
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66173823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91aabef4df60debd2a22d26ff5f4e921904afa674132f60afb2577aa2996cdf9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:23 GMT
ADD file:40a2042e14b22d803da216af628cd6e8603c923c4fe79ca3c4c79c95c1c1e878 in / 
# Tue, 02 Aug 2022 00:40:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:20:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:20:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:20:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:20:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ef86b631f45587b4b6d1c16b80732997a4895ae8df072b14d68c25aeff8b901e`  
		Last Modified: Tue, 02 Aug 2022 00:47:20 GMT  
		Size: 54.2 MB (54195066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad56ce46d52bfd83905b2ba1001b937d0d384c2e9f52223b216e0205c495152`  
		Last Modified: Tue, 02 Aug 2022 16:22:42 GMT  
		Size: 11.9 MB (11879907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1643e5b63805dccebfbcaa3e8093baf3557f5e2d535c490c03e1dc32589240a`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e09ccea7ebbf3f00dff13f17b94a50a8828ca7a220bc06fca82b09fd996b414`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54f18cb63a52981a30664a1778e0a688a3aa900a519ae5ca7ec36351fd2ef6`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 96.9 KB (96869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
