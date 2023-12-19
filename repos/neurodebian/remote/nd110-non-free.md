## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:2cce0daa7423ab3c692c4904edbe4ca12a6f0bbc3a7d159b20505d0b80798dc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:62f489eb5479e968e8c7c95925b27de9a00e0c8feec115dca3360e7fc0e8577c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66679629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982a6feac3daa4329dd853bb3f5ce5e6aea98c80dff35c9a691ccc6703f6c0a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:58 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0856bfbd37c04c98dbed2cfbebaa2c7f12b11d4603e1cb62110aeede128091`  
		Last Modified: Tue, 19 Dec 2023 17:27:32 GMT  
		Size: 11.3 MB (11311904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5429bd5bea56c5bc55594233fc233733046f366dd1123c4a94b04f92f19228`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aecaaacf549bbf53913c6f0f497a5439b394e793b413c0cf0c796f9a040148`  
		Last Modified: Tue, 19 Dec 2023 17:27:31 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfd707f03ef0ab3405a9b45e6cec06e69f42f362ca8170ed6ac867bb3cfc5`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 308.0 KB (308007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe21a9c4f2844b1731353c2ccf79ed576bb765bc5854eab55e8c885e783c04d`  
		Last Modified: Tue, 19 Dec 2023 17:27:42 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:c0d28e0c05ae9c84fb89006bd6effeb566b7b36c125e840469027ac858a2fea0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65331998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e6683e8b8d8ee63d5c5efe716a4e5f08c490c43604cdb1f28350b960ae8b32`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:06 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:12 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a678807dec42582e887390c579155f2ff3f3c25b0fdfeb11854c487bfc0479`  
		Last Modified: Tue, 19 Dec 2023 03:07:34 GMT  
		Size: 11.3 MB (11313652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2434d66e0ac932afe623ab8fb9ddeaf97131cee80959a55990df31cdcbf946`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8665dd0adc074adaedc5ecf6d1a9424f986359c007f4c36cbcae0e95056a940b`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9cb0c2c79d2d93968c00288fda1bdc0a21e05ec517669fe68234be55ffd271`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 307.9 KB (307878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2849c1469b7eddd754a21b835849faa61f22936935882ba932182e1166a8e`  
		Last Modified: Tue, 19 Dec 2023 03:07:46 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:3525dcc77a6b6f044fb762f2a30c6e1d94790d1853116ce54032830935b37d73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68065268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bd45296a7a75d68f3b5963299ba70aba200d208e0dfe56532f768a6a9ee1cc0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:19 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Tue, 19 Dec 2023 01:39:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:18 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0a042ddf885a246973867761eaeb7097c4ffba0155dc9ecd3c004dd567e6d6`  
		Last Modified: Tue, 19 Dec 2023 03:52:41 GMT  
		Size: 11.7 MB (11708784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b236339ceeaafd4e56a9404e9528b71ad8f45255c5f053e303f89715c4f09bd`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca1d30df83fb1854dac8182f65566474d229cbccc4c7a4029273bddd4829d`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c554dc1a2dd646999214a1df9a3c0747d1dfb49b0931fd602f90f37f7f2ba84`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 307.8 KB (307775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b230d20e89abb46584252eccc63bcf58afb7c16c9f0fe85da93d4a3b3f28442e`  
		Last Modified: Tue, 19 Dec 2023 03:52:51 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
