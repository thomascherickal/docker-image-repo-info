## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:5aa43e50b05324790c4781030fb4f97e22e8bfebaf355f351a2f200139d46381
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:24d0fb21d2a56378008ed0a52312fb574275b3911f1bb78c97b218067703294d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65167237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228485f820e3ff21f435fe95896f52fef2313b7c2570bf74a78d3a767330e97e`
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
