## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:f71ece400cb628ad9d4b0db27f7814eb1fafa92212ba5927629ae6dcd1de5cdb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:ff6d3620c1c66c78c0bbac1777a9210a12b99820500864f4c29c8bfb04022d80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65167634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f3fab281b752b2df58cdf2781f1eebc22dfae6c86b3e278f1fe01333b32562a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:21:07 GMT
ADD file:0aaeb8a0c7fde9f030dc2ab67a03f21f44e9eecad9e4cf1f360dc5f768292460 in / 
# Tue, 12 Jul 2022 01:21:07 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:58:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:58:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 12 Jul 2022 04:58:12 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 12 Jul 2022 04:58:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:55:53 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:4a81bc091a3ce5ccc3c89ef56e710ee1854c5ff9fd3d7f148e87cb956b5b78c7`  
		Last Modified: Tue, 12 Jul 2022 01:26:19 GMT  
		Size: 53.2 MB (53226349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514b4a73206bb24c6c1a61317455ad4b96a0018d17702e00ba50703b29820ca5`  
		Last Modified: Tue, 12 Jul 2022 05:00:14 GMT  
		Size: 11.6 MB (11647405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02230813fdadf6cdf443f7f92c7f0a828a76c7b448874ea87383ed635c1d148c`  
		Last Modified: Tue, 12 Jul 2022 05:00:13 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8267385aba6f2b02cb781b8b1f6808021c1af5aa73b1cf9b0e8988a821432438`  
		Last Modified: Tue, 12 Jul 2022 05:00:13 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba75a7980e02257e64e233724b2d8263c8598da79360d3142660fd9a3ae28e8`  
		Last Modified: Tue, 12 Jul 2022 05:00:13 GMT  
		Size: 291.5 KB (291473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e79e94c4767b94e3b6a77fe9ecc899cd5ee00a50eb99dd02290115f0659c12`  
		Last Modified: Tue, 19 Jul 2022 19:58:30 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:3f5300b224dec81ab647fd09d674d36322b700b5d89b4241c87d901246b3f587
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63874922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7c2ffc3ff5e75779d1a6dcd31a512bb15b50e84dfc5ed5f5c4b4f98b425c46`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:41:40 GMT
ADD file:0f18dcfe7e502abae9dd7f72911dda640e4675306760d63f467092f962228ad1 in / 
# Tue, 12 Jul 2022 00:41:41 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:13:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:13:46 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:13:47 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:13:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:13:58 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:d3ef27d3c918a6321957a64c33268d09a01ec18590cce79a144625d9c0c8599a`  
		Last Modified: Tue, 12 Jul 2022 00:48:17 GMT  
		Size: 52.3 MB (52331756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ec2d05f04c3538faf1252a53a3f8eafe0ff0fad3ab34779790a374564b0924`  
		Last Modified: Tue, 19 Jul 2022 20:17:07 GMT  
		Size: 11.4 MB (11445000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8572615350d6371e128aa042f6394472a1404c81eef41cdacff8348dcc384c38`  
		Last Modified: Tue, 19 Jul 2022 20:17:05 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395b84807b733fe258bbc2aa263b29c0a3d57649ca1a3dfc47573c283a0d5dcc`  
		Last Modified: Tue, 19 Jul 2022 20:17:05 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb3d7a9dc222e602bc86be4c0e581de2cffee89ea0ee03a579d456bd9336f56`  
		Last Modified: Tue, 19 Jul 2022 20:17:05 GMT  
		Size: 95.8 KB (95788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2dac13ec19481b8df21100d2ca22075901fb1e391ba654e308eb7c83ec363e`  
		Last Modified: Tue, 19 Jul 2022 20:17:17 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:ca00001dc234bc6177866cf599a70b7b3058158ce55f6647dd03892d5db3eb8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66183410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbed5ec4e0638f0bce865774b57738c9caa8ca6e1cd1189212e5615fc2e9d67e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:33 GMT
ADD file:f76df7d0d2c0977290a0183cbc4f62656ab20d04eb0cae4d075fd31ddf9df8b4 in / 
# Tue, 12 Jul 2022 00:40:34 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:10:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:10:20 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:10:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:10:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:10:32 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b7f5437d02adf5c6ebc8b31ebf7b4950c58003a838e1f6591ce754472a3bae43`  
		Last Modified: Tue, 12 Jul 2022 00:47:20 GMT  
		Size: 54.2 MB (54207595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cceee5781c9f099fefdd78893e31a26bd41859246858d435b15f686abc95d1d8`  
		Last Modified: Tue, 19 Jul 2022 20:12:43 GMT  
		Size: 11.9 MB (11877644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f601990e08e4e6b453747a5131289362248b1b66a2cf312e00428a6249a293`  
		Last Modified: Tue, 19 Jul 2022 20:12:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419720c8ad79105df57e634617745b4d24dfe22ed8055b5feec9e0375c63e978`  
		Last Modified: Tue, 19 Jul 2022 20:12:42 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad05b2cc3252576c38611644a853bba061eadb0faff6e2b261a0b63024ac2239`  
		Last Modified: Tue, 19 Jul 2022 20:12:42 GMT  
		Size: 95.8 KB (95794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2b88beb03c75a096c3a96ba91747e5707b9658f7dee6f2ac146af6919f7f2b`  
		Last Modified: Tue, 19 Jul 2022 20:12:55 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
