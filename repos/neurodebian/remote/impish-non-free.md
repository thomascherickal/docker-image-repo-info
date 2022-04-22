## `neurodebian:impish-non-free`

```console
$ docker pull neurodebian@sha256:3dc5a444e8a4eab525db8216d070f3e4d819457031eb4e8fbd342d9b1402b82c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:impish-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:a2894b29edc077089e14fce7de29e3cba0f7a8d0d0b751daafe9816d6696b4b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34386821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38dd596c7a41ca7fa5bf263b8cf4c293b659dfaed05a0e78e9e5d3f7962f14da`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:16 GMT
ADD file:9b7b0966dfc440424d605ce69eca7c183576d2d20f1534bab2c169b0550c40f0 in / 
# Thu, 21 Apr 2022 23:00:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:00:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:00:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 22 Apr 2022 03:00:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 22 Apr 2022 03:00:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:00:24 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:6eb9a17f92a2d3c01d47408a9505c2dabf5eb36c13a06aa25adb53b1ee5ab488`  
		Last Modified: Tue, 19 Apr 2022 13:18:15 GMT  
		Size: 30.4 MB (30382790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200d665c3996926ebb81d48c31a70a2c36fdc7288582849108c39e97bccda1a2`  
		Last Modified: Fri, 22 Apr 2022 03:02:02 GMT  
		Size: 3.8 MB (3752071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6df395cf0660542ad1548610f055a0f059ab0c13e0efcb4846aed58b2d97f1`  
		Last Modified: Fri, 22 Apr 2022 03:02:02 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d65fb0dbf939446ba47d47e3d405b2de02888507c6318603da8d8e8af1727cf`  
		Last Modified: Fri, 22 Apr 2022 03:02:02 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3e62e0886897c3f75882d8b80f825f5b58cab6da492c4181d2f548cd06cc19`  
		Last Modified: Fri, 22 Apr 2022 03:02:02 GMT  
		Size: 249.7 KB (249687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324109be964c8011b00ac109ebbb299e5d1ea71c151e1dd890be4747cdcfe356`  
		Last Modified: Fri, 22 Apr 2022 03:02:11 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
