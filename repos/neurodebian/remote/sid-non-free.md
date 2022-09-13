## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:001b0ce9dc3b27788f33016b632415ae4ac9cf3a91504e6af260a48fee8e9847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:e466f7dbd3de62a843682246318539d8d8cc23653a253008887805e8cc76d3c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64687104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81848706649fb2dbee852abdf0bb3057a7a91e27e1a07658c87cf4fa3cf53e79`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:57:16 GMT
ADD file:7b7161ef988532de9a1ae3caee50f4337a445cd5d88bfe1da455ad45111e2a4f in / 
# Tue, 13 Sep 2022 00:57:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:43:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:43:28 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Sep 2022 13:43:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Sep 2022 13:43:32 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:43:36 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:fbb5199f866b772d7999f8d0fead2c513b95972d6d32ec2c8e29311458f0855f`  
		Last Modified: Tue, 13 Sep 2022 01:02:12 GMT  
		Size: 52.6 MB (52643556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fdfaa6048bb74e484185c6a2954a2edc5c86707c9e5ec0ee4a78c9fee115d3`  
		Last Modified: Tue, 13 Sep 2022 13:46:01 GMT  
		Size: 11.8 MB (11756683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f92f815ffb1fd449d2870306889921b418cf343bec3f203c29bbb28e4b117c`  
		Last Modified: Tue, 13 Sep 2022 13:46:00 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6369fb38d66c84bf934264cf2fcfd92ffaee5934d4ac2465e27163e3faa1eaa2`  
		Last Modified: Tue, 13 Sep 2022 13:45:59 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb375eef344b1f9e5aa7f70e064e12273ee09fd30619de99b643554fa27a606a`  
		Last Modified: Tue, 13 Sep 2022 13:46:00 GMT  
		Size: 284.5 KB (284457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1499a48c8db15a545445a4000ae198f80bbb6f557316d43fe2e7bee4b154257a`  
		Last Modified: Tue, 13 Sep 2022 13:46:12 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:84c6e52209701f0956c0a509b999b4ac4c3088a7ed4c700cddc9b6c31f467912
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64727521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ca8a998e1d3135ef6bc441e3c5513eb42609b8f71927d21d8167612e90546c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:54 GMT
ADD file:13af7384e2c4f0c81e2c22e39e5d930dc4524d300c5f3d92ab3288096c308777 in / 
# Tue, 13 Sep 2022 02:11:55 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:06:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:06:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Sep 2022 07:06:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Sep 2022 07:06:56 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:07:03 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:113c8010a5d8650dba62a6df118557cb9b270a562e4a0537563cf79291f65ab0`  
		Last Modified: Tue, 13 Sep 2022 02:18:11 GMT  
		Size: 53.1 MB (53103634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887dc674c5850b6755aee7251b98a2b33fbac3e6097796403e72666b0f7c48b`  
		Last Modified: Tue, 13 Sep 2022 07:09:48 GMT  
		Size: 11.5 MB (11525842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4a8e47f25bd59db866901f94fd5e79dd5334f9b9a90c1a5dd5e3debbc4f133`  
		Last Modified: Tue, 13 Sep 2022 07:09:47 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a671201db081d5c370e44f8b119968c752abb0c2b39978a94efa246a7e09700`  
		Last Modified: Tue, 13 Sep 2022 07:09:47 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48d657154fff6a70a3d5170015991747c2dfaf50e1c6a8913973ef8983c00ca`  
		Last Modified: Tue, 13 Sep 2022 07:09:47 GMT  
		Size: 95.7 KB (95667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce45b54b48cccb529a28c0a35b3c4c36be043b11945d0f62b90f2875f092f12`  
		Last Modified: Tue, 13 Sep 2022 07:09:59 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:a82927e61db526482f8c9873f8801473b3cfbf8cd8cf9e84fd33f06962c3e69b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66091207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6768e0c84eab9022340cf2b56df4fca4ec8417fc7ec182c311574a4114fe071`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:40:48 GMT
ADD file:6c1d0f31b3527c2c240577c73b2476b1c6bcb8fa8d10fea614680e40f1c15858 in / 
# Tue, 13 Sep 2022 01:40:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:57:18 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:57:19 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Sep 2022 06:57:20 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Sep 2022 06:57:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:57:31 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6d4ab670272048731963c87509c528d8f874ef24e7e5eb410c2b800aea0d16cb`  
		Last Modified: Tue, 13 Sep 2022 01:47:14 GMT  
		Size: 54.0 MB (54012005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5566e95e23d4754af775dba6ecf29425c2834643d6f2af010e156d7da5da9b36`  
		Last Modified: Tue, 13 Sep 2022 06:59:26 GMT  
		Size: 12.0 MB (11981114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7ac77f1571422d4dc459fae7d0cd8f0031fac99f4d6f4141fbcad8ff33bf00`  
		Last Modified: Tue, 13 Sep 2022 06:59:25 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536a36f731b3c2f82eff802367201770d96131d747b858e6fbe1f5848224bed4`  
		Last Modified: Tue, 13 Sep 2022 06:59:25 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f87618e59e6c601af0fbbaedc6e3395f48fbf90be466a188cc336c9fb0e5520`  
		Last Modified: Tue, 13 Sep 2022 06:59:25 GMT  
		Size: 95.7 KB (95709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc1a2d9b7b291e240057afd92dc9c34db48cc76818d3f18bd5979980174d839`  
		Last Modified: Tue, 13 Sep 2022 06:59:37 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
