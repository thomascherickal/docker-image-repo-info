## `neurodebian:stretch-non-free`

```console
$ docker pull neurodebian@sha256:0427c0b2c1c96eab6f4dac204a5cac90882dc9c31a43dd948b1fca4696c8f84f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:stretch-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:fe740e83c05cdb2e59d41691420443e5fc39be63637b5572e087a78bf04cb774
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52247488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0de1e83652d0a43f0f05482f00dcbb0e6ffbdc7275c427ec70094baf6befc938`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:05 GMT
ADD file:fc9409352ad67880b83ccf1ccd1587eb2666715eae04e4dd98fca919f1bb98d7 in / 
# Thu, 22 Jul 2021 00:47:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:23 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:26 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:08224db8ce18b31a78a0a26d1b344d173528e50a7067797c9df4de5d8df353e2`  
		Last Modified: Thu, 22 Jul 2021 00:52:52 GMT  
		Size: 45.4 MB (45379781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289adce44c74cd3a9501987ddec1de9c56dbb545616cbfea0b4b2a956ae56e72`  
		Last Modified: Thu, 22 Jul 2021 09:53:47 GMT  
		Size: 6.6 MB (6571690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fde85f89658efa8b979f1de6a0663239b9f4c362692e305ee64910699d9cd8`  
		Last Modified: Thu, 22 Jul 2021 09:53:46 GMT  
		Size: 3.2 KB (3156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4e487d6d5d279e94dd8d7a0f1e4ce1b64782718dfce3b1097823b14cc0938`  
		Last Modified: Thu, 22 Jul 2021 09:53:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9fd062465c63ea7dd9b47b082b1aae8acf40f8986201be095fe539191b7ae5`  
		Last Modified: Thu, 22 Jul 2021 09:53:46 GMT  
		Size: 292.3 KB (292252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9fb36130a8fab9876e15dea4761044754c3ba091cb0685efed82f701c01bad`  
		Last Modified: Thu, 22 Jul 2021 09:53:58 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
