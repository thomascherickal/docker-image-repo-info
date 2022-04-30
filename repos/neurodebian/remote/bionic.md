## `neurodebian:bionic`

```console
$ docker pull neurodebian@sha256:5a1bd2ac5b76ae945a0cac899c9f46957c7425f97d7501a698a6be1f328ffbec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:9008162399f5faad246cae7ea1247539f2ca3be00f72bfb90923803c97fdedf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31765851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ac28c18d97f948e77cd8da2da449193548c4ae243c4d777622f71ada5b0e63`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:33:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:33:20 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 30 Apr 2022 01:33:20 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 30 Apr 2022 01:33:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58583b539d46b7038202773a325819468be109165b71744af9cd7a6b2ce7b0aa`  
		Last Modified: Sat, 30 Apr 2022 01:35:23 GMT  
		Size: 4.8 MB (4813350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea30d87d1c9a9fd197814dcf12543419ec281f0f90d05d3aa45ed044c564ef3`  
		Last Modified: Sat, 30 Apr 2022 01:35:22 GMT  
		Size: 3.2 KB (3157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85142dccede946e5a0dbc51173c140df7909d56ad23c40ec8fcad485fc16d3ad`  
		Last Modified: Sat, 30 Apr 2022 01:35:22 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa1a1dbc1270f07c1df0fb94fe476e78e70ff0f5768675440c5ecfb55195410`  
		Last Modified: Sat, 30 Apr 2022 01:35:22 GMT  
		Size: 240.0 KB (239992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
