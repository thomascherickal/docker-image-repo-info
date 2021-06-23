## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:8e08d076837a26067c28fe149f0e5b9c3601cc99f1b40b85d11d96237d0cd68a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:34d15f906d162b3e482e558c73dbd8f330d443dafacb250630d32568d96553ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66519793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b61f08d9a32a72f0a424de283fd3ec7b78c19600b1655c06c029c0f6d354cc1`
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
