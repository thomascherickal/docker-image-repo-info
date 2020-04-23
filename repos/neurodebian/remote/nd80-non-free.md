## `neurodebian:nd80-non-free`

```console
$ docker pull neurodebian@sha256:ffbc4fef8b691aa02f03a442ace09c1de3fb7f345cc103ef3845ce97bb5881b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd80-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:a4c003c1841a6c841e4b5a702a6d8e595e45f7b59ea8d352fdb7fb81a0acdcaa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54696734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6909aa7de96f36d0590253d5925cb8d76a4d707338a20019c6b457d16fe02bad`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:45 GMT
ADD file:545fa4a7e3efbc02fd93b103a922af1496dafa1358953302d1e9112772a46c6d in / 
# Thu, 23 Apr 2020 00:20:45 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 02:24:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 02:24:48 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 23 Apr 2020 02:24:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jessie main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jessie main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 23 Apr 2020 02:26:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 02:27:02 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:f4cbd35197708a9e2a08a980f6184996202108f81f5a0a2639bba1f4e070c56b`  
		Last Modified: Thu, 23 Apr 2020 00:25:23 GMT  
		Size: 54.4 MB (54390774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb3b1b9a540c570e89ba02e3fcdcb8d7fa46b31de2663eefdfabf4388133e93`  
		Last Modified: Thu, 23 Apr 2020 02:29:48 GMT  
		Size: 298.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21041039d056ec83860d9c67797fd0af80ccfd5d35cf3377d43fd0867dc0890d`  
		Last Modified: Thu, 23 Apr 2020 02:29:48 GMT  
		Size: 3.2 KB (3154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c924be277b9b363728988d796325bbfb53f23a1299abd4b9ee6a46ff0a5d9fb7`  
		Last Modified: Thu, 23 Apr 2020 02:29:48 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db4a94d30a4b02808333b5cf93426b64c6733e16dcbc381513bce34c9a5da4c`  
		Last Modified: Thu, 23 Apr 2020 02:29:48 GMT  
		Size: 301.9 KB (301902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854b0644935eac34f245051bffed4cb6742524be38d44104563e8246c6a555e0`  
		Last Modified: Thu, 23 Apr 2020 02:29:52 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
