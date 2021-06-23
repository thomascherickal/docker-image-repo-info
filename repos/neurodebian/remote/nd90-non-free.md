## `neurodebian:nd90-non-free`

```console
$ docker pull neurodebian@sha256:d6acc3803cfd1ed66c5db56da11f7d2fe491eca8dba4d2a619f73b8acd11a58a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd90-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:ca3710248ea20749352d3741e0aff684937e76154cca5aad92e19338ece59603
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52247656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c46b66e68a31ca90db7dc72a00a13747de5ef70081d275e34d12f0eacc4b672`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:21:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:21:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 23 Jun 2021 07:21:51 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 23 Jun 2021 07:21:55 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:22:02 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857559593f8dda1e410719be8972b785cfbae930aad7ae9cf766507c70a4ac89`  
		Last Modified: Wed, 23 Jun 2021 07:24:36 GMT  
		Size: 6.6 MB (6571635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0736faef4fb0d48e084bad3380a3836d5d1b6e1b5c8f205918bd0b66861948`  
		Last Modified: Wed, 23 Jun 2021 07:24:34 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f33265cce1268b74c0c2c135c3209c135b70f98374def5bdd1c50531f83c96`  
		Last Modified: Wed, 23 Jun 2021 07:24:35 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc75833b2d5af44e32b488c15289ce7334fe9f722fd710d523574d93ff5e0c0`  
		Last Modified: Wed, 23 Jun 2021 07:24:35 GMT  
		Size: 292.3 KB (292263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65739ba9e8fa13d631c52a56ff52abbd022cb7d807b721525edf1e79065371b4`  
		Last Modified: Wed, 23 Jun 2021 07:24:46 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
