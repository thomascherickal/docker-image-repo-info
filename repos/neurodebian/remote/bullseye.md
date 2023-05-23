## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:58ede793451b5dcd9b8484cdf7a4d96286b7ca6dd4cd7691b09bcee139a37c03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:7f15da2016b618ea07c99f0db53a7d4d811f7d3a1e07b3dcfc62aa706a62d14b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d3c77884c39fcf8c8197b0e9da8509b340aac50f30d7d6f7927089ca89bbbc2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:42 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c8f317bbcc308a1e6f1fac03e1e3a9f2a39fc82e936c0570d59117b539f98b`  
		Last Modified: Tue, 23 May 2023 04:24:10 GMT  
		Size: 11.3 MB (11310985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339b1ccbf456e866652af2b8427b66dc919fc8ff09b50fc20bbadf9864f1299e`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec272ec7995fd0da0e4007df35052366ac83178183bc9be766a7c07054484d`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b179b6be05eca9ee18ca837dfeafb6f09c1357d864b810f767c3b8c7e6150efa`  
		Last Modified: Tue, 23 May 2023 04:24:09 GMT  
		Size: 312.0 KB (311996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:8e9a1ffc99ee63822e0d6d473744ca2ad41ef31639f50b2db48affd80c7cee32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65319625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a17259e4c5d36ea6062363803be00e2629bf3ed07156e49ed82adb0c75b262`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187c756d024d4e7c2776681889618e1a5149fc672ed0aac61d785f286e69cb45`  
		Last Modified: Tue, 23 May 2023 02:31:19 GMT  
		Size: 11.3 MB (11313121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0227cf7a0eaf0af3c3c1164de31c4c5555f9f5b511769db242fdc93b238f9876`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78eb1f7c1bac7ebaea871680d53583c59acee5339b44ced2f4aa3cb3e1aa6cb`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7532dbe02d3f898678b483d0df372497ea9472a859b411edd0993544bab9cd6c`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 311.9 KB (311882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; 386

```console
$ docker pull neurodebian@sha256:e013ecaa24d4606f907599811071f8b27f5c368a4f3b70509ff650713c26f7f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68050980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b877fcd3514ab2d8dc777764b898ba9ff9a8029ad45de0c1312ca006cec9a203`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:14 GMT
ADD file:acdf45f51b991111aa6c929fedd4e8de03e5d42578cca2f895f74697c3c66e33 in / 
# Tue, 23 May 2023 00:39:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c377769761bd9f2bd79d27a4f6dfa29be1047f4e6e8df1653027ef5262e020bb`  
		Last Modified: Tue, 23 May 2023 00:44:01 GMT  
		Size: 56.0 MB (56029173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaae1eed722697680293151e7092e07fa7042893bd549883ec3cc9b401babf0`  
		Last Modified: Tue, 23 May 2023 05:44:13 GMT  
		Size: 11.7 MB (11707960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c029d5297bd9708c2063123e4843df78700aa651c8968e98d0bb366528c3a761`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf405f235e316c73593fa6527a595699f0597ddcd7b09a16cf17b7c645e3b76`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a472eab1c6eb96814a14e198ebc46c183ff9b9b7a4b5244cd7133a8db20481`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 311.8 KB (311833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
