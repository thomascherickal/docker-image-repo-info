## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:df24c3a68f97dd04a1269f01a57c7e82c479ded2271a878e6faf6303467f2a28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:88e6723270c2e83952eb1e8cb154c3b42c2eb60237cf1d638f0a7875c652f143
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64963217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24a1cc12f821c28df1e6fa6b69cae94b15fb0a4407574619c36235f29a3241df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:19:34 GMT
ADD file:e413c7d61ecdc96ab067e1f8bff6ce03c792c94b9d1f54e80cf633052c5d975a in / 
# Tue, 12 Jul 2022 01:19:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:57:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:57:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 12 Jul 2022 04:57:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 12 Jul 2022 04:57:57 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:55:48 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:7c7a32fcf1e30b18b7a9a032acf892763291bef7159859a35297bf81217bbee4`  
		Last Modified: Tue, 12 Jul 2022 01:23:29 GMT  
		Size: 53.0 MB (53022393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622b9e64a13adb2ec39801de6daa43bf1188cfd935031f612cb89c8120020347`  
		Last Modified: Tue, 12 Jul 2022 04:59:54 GMT  
		Size: 11.6 MB (11647040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb18285d163a3e7c2adc17ff28b99d1d4a5929e73bb8c30683af77986b88aac`  
		Last Modified: Tue, 12 Jul 2022 04:59:52 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e95e4a223c5b60da47a199e50dd435545b3dada916b9e2b8aae3aeed6d6767`  
		Last Modified: Tue, 12 Jul 2022 04:59:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38f3844b946448047ddc8a537538ba4589325ed4f642b8d43bd5284ce345c16`  
		Last Modified: Tue, 12 Jul 2022 04:59:53 GMT  
		Size: 291.4 KB (291412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a428e3dfc05da5791533f0f83ad786bc79a78872364ba86b3e9c738bcff0c`  
		Last Modified: Tue, 19 Jul 2022 19:58:20 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5b928d7326029c78801f07bcc7b08c00aa748cd98b458866133a5ce90232fca4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63670580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ebd003459a1188344448b301d0e5910c25963e6667cc48a1ff3673a80c03d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:53 GMT
ADD file:56a82a6c91d29741aef57453822e5502a13bd7841a1b3c8936a6f7b5c0b80bb6 in / 
# Tue, 12 Jul 2022 00:39:55 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:13:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:13:20 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:13:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:13:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:13:31 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:73d3feb17dc47282a9451cf8832ac9c5a707630877cc6c832d9f5cf4d3e2d202`  
		Last Modified: Tue, 12 Jul 2022 00:45:00 GMT  
		Size: 52.1 MB (52128620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d19f91d5a7b2d0054c0bcb6db7d19236aa7fe4fcdf009a35697554c989d9cd`  
		Last Modified: Tue, 19 Jul 2022 20:16:44 GMT  
		Size: 11.4 MB (11443963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f5e2bebd15a41f8e8f3f48e370d082842f0ccfeabf6b5b14c7c3803bc340c6`  
		Last Modified: Tue, 19 Jul 2022 20:16:43 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455ce410c6ff6ea4432b355f70f24e3768b6ba6119441c24a73ae78965e6894a`  
		Last Modified: Tue, 19 Jul 2022 20:16:43 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfbde9dc7421ff740db55f3872383877490c9951bcd3f7ea1fd7f5e76f0584d`  
		Last Modified: Tue, 19 Jul 2022 20:16:43 GMT  
		Size: 95.6 KB (95645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6c3ebbef7db1e96267b6fd7a360267d2e6410ea8b1eeab9d612d3c33577128`  
		Last Modified: Tue, 19 Jul 2022 20:16:54 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:53f8af6d2d1e7fc84df9d035a2c556a5ac18f035c6160ad2c1fe9d965ac55559
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65977911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3f47ea34421b6b8abab8b1f8b72667764c5c5fefa783413db0a76b24438c8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:38:44 GMT
ADD file:80ec0e35d6a4c162afe79f40617b47f846a2eb2065f245a230447609d1e7c001 in / 
# Tue, 12 Jul 2022 00:38:45 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:09:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:09:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:09:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:09:55 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:10:04 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ec7f9e3ed305349e742c012dcd142cce637ef3525759fea18f30c5987bf0e2fe`  
		Last Modified: Tue, 12 Jul 2022 00:44:03 GMT  
		Size: 54.0 MB (54004076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8374589e9f20263a177a6289588494dcca579725fa4e36b830fcf55da8fe012b`  
		Last Modified: Tue, 19 Jul 2022 20:12:20 GMT  
		Size: 11.9 MB (11875820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858bafa9e96debdc2e3c0c4cc2e8a3335876f044fe4f7a2dc1e673873c0e8934`  
		Last Modified: Tue, 19 Jul 2022 20:12:19 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c830b33ddcd959e6e8589706d9af61812e0caf13f99b340ba891f69c2cf0781`  
		Last Modified: Tue, 19 Jul 2022 20:12:19 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46936cc02729f7e79d4466f5094f8f10c45480ee1bb91224fcf8273bddfeb012`  
		Last Modified: Tue, 19 Jul 2022 20:12:19 GMT  
		Size: 95.7 KB (95664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78e920a810d34b26b0228171078e931ccfe92b441af1b8caa1a8224037d3ae`  
		Last Modified: Tue, 19 Jul 2022 20:12:31 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
