## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:d1695cf30bdfe468656a4a3daf3baed64ba511f1c7c169cfd3060692286cb9d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:7b87019ae75369bc1d4b7bc684993d16714f4500c1c49cccd126d06aad2f6d75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66672485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b136a8573346edc2d1b25937a3310b3a9dca281065979f9bf3040ce8596450a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:13:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:13:28 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 25 Oct 2022 04:13:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 25 Oct 2022 04:13:32 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed2c6a9f12c16bef8e9d62b2f3919ac5cfe7e4dcdd2a410c5d1512470357546`  
		Last Modified: Tue, 25 Oct 2022 04:16:19 GMT  
		Size: 11.3 MB (11311651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32085ba5b820cb53d95f1c5a64d3d44cbe004ad8a7056e472f598b69831a4ec4`  
		Last Modified: Tue, 25 Oct 2022 04:16:18 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f70df6cc7ad4d9bfaee7502c94223d7de09183ffebe612ee0ab3d6d6889f94`  
		Last Modified: Tue, 25 Oct 2022 04:16:18 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd775cdf48cc3d8cdc1cf2b8241d7861683a6829d2a99a0ee00989807b1b2420`  
		Last Modified: Tue, 25 Oct 2022 04:16:18 GMT  
		Size: 312.5 KB (312491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:549507692b43319c3085c66c184331a3690843651c9856f1f1a451b2822abb7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64912635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3771988b0944a19a09d4efadebfc7d8a9cfbb1195dbd0f65a981d082e17e6c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:54 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32748b0f6967d6d3a663ec439e7a0b631ffe7f6e19fe0a854fa9f60cfbd8013`  
		Last Modified: Wed, 05 Oct 2022 04:02:54 GMT  
		Size: 11.1 MB (11104845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2cd3f4776c95e95f8cf2fe1866ba88b1f93d61bd9cf77c2b0454c13231a54`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74195093fe58a8f1f862fdb46f29db25a349b6d544a17872538f43ed9f69314`  
		Last Modified: Wed, 05 Oct 2022 04:02:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bb772dba620ade3ee2ee0b39ede83b9e4e52271a3c735aea72ebe200c60d9a`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 105.2 KB (105178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; 386

```console
$ docker pull neurodebian@sha256:faad9fd73720614aa3571453130adab314a1337233c23716ea029d9c8f2f5262
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67630593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82bebd1ae720b0a3624a349c8605a9c423db494f38f028eddfdfc8e500ab3db9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1913722e4098b05a88200af242b3e4de75036431d863b1330ca708cec7d52fda`  
		Last Modified: Wed, 05 Oct 2022 02:17:23 GMT  
		Size: 11.5 MB (11499735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16eddaf2626ebe571c30e863702e069074b6e5a9a22488db55e5d6dfdb41fdf8`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b6358b663dae0a2653ca7146baf655ba0e0e1b765ac7cc2914cdcc4390ea7b`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2069c1e6d4aa4c4d2b785d1396e8487db0a8e83ff092b0fae2d0454a2d6b9a2`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 105.1 KB (105067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
