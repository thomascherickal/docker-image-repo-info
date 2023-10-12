## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:0fcfce1e17a12a4e86346ccf759f7494b493f94aa9bfd23362a27529e36d4007
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:e6321804e22a00ac278a9fe828eebf2f0e5fc51895e955445e97752399135e5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64077242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc9f1fc5704faac1b7e7406c3012086b90cd279dc217db742f500afe116cd7b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:36:29 GMT
ADD file:0301a32b2b2f0af81dd4277b61ab0069818663e8ad39e59dec42f2a74e027eda in / 
# Wed, 11 Oct 2023 18:36:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:04:52 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:04:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 12 Oct 2023 00:04:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 12 Oct 2023 00:04:57 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:05:01 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:3997a52aa0dcbfc5a01686dece23fdbb32f74ea998359451f16034544761414c`  
		Last Modified: Wed, 11 Oct 2023 18:42:29 GMT  
		Size: 49.5 MB (49503645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc64fa2e37f8989a74e99ffb107aad254e7976873443f8a4bd5c99735c327a87`  
		Last Modified: Thu, 12 Oct 2023 00:06:36 GMT  
		Size: 14.3 MB (14287000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11c551cc6c41f9b4547f1e21c0a2dd4e7ab58e7eb543916c529698ec68c2115`  
		Last Modified: Thu, 12 Oct 2023 00:06:34 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1870f67e592e0be20d08c2bf9b688a27ae99d26899b2b7122dcd50d11cfd7b09`  
		Last Modified: Thu, 12 Oct 2023 00:06:34 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2285a1d3c3065086a0887974ed20b67a06b7d10ecbe3c5a53d6a353f776645`  
		Last Modified: Thu, 12 Oct 2023 00:06:34 GMT  
		Size: 284.2 KB (284194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b01ce625d79dfe8294587212e87ab97d821d8b7d954c21f1101889055b7991`  
		Last Modified: Thu, 12 Oct 2023 00:06:46 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:54482980bee69c3352033b93184d46a979048b0fb87280463f01677648a1821b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63895948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0697da882e6a65bf8e09d064d79b57066935f6734e05a9ef7aa3d449022f01b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:56 GMT
ADD file:c18e09bd64c99d045a504c333efaa05322c76b488039b206edcf75aa2a1a3812 in / 
# Wed, 11 Oct 2023 18:25:57 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:45:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:45:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 11 Oct 2023 22:45:41 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 11 Oct 2023 22:45:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:45:47 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:9d2c869ca968be69328dfec29874eb48a467a69cd422adc8efeb8becda0764bd`  
		Last Modified: Wed, 11 Oct 2023 18:31:12 GMT  
		Size: 49.5 MB (49505948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844bb225a5a348ff23686694fbf59eaf37068ed24819e02d30c61bec857c081`  
		Last Modified: Wed, 11 Oct 2023 22:47:18 GMT  
		Size: 14.1 MB (14102923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8044ce3ea04c5947d141f918d281ac9008eeacac3f25ad93c15a863417945d9`  
		Last Modified: Wed, 11 Oct 2023 22:47:16 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64155e7810b4ad02035c50e244dc6333dbe0d31f00bfd84e224b6be053441b5b`  
		Last Modified: Wed, 11 Oct 2023 22:47:16 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ede91c5e4d86e0c7fa3ba7728a20d98e6f941def37db7cdd07f5740a5156cf`  
		Last Modified: Wed, 11 Oct 2023 22:47:17 GMT  
		Size: 284.7 KB (284674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c67d26480e865cb0aea487916858d74700173a3527c042639724f1f60e1337`  
		Last Modified: Wed, 11 Oct 2023 22:47:26 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:8f4be44da1a1a678ffebdbf11da2f012beb0b6ba06c61b9839c190c5cc9819cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65462931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c38cc06663c0b8d35b612131e4b9609d90f12d4aa2d52b65657c1cc0c00dfe09`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:e8e1c13db04ddce5a6b3f4e29283e75eeecf85f213c2433ccb342a253457abc1 in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 13:32:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 13:32:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 12 Oct 2023 13:32:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 12 Oct 2023 13:32:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 13:32:48 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b15be2fd60b9adae282f32076fd2c71211d17ebbacfcd05f447fd925da0b81a7`  
		Last Modified: Wed, 11 Oct 2023 17:49:04 GMT  
		Size: 50.5 MB (50485267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e1b5c50d0eae63b22a19358100cdf59b202c84384683ac8aba451def7e4788`  
		Last Modified: Thu, 12 Oct 2023 13:34:09 GMT  
		Size: 14.7 MB (14691175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368d8bb9e3ee0f001af8e4687c69db619d8d97a18557427e30bd3df111808e69`  
		Last Modified: Thu, 12 Oct 2023 13:34:07 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8871ccd7ab3dfdecca636df48b9b597abf19cd53a667ec4a852c3e5233443ebe`  
		Last Modified: Thu, 12 Oct 2023 13:34:07 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94463383b7640cfd04fd8da81e0c9bf672266a85f032b7d676d8833f9df3695c`  
		Last Modified: Thu, 12 Oct 2023 13:34:07 GMT  
		Size: 284.1 KB (284083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb95dca79367cdfba77129d56e6c1ec7905e8f9593ed328e64154924eabf7815`  
		Last Modified: Thu, 12 Oct 2023 13:34:18 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
