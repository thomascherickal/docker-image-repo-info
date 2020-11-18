## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:59d21db48e633272499a8e555965cf8104faa8a16edba755736fe05b16846146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:72064c1f3766d2d1b2a1d4968837e0b5e4cbeae7d7b16a782a040f45585b90e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67376027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e9c08df692a7897aa86d59a6c74cc7dac99424cf9ff7278a4517d33e0a4b25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:09 GMT
ADD file:e5210ca55e6714aec9564543eeb4b4a748c57e62c0ae0c741dd0f3eb75ab72de in / 
# Tue, 17 Nov 2020 20:23:09 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:11:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:11:34 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 18 Nov 2020 00:11:36 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 18 Nov 2020 00:11:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:11:52 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:648de6ce4c8700aa65bb00de61082bc80448ba5410d2558ccd0f8c5e5616dbdf`  
		Last Modified: Tue, 17 Nov 2020 20:29:13 GMT  
		Size: 56.0 MB (55978493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae892a0f1e4279c8edb9dd1597c0e0941807854b7ccf684cc7940b186aaed603`  
		Last Modified: Wed, 18 Nov 2020 00:13:45 GMT  
		Size: 11.1 MB (11079994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42559e0d960b0a45b7049ff9df554665ad9452f284e0ae8c00a5e1e2eb025e3a`  
		Last Modified: Wed, 18 Nov 2020 00:13:41 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e55ac40ede7cc9d8ba2ab4b920a93873301688fa106e1fc74f7d8275df80181`  
		Last Modified: Wed, 18 Nov 2020 00:13:41 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576a505ac95102c295f68f05ff1cc89ff40c9e2a7538818eaeebe65a21dfcef`  
		Last Modified: Wed, 18 Nov 2020 00:13:41 GMT  
		Size: 315.2 KB (315217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5cca790147700bce0a4e3a5f3d28226d3cc2cdc3a898847c4a5cb0ba216123`  
		Last Modified: Wed, 18 Nov 2020 00:13:51 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
