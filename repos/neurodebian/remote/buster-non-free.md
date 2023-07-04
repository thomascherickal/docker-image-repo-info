## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:6fc7c554df0f8ec81a46040678e4a0bc2be29e8384b2c3eb824541d564e955c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:3beb6eb835fc85250784eaf181a8f8442fea08e2f3aa80108d7dde6b2bc72767
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61259760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f39d598e139315dace03a80d4bcdef913aca8886793228ecf7db0ef1a1675b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:19 GMT
ADD file:54838b3dbf7839dadd0b29835bbe53ecbfdfde657ef8671ec5ac3cf5867ea069 in / 
# Mon, 12 Jun 2023 23:21:19 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:12:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:12:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Jun 2023 07:12:25 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Jun 2023 07:12:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:12:32 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ac8bb7e1a32398e26c129ce64e2ddc3e7ec6c34d93424b247f16049f5a91cff4`  
		Last Modified: Mon, 12 Jun 2023 23:26:48 GMT  
		Size: 50.4 MB (50448512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd55e0d52139f2716adef2646b22f6817ed7cbc53af76173b96903eef04452a`  
		Last Modified: Tue, 13 Jun 2023 07:13:53 GMT  
		Size: 10.5 MB (10504527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f63b4a532d30401d4c0c6ec826c4682102ca79cb07b5f62b161722331fc57a1`  
		Last Modified: Tue, 13 Jun 2023 07:13:52 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c22ebb0e828bce675d01c201519636bb9e91a37861a3f769ce1c40d757661b`  
		Last Modified: Tue, 13 Jun 2023 07:13:52 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6b384379a945984dd8a312d280c821be714db2c33a1f9299adc7812753e91d`  
		Last Modified: Tue, 13 Jun 2023 07:13:52 GMT  
		Size: 304.4 KB (304362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb95f2e7198488aa6796521abdc64ec7d356a54b23e0836f63f9e2849c24a4a`  
		Last Modified: Tue, 13 Jun 2023 07:14:01 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:a0252cd512d037e3053d4cf4e540ee0f877b320a5079e0e861ae03254d2e19da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60055743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac4010dc112ef79880088a91a195ab5203a453d5ce5506868767a836459b270`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:59 GMT
ADD file:a61276f534601d7b193af24e35c16b73a2913511d2b1ad997c9a8cb907685257 in / 
# Tue, 04 Jul 2023 01:58:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:03:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:03:54 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 04 Jul 2023 04:03:54 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 04 Jul 2023 04:03:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:04:01 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5e2555ae6edde2e7933c533234cb224b6d7ef3a3c90041851e31fe29ab7197c9`  
		Last Modified: Tue, 04 Jul 2023 02:02:18 GMT  
		Size: 49.2 MB (49238644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d531d25790825e41444bb69f0bb17e2b5df75a15de0298dcf3989655d6eb7b75`  
		Last Modified: Tue, 04 Jul 2023 04:05:58 GMT  
		Size: 10.5 MB (10510379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461e85bf7126aee3bc32065bc89583822e1a8475ec7944d58970c9680985d399`  
		Last Modified: Tue, 04 Jul 2023 04:05:56 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11727db7413c0797ab3185cc121327037478eeadfd63bc1b28ca6dd4e4c61d32`  
		Last Modified: Tue, 04 Jul 2023 04:05:56 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949944ffb995b80048a3b556a86dc236acadcc632d995a23e76d0665b23d402f`  
		Last Modified: Tue, 04 Jul 2023 04:05:57 GMT  
		Size: 304.4 KB (304351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a954847d698dbc608e12c380f76e1b5aa3f1f166e792278130cd6bec8eef7e1`  
		Last Modified: Tue, 04 Jul 2023 04:06:06 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:e955b46f93d7869420168bd95f5292be5718a669a814807adce344ca33728efa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62380976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30d1f0abb7af1039948bae90ac516c37499c15fc168dc988b34e3921e2150a21`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:16 GMT
ADD file:c4d7ce8374a492278fd0b54ca10fd35f995676380e4ef134e484fd85ed50c58b in / 
# Mon, 12 Jun 2023 23:40:17 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 20:17:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:17:40 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Jun 2023 20:17:41 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Jun 2023 20:17:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:17:48 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:121d519ab26049cf059ad8c480f995a2bb103d39a5b57857d7ac27ab2b0d35f0`  
		Last Modified: Mon, 12 Jun 2023 23:47:27 GMT  
		Size: 51.2 MB (51205988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb428aec28623e7a6a452fa9764c92011de628a16c3be371229142d90f08430`  
		Last Modified: Tue, 13 Jun 2023 20:19:21 GMT  
		Size: 10.9 MB (10868299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c9bfd1d98db4e6e1c5e9369ce1799ab13acc0b7604d1716efc8620aa63d7d3`  
		Last Modified: Tue, 13 Jun 2023 20:19:19 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5f946b6887836f478a5faaef5945545878309f58cdc84bb87a8282f78a2100`  
		Last Modified: Tue, 13 Jun 2023 20:19:19 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e30e5e59e7737834638fb1552064160d5bb1249b4acc5f0586e28a19deb650`  
		Last Modified: Tue, 13 Jun 2023 20:19:20 GMT  
		Size: 304.3 KB (304327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f2d3be2912f8492540c97676ff434a73e9c08ed0e9936fefb8e8d483d098b0`  
		Last Modified: Tue, 13 Jun 2023 20:19:31 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
