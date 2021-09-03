## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:53556fcb2299d929a10eeeacbb38e3c1fb18321477ee63a73c62823d938a89d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:4805e0dedd85e78aa176a509e183a510bc6b705e62b21cf2750c12b767e2c4d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67131607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1637aedc5eb635928dcb1990fc63c575f68b387489e99c5fea4d261688794597`
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
