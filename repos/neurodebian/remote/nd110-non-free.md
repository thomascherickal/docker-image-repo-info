## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:5cedd0e17ae4823493af5c647d8a1f9a2b88491dc2ce799182e7a0bc2d769404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:e6506f40051fd389d3c9486cabb81ae5e2e9251966e2dd135c823bfd961f5f7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63086733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dc38836117d043c2739b5e8630cd620f3660f6e8585ad3045f121c99fcaf219`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:19:50 GMT
ADD file:3785e6fc0adaed3cfee77ab7dd0756681492573e3553e88b5225fc14d56562d1 in / 
# Thu, 23 Apr 2020 00:19:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 02:28:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 02:28:22 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 23 Apr 2020 02:28:23 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 23 Apr 2020 02:28:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 02:28:36 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:91028a6d2ef79dd78d620852cfc6dcda63ffb7301b4a1e87108edd2e9e499625`  
		Last Modified: Thu, 23 Apr 2020 00:24:32 GMT  
		Size: 52.0 MB (51981200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ed4d3f137e711178f448cf040fd1089430356d44c56cc4850bdc605784ecb1`  
		Last Modified: Thu, 23 Apr 2020 02:30:21 GMT  
		Size: 10.8 MB (10803713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15132203cb696660534a47248d042d0e486196f12be13fbf155cf24daa544208`  
		Last Modified: Thu, 23 Apr 2020 02:30:18 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2356a37aecda13c9bd6535910a8adf19e151feae95732bf71b6bfe8b859b5392`  
		Last Modified: Thu, 23 Apr 2020 02:30:19 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38c8479ea96f2d3bdb7efc7b26a72fa7c899a76a2ba8becb1cf2129c3185d8`  
		Last Modified: Thu, 23 Apr 2020 02:30:18 GMT  
		Size: 299.5 KB (299487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ed738553a4bb4b45acce06b20e80dde97fe37c615f1d6e6648ed9af4fc5206`  
		Last Modified: Thu, 23 Apr 2020 02:30:25 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
