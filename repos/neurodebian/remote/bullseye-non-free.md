## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:808c6e2e00b1e33f2937bae109801351c6a6a07c7fb620276b381bdeb1e21da4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:e5db591faebb451c8f4f62fef27775eaece83653ac128184b45d6f19bd04c1f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66520159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2ba03fe2527e296b0155f333dee4ebeef356428d3edaa8b19cc5e25c48ecea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:19:59 GMT
ADD file:eebf6f761892ad2407885aa93a2abf7647cf0367e3590f3cc7971594ff47193c in / 
# Wed, 23 Jun 2021 00:19:59 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:22:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:22:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 23 Jun 2021 07:22:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 23 Jun 2021 07:22:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:23:05 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:d28ba3bddf26336a2dff9ce3319ecd166971168469860f171fa659f62cb3ff6d`  
		Last Modified: Wed, 23 Jun 2021 00:24:24 GMT  
		Size: 54.9 MB (54898218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f4fca9472bd77559a0b979cadb904cab6c586d4758d216cc9164240c46b154`  
		Last Modified: Wed, 23 Jun 2021 07:25:27 GMT  
		Size: 11.3 MB (11308984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f246cf55d9b2cf172a8093664180df1fc49e03c400da38d2139b483dfe68e2e`  
		Last Modified: Wed, 23 Jun 2021 07:25:25 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df88bd28651be3ec0af911a7f5bb5c34afba4e9033ab306b39e9f2091af29e7`  
		Last Modified: Wed, 23 Jun 2021 07:25:25 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b71de42abc6a1c4e365cdeacc07172d31d5c328c749aff1e83045d3030d3fc3`  
		Last Modified: Wed, 23 Jun 2021 07:25:25 GMT  
		Size: 310.6 KB (310576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e1d8c6420c23e01880846ac0e4a18503e06dc0d2d4ca46a2b0dca9bf5eda0`  
		Last Modified: Wed, 23 Jun 2021 07:25:38 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
