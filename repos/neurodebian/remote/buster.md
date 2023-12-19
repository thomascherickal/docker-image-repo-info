## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:ce0180be636220f3a87835ecb491e44dcac234df82efcbc10d099866b1617ce3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:a62b209877b5c5a25d335582b2bb1167bd12a57d812fbee47b395a35cc125699
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cec7c78b29b47c0541641b7be7d3eeacef33acddf23f606023369d26314c5c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:00 GMT
ADD file:e5e3f2fedf4fa6382f3bbf6203060ba68df1aadc7ebfa3350df20bf31b102f0e in / 
# Tue, 19 Dec 2023 01:21:01 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:27 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:29 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30b73a2ffaab3c39355a8bcc5eae8ba1465bd7d9467f197b91f7635816b16bc9`  
		Last Modified: Tue, 19 Dec 2023 01:25:58 GMT  
		Size: 50.5 MB (50500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab53549f1d6f91ce1fcfb5a6ff812ebeca69b02bd07cbe6a1ae8df426ca90a4`  
		Last Modified: Tue, 19 Dec 2023 17:27:13 GMT  
		Size: 10.5 MB (10504778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e731abcc54cf5bcb086bc36b1e6f12ad7d73ca0f0139f4a0070a16d1bb6105a`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f5821293636913a5e5f156fde6c19fb62901cbcf38d66898b3154b4222b9e4`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2c8d395609db22d85da949ac48af56210ff29e74765f2ae4f6f3dd8007e73c`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 299.4 KB (299435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:600d482db7b7f3d51d4f3421c83edcc89e1f2877a2a2eee0924eb54a7f2ae386
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60101042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a3893cecce63384e1d3f1b1992262b77aefdfae5aaba094ef03c980ff3b6a89`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:31 GMT
ADD file:df5e5dd39efc6ae3cc9132f6ca6bb569731f7a37cf4b41f87bcb7aa1ba9771e8 in / 
# Tue, 19 Dec 2023 01:41:32 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:05:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:05:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:05:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:05:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93507f9712ced9fbfd0d0f689cf7b55fb245cef88530c07ac5dc5cad20fa889d`  
		Last Modified: Tue, 19 Dec 2023 01:45:40 GMT  
		Size: 49.3 MB (49289026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c5fbc51c74a4f8750f148252ed129c0c57cc94d6e2b2f4ae83d5f1420fe9a2`  
		Last Modified: Tue, 19 Dec 2023 03:07:17 GMT  
		Size: 10.5 MB (10510551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7d0a1a828eff413800cec078c31256371b964ca8aa29198aea52bf930d8057`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dd41deea093d7e81d0007ed35420760c6cea45b552f575b45ee9e400eb7beb`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533e3cd401bcc7d93489b3ef17afb87ed22d96e3b19fb76fa2dfc90ee457c0c0`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 299.4 KB (299449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; 386

```console
$ docker pull neurodebian@sha256:ec322aa50424cc143d1686f5c149fa6a13d427e7e3a49126580823944e5101a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff097a81fd1e52e4c0c90fb596ba089dc94e8a830bd1c10c18c463bcaca93815`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:40 GMT
ADD file:4c009b0d408e3df297246382d87b0be68c34886e13ed79ba47feb8ff51acb863 in / 
# Tue, 19 Dec 2023 01:39:41 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:50:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:50:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:50:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:50:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8d351f5ab6958b8ca5f2b8e463c49cba65be4285ead8bdbc1378b5ce2c8cd736`  
		Last Modified: Tue, 19 Dec 2023 01:44:53 GMT  
		Size: 51.3 MB (51255444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01ee695ce5b07c4aa0b90a93605547e631e728141c311b4bbf7c54fdac3be4`  
		Last Modified: Tue, 19 Dec 2023 03:52:23 GMT  
		Size: 10.9 MB (10868372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379f0dec32e0488edb8bff0dcd0be9abb4c04675943257bc5c784bfd82fd870`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56e62a0bf8c627e0bfa8f075fdfdcabfd6fc8d4809a1ec507a91d81eec6c13a`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f016555c3e2050965be5f7aece4aa1a93943629cdaa4359707eb76a9fac47534`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 299.4 KB (299418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
