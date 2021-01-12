## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:71c08c4be38d873e2488a23f4c762f6026669bea6ecb9a397f4fc7ff4d997bf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:b70d62e632ee692d593930d2bd74719b26dc90aaf1ae17190dd4c14e710681a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61201974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:534a791ddb75f546e89d412eb98f7cbbee654c51effcde7e67e03482ba9eeb9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:24:36 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:24:38 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 12 Jan 2021 10:24:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 12 Jan 2021 10:24:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:24:52 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8697dd90e9187aee9b6fc99ac097091b2034feb04a3ec43a5b90ff1fcbbe28e4`  
		Last Modified: Tue, 12 Jan 2021 10:27:44 GMT  
		Size: 10.5 MB (10497954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f66763f38b2ede7a133b78edc92c6c9edb138b1c8337b1ae029efeb6f6c0505`  
		Last Modified: Tue, 12 Jan 2021 10:27:42 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e25b9e0e7a5ee63b20971878f742f5576cdcfa2122b8f4a8b561b5d5b7a1da8`  
		Last Modified: Tue, 12 Jan 2021 10:27:43 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3626b358cb25db730b2c9befb2675744353e52cd2f20f555e14f1e9184a8a64`  
		Last Modified: Tue, 12 Jan 2021 10:27:43 GMT  
		Size: 302.5 KB (302474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c737d7eb2c36a5b80856fb4ec72bb341c6b2f57bc47bd3f07c98b98fa8f3083`  
		Last Modified: Tue, 12 Jan 2021 10:27:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
