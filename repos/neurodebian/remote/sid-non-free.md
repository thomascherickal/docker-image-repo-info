## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:db190ee7530c06a3b7ec273af342be45667491aae52ce63e4460668a7db9c8ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:23f729750988d2f5d1b71c00d86778c8806084f5cb43a0079592aec5461b98c4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67131923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37593f1427bb1b796a8c9656ad947cfaa60b6051382cea72dab4217fd884ce7f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:48 GMT
ADD file:7ab12da96bcf5f352bcecb8ee3269debf1ca1bd2d25aa9a7b66b1e4f84e07c3a in / 
# Fri, 03 Sep 2021 01:22:49 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:31:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:31:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 03 Sep 2021 07:31:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 03 Sep 2021 07:31:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:31:24 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:f9ad9a9c210fa67e2eb0faace583b349a4623b682daec47e2b4c65c33ac9a92f`  
		Last Modified: Fri, 03 Sep 2021 01:30:17 GMT  
		Size: 55.5 MB (55493249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c39cf9af1d9f21f44a5049049a2f43aa27ec81e666382dfabfa3b0e758f3b`  
		Last Modified: Fri, 03 Sep 2021 07:33:22 GMT  
		Size: 11.3 MB (11330267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12ac919adbbf81bbd1bc18e1ac8ac8092564913d50c67622b597583d67aa33b`  
		Last Modified: Fri, 03 Sep 2021 07:33:20 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268681e4e5e85bf88992cda94cd942d673ea27aa7c32d24f366478647b769607`  
		Last Modified: Fri, 03 Sep 2021 07:33:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaf89740502350ce94057898591d5cd5043f0cbeba2826631635210c63b6765`  
		Last Modified: Fri, 03 Sep 2021 07:33:21 GMT  
		Size: 306.1 KB (306087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b939c3e8c3f996fc8a610bc9aa85ef643d01f683c993736dff2af117a0a064b`  
		Last Modified: Fri, 03 Sep 2021 07:33:33 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
