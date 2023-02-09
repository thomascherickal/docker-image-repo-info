## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:e49be3797df78950663c99383b242ecdb280aac33088c95d854db1b4cd93eb04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:1d4623f580034954fb9ae2a6581693e907b81515de59dbce4828b3fa0f7c237b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61219162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014f69502a0fadd5f7f6eeacbf6b145d2391afe2b7afeb3d39bdccf6f6453351`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:21:29 GMT
ADD file:b3a4ee0f0fbf2d8fbbab0aefd91aa4d658c41b09c8a2beea1024bfce5e7d3fca in / 
# Thu, 09 Feb 2023 03:21:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:54 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ca2c7deeb5af7aa8a0aa3358218901c07b10bb98573151782e5e7af0ab03009c`  
		Last Modified: Thu, 09 Feb 2023 03:26:46 GMT  
		Size: 49.2 MB (49234515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8364caf5a58b2deb6126067cb35d010bad611576893cd5016c15f73077ed6`  
		Last Modified: Thu, 09 Feb 2023 10:35:29 GMT  
		Size: 11.7 MB (11700970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d427fbbb2b26c4a76ad11c5aca1a15a6e3a3ce0ebed9bb368ac16aa4b0a201c4`  
		Last Modified: Thu, 09 Feb 2023 10:35:27 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaccf87aac953e023363d8b331021aa3544b998ea3b8a32099f54494bf17268`  
		Last Modified: Thu, 09 Feb 2023 10:35:27 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d98dcb68c6cd5f7564faf602448779dafa9193a157852d3d9b0cb9194ff14a`  
		Last Modified: Thu, 09 Feb 2023 10:35:28 GMT  
		Size: 281.3 KB (281270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d986c1719d280776ecb8e97d8c6f14bd2def0d6f2263214410856de069a22796`  
		Last Modified: Thu, 09 Feb 2023 10:35:37 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:0dfc6d72a79ebae3679ff6b7311d814ad650c536b908466f05bfedab09c0c447
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60961744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f8d4407ad794329f99fbc45860becd38ed0ebb95f343004673e640cc94f0e34`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:18 GMT
ADD file:e0f39d8fee93f482160beca25b949b1de50ecc55ac86b1c276bed0b5c9955393 in / 
# Sat, 04 Feb 2023 06:18:19 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:49:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:49:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:37 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:541de84dec560e0a7dc13f9e5246f1a165b0955a6aefdc92d0bc46a50138a249`  
		Last Modified: Sat, 04 Feb 2023 06:22:53 GMT  
		Size: 49.1 MB (49064951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feef954a467cdbd9442f76eae26dcce65b43e942cf51fb0fc9932a2ce11a37a5`  
		Last Modified: Sat, 04 Feb 2023 08:51:11 GMT  
		Size: 11.6 MB (11613149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1fb0ddc7c21670259cb7fa6d33e4a66293440c6bb9ac9b12014f6ad578ba76`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b3ab955b5154981b3ebc74d79cacb2c050f8b3045d9e3b9bb5d5b3c6d69a3a`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e036d4fa82c2440e6b7a89404b4a9cdf679911cccfc91b67183e47fac4bfe42`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 281.2 KB (281241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69955de265518b9a0350d0446a8659f1d17fbd7262785ae52dae2c7b501b6e42`  
		Last Modified: Sat, 04 Feb 2023 08:51:19 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:a7055efcfe63c64c27f2d87abf8735eb755fb868a8741acf37a3d7f454513e92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62313023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9887da48d9004339e187c7ffcab2d5c6c4ca7fbc748db978d079cfb9ac1777a2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:14:01 GMT
ADD file:9ac1978405b6f0a95e33d1c34f01be82bbc11fcce2878747e4f688335279964c in / 
# Thu, 09 Feb 2023 05:14:02 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:44:18 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:44:19 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:44:20 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:44:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:44:30 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:e58ae2871ac91256d220f3da2b9736b2afb1a06906579876546cfae103647f95`  
		Last Modified: Thu, 09 Feb 2023 05:20:31 GMT  
		Size: 50.3 MB (50285434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2a120090af691fd4e5ade938037157e5d29f3d11e3c3fd540b83e8f5a65011`  
		Last Modified: Thu, 09 Feb 2023 12:46:22 GMT  
		Size: 11.9 MB (11933559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93706304552ccb0d7cebc8928c9d0832dbd0daca00da28c190209bade85501`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065c687c96091f2284561bb5a43d98da272ed8a551560f9d647cf28c84137b8`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe14b41a09e2614c0ecf5a7a46afa8824cb42dd8a5503453498ba712306cc7b8`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 91.6 KB (91647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992b26ef35e55050f48421f0d0441414650d88f959be0fe5cc0f64dc9aa920b2`  
		Last Modified: Thu, 09 Feb 2023 12:46:31 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
