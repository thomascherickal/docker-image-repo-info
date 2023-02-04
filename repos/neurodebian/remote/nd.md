## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:7050790325ed90cb2ad5504cb32bab5a362955e1d5939ed3bfc64f7c549f2314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:01733acc29a04a7faad8a1e09c1919fe6d8b71b7295bfd915b40d71db1fef847
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60972971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3b8a37b4ea661b89d5515f16546db1c84db93ec0646df453320d9b0691f370`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:41 GMT
ADD file:3bae49887734af64f153e9e3668684efface6dd04ba31139b3d6b3aeb7589128 in / 
# Wed, 11 Jan 2023 02:35:41 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:24:02 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:24:03 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 11 Jan 2023 06:24:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 11 Jan 2023 06:24:07 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a0e522725e09a558b80e5d58e7b360150ad3fe901915db5358002bba7e461b9c`  
		Last Modified: Wed, 11 Jan 2023 02:40:40 GMT  
		Size: 49.0 MB (49040747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b093824ed1f576c50312d2531a60249f8b342a49baa7f5f0a9d9a6b9cec0b70`  
		Last Modified: Wed, 11 Jan 2023 06:25:54 GMT  
		Size: 11.6 MB (11649490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2422ed7b998669c36c668d35db3cf1da32dc2a1f5711146a19f303ec480fcc`  
		Last Modified: Wed, 11 Jan 2023 06:25:53 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcfaa5a5a9c6adc89eaf021d00c00b9020445247993e0a90f958212bd60607e`  
		Last Modified: Wed, 11 Jan 2023 06:25:53 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e726242bbd62259ba52ab5e26c3bf090f9854f4eac92df4e9af5e3799256c7a`  
		Last Modified: Wed, 11 Jan 2023 06:25:53 GMT  
		Size: 280.7 KB (280725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:6eb274643631939f13097c755fe3b8cf92bd7086309a009a638fbe6cd4c943a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60961349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d679ee54e61884acbc26f2ffce51aa67f4d41315ba0d0987a72d5f37fe00d5a`
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

### `neurodebian:nd` - linux; 386

```console
$ docker pull neurodebian@sha256:d406c7f2354a0571821073ce09f88b0158dc300fb165175daf29c7fd5ab65528
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62057792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c354a0fd7fcc315a4efc2ab10c76ce7706e7889a5a33c7d1506546e70e4829f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:17:15 GMT
ADD file:70daac43e15ae08f49ca2f191e46f20fb9df90f6fa25b199b61103e75ae43d16 in / 
# Wed, 11 Jan 2023 03:17:16 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:01:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:01:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 11 Jan 2023 06:01:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 11 Jan 2023 06:01:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:19edd03a92bb4010fb5a10c8cc739c02db9ae484e4e25247ce4b7e0977cf1e9d`  
		Last Modified: Wed, 11 Jan 2023 03:23:48 GMT  
		Size: 50.1 MB (50082487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f499715b73481f8ed830e3119b016f36fbff9017066f4501e5d2292e80ec6d`  
		Last Modified: Wed, 11 Jan 2023 06:03:18 GMT  
		Size: 11.9 MB (11881711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd3157fc8065bafacb7cea031b92ef19ebf4a95828b4891548b2ed70279d295`  
		Last Modified: Wed, 11 Jan 2023 06:03:17 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993baf5675aac33222c34733d36710a1a9a8989f8b60b85486f77fd339ee55f2`  
		Last Modified: Wed, 11 Jan 2023 06:03:17 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b981c6b645a66da18351c765208968b066e0172c6f98a173ff8553106121119c`  
		Last Modified: Wed, 11 Jan 2023 06:03:17 GMT  
		Size: 91.6 KB (91612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
