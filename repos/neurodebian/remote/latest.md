## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:334144e4900588244c63a7a258e110b4e377c1d95047e0fa1a3ce29bf075d6fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:413143670fd95da1939154a5a3c5e121578f46f23246da40a6ebb8cee429a6aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61241892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0e1dae6efbc6e0a891f6049d48bd8d60864d76d73ae2f266da7b2e7cb1e3715`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:40:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 18:40:54 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 21 Dec 2021 18:40:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 21 Dec 2021 18:41:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f9fdee196cecc5cbea113a8381bf3ffc111987debfb2bd5f201083dd18a972`  
		Last Modified: Tue, 21 Dec 2021 18:43:03 GMT  
		Size: 10.5 MB (10499972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4fb201e2ebe8939a3083c64b90223c5684f0dd58eeeaa420edebe6d17d667c`  
		Last Modified: Tue, 21 Dec 2021 18:43:01 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbf343e4dc9cf43f6bfec590ea6a52001e7a5482c25524831bcbc24612e0e90`  
		Last Modified: Tue, 21 Dec 2021 18:43:01 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34167a31df93ed2967db51b72a8ef0e0990705f95b2739168595e01a2200150d`  
		Last Modified: Tue, 21 Dec 2021 18:43:01 GMT  
		Size: 302.8 KB (302768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
