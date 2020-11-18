## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:5f77ac646fba6920973f0dd961c7821a8b1786fc8e3213da3bd19a576a5e7dd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:c69dd0e7418a6e3a68d17c004610ac8e2666f0158fddbbec386ce3f4aafd362a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61199898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800f4718de059d84f113194fedd6191f3f6904af9a8daee6834c9db58ff980d3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:58 GMT
ADD file:9a4fd72d749f4a791e75e0f6fc6028d0771e3381b6d84a8d0b07a4887bc7c641 in / 
# Tue, 17 Nov 2020 20:20:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:10:23 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:10:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 18 Nov 2020 00:10:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 18 Nov 2020 00:10:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:756975cb9c7e7933d824af9319b512dd72a50894232761d06ef3be59981df838`  
		Last Modified: Tue, 17 Nov 2020 20:27:06 GMT  
		Size: 50.4 MB (50397725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ceffd8c52a28c8873d96d4f2b3adbf04ca204e450b915882314c9a326864e4`  
		Last Modified: Wed, 18 Nov 2020 00:13:14 GMT  
		Size: 10.5 MB (10497692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357bf48515907d129f764599c9fe192123a6a5705144928b35b8f7127bd0e1fc`  
		Last Modified: Wed, 18 Nov 2020 00:13:12 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcf29cb467a2c808ae6ab4ae9a66382b886d0ac30340dff38375fbe481b1887`  
		Last Modified: Wed, 18 Nov 2020 00:13:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2395d0fd8779a30737ae80202b6aad3f341e16cd04a18e249c841bbebfa0c`  
		Last Modified: Wed, 18 Nov 2020 00:13:12 GMT  
		Size: 302.5 KB (302472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
