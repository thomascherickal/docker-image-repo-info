## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:706fd6004bb27a100017790756cd5ead82a1b25e6110e6aba1feae4ebf28738a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:089aace451cc2531330594326419c2f78366abc5f5f93379bccf82823a494dd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66975428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:789bab2c6212faa26ed18ff0337dbb9bfc15632aa3513309e07f5671d88274a4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:24 GMT
ADD file:fa865518757ef9e0af03796e7abd6cbfd59e20f5ae325422e41524615051a2d1 in / 
# Tue, 17 Nov 2020 20:20:24 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:11:00 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:11:02 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 18 Nov 2020 00:11:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 18 Nov 2020 00:11:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:11:14 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:d004aa4da82e9e47169ac4cccf33df9b52bef6dda8aa5f7b0bcb03af34078173`  
		Last Modified: Tue, 17 Nov 2020 20:26:32 GMT  
		Size: 55.6 MB (55578105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28dd32a475eb32ede09508462cc31859b1f7422477dcb8f22420ea8e8d39007a`  
		Last Modified: Wed, 18 Nov 2020 00:13:31 GMT  
		Size: 11.1 MB (11079912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2572dc0cacee04077da6a67312084471299ca8a3ead2e944c611966254b99cb`  
		Last Modified: Wed, 18 Nov 2020 00:13:29 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b366ac69b4673e7bce23bec3fda13eb5f2be0aca11968dcb5333497a0a0d9e3`  
		Last Modified: Wed, 18 Nov 2020 00:13:29 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a900b4acbe0fb86b8cd6ea990bbbae90442b67c295d53c811ccc6e3fe007d226`  
		Last Modified: Wed, 18 Nov 2020 00:13:29 GMT  
		Size: 315.0 KB (315031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a978e968019d06ba7a5870c294e72ef428f63323c6b9e1dc6fa325670fa4929`  
		Last Modified: Wed, 18 Nov 2020 00:13:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
