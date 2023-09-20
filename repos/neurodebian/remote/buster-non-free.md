## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:e16b3a776cdb308b661e176a9f6932992c40c47027b2894de1ad280ff7fd7c2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:c3f765b94ca2d02079796992c7c8e36e72da9d76da5eaca84ee740d669ce69f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61304766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7040d81a099c518caa29d04df24c3910b883a8013fd1b923e5d3b7b4ce3f0620`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:13 GMT
ADD file:5a868c8105f7b621ffe46e19453d846faef824601a70979f6ef2bb46076151b5 in / 
# Wed, 20 Sep 2023 04:56:13 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 05:56:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 05:56:48 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Sep 2023 05:56:49 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Sep 2023 05:56:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 05:56:57 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:0dfc3f78750b97e03b66f316b37e155e3de173a8ac79942f0511888531fbe5ac`  
		Last Modified: Wed, 20 Sep 2023 05:01:23 GMT  
		Size: 50.5 MB (50498165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b41b837dc61a18e66e49f183d338aea00f298efacb0491f785b2f80d45ebc7`  
		Last Modified: Wed, 20 Sep 2023 05:58:26 GMT  
		Size: 10.5 MB (10504796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace23b2af1946591ebbbf04718164966cd3e11fdc258c372a6844f86f30d23d7`  
		Last Modified: Wed, 20 Sep 2023 05:58:25 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ac5d44398ea359322d47e2cc412a868650c1c33327adf181b871d7c101a4f0`  
		Last Modified: Wed, 20 Sep 2023 05:58:25 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c562aae2642187cb97671490d0fa6d2e11f329bcf3bbc8335592b4d5c4730aee`  
		Last Modified: Wed, 20 Sep 2023 05:58:25 GMT  
		Size: 299.4 KB (299441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977979133f4a18ca018cc5f8c92ad3ea754681458f2cdb343b43f38564f93dac`  
		Last Modified: Wed, 20 Sep 2023 05:58:35 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:a3acf0d3cc3de4bc954cae42521ccdfc73aa281b8413a571b686911c7c6dd52d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60103343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8396aa15738812f256e416237b6edf56f7a05c82442a5f5dd883bd5e7953bfca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:34 GMT
ADD file:3ec160f0e210563bfac108f23e5034dda5bc7b513b824ee276e4fc6daf80c89e in / 
# Wed, 20 Sep 2023 02:44:35 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 16:38:55 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 16:38:57 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Sep 2023 16:38:57 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Sep 2023 16:39:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 16:39:04 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:acd8b5ac4bd39653c2ebe6bd243f4ad2ee504ec9f8feeda9ef727446baf30721`  
		Last Modified: Wed, 20 Sep 2023 02:48:30 GMT  
		Size: 49.3 MB (49290887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5cf4d9e8764859480212179a73cfd2711a89b9c0160816969a1d60a4562444`  
		Last Modified: Wed, 20 Sep 2023 16:40:25 GMT  
		Size: 10.5 MB (10510625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9728c44b795090956dc89bd643b7ccc54099c5402892e116c4f730c000f0f57`  
		Last Modified: Wed, 20 Sep 2023 16:40:24 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac80e3b2d197f8ac212253fd30a643499c3e28295c45f397680d68c3b9491f9`  
		Last Modified: Wed, 20 Sep 2023 16:40:24 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72eb3a4074a16ab283a5151d7e700b6bb29accd9a2c01a0de32145c5d33588b5`  
		Last Modified: Wed, 20 Sep 2023 16:40:24 GMT  
		Size: 299.5 KB (299466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6085794a044c1573521a84ee68d09170a87dbc632bbc2d6902f0ad0aad80bc9`  
		Last Modified: Wed, 20 Sep 2023 16:40:33 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:19f91d5ee133f9aabadb643401a6381aba9889ccd02b9f9dcc4b62069eaa99d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20b665ecab14e5886e27d56319dd646cd702b8ec8d40794b11d5578c84906e1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:29 GMT
ADD file:6603eb215d695ca693056401592eb42db80ae6d6fcd314b50322ceb7858c1f2c in / 
# Wed, 20 Sep 2023 00:42:30 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:50:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:50:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Sep 2023 15:50:12 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Sep 2023 15:50:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:50:21 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6be8533983dbe30a84ca98eed25142115c1c6e36639d1e5086fd77e3332abc10`  
		Last Modified: Wed, 20 Sep 2023 00:47:58 GMT  
		Size: 51.3 MB (51255415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67498dc1adefd160a039a8adbc0bd2286cb9aa4f836d52d29a196a826e264ded`  
		Last Modified: Wed, 20 Sep 2023 15:51:52 GMT  
		Size: 10.9 MB (10868432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50fb22897c317d5f10be78081ea623fc7d2ee80545630e2c2ccb88678bf6ed1`  
		Last Modified: Wed, 20 Sep 2023 15:51:50 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69ee5ed14e2116b3742cc47fe4a1473f70bf94708832c91bf861633c3811eba`  
		Last Modified: Wed, 20 Sep 2023 15:51:50 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f73703175944520327704c5082b0f49d1bf711e10c7fd0b953a8638aa3781`  
		Last Modified: Wed, 20 Sep 2023 15:51:50 GMT  
		Size: 299.4 KB (299412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf6e337ccd966599b1bdb17176e78effc2da54cf72d87f6f50ed877c17a93af`  
		Last Modified: Wed, 20 Sep 2023 15:52:00 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
