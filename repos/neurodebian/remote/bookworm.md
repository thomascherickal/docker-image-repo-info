## `neurodebian:bookworm`

```console
$ docker pull neurodebian@sha256:305a88dcf534bf4b940a7ec6db90d6ee025c6e6a483c09dd5ad63c711b84f6e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bookworm` - linux; amd64

```console
$ docker pull neurodebian@sha256:0f5a03a1e2b92ae1e0de0b26931de84428593d873ee4ef9935ac98d6971332c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67194760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74109098bb2d29c49ba1858321d2f58554be704075871131e3abcb634f537700`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:42:54 GMT
ADD file:b5180fc4d45b984afa69f3cdfa95980bcdfd76d75f704f74f1aa60e416272f1a in / 
# Wed, 20 Apr 2022 04:42:54 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:09:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:09:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Apr 2022 10:09:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Apr 2022 10:09:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8cb01d170a54a4c7fd7c1969e79df0a453468ebabfe1d860b863f7a3b6fbbc2f`  
		Last Modified: Wed, 20 Apr 2022 04:47:18 GMT  
		Size: 55.6 MB (55578729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5f3a12b5a1f781187474ee306fb16ff881deb5f4f6d47e9114754b8d087982`  
		Last Modified: Wed, 20 Apr 2022 10:11:45 GMT  
		Size: 11.3 MB (11306666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b0fd47a358971a676606a7707c75ac7b055feeaf4089e1a1281a9cccf5af7d`  
		Last Modified: Wed, 20 Apr 2022 10:11:43 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c83f249693e521108cee8fa3486ce9a3b4f1956657877e7d08b657f962d574a`  
		Last Modified: Wed, 20 Apr 2022 10:11:43 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59b5d37d14dc4fe45330391b6b191111d88e9b6a2c41443dd14516c06b3bc00`  
		Last Modified: Wed, 20 Apr 2022 10:11:44 GMT  
		Size: 307.4 KB (307354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
