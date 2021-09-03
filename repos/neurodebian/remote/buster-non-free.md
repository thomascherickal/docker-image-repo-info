## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:06467b6306536960bf390d9c36c82dbe5be8a44378db96c3118460c2c5485f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:01f85cdc92592fddb8e6e898a17a4c8ce22f10bcc7e470afa975ca7de1f0bbc0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61241089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd2f9338e6a0a01d188e8fb049804487a9a9e58621cc2206988ce4ff825f1325`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:30:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:30:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 03 Sep 2021 07:30:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 03 Sep 2021 07:30:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:30:27 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea535d1272aa8e5a32839c9e19affdf9f921d97026e9114e876f43c8942e1df6`  
		Last Modified: Fri, 03 Sep 2021 07:32:35 GMT  
		Size: 10.5 MB (10500033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc99eb20e5547a686fbf9a226999bb64d0c12eab62bdbeca69ce97a5365e05e`  
		Last Modified: Fri, 03 Sep 2021 07:32:33 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1201e23693ddafc23a4ef1584f2730a5ef3c2f13dac6ff08562deac09ba94e8f`  
		Last Modified: Fri, 03 Sep 2021 07:32:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8914372c601dcbfd4a7ce6ed003526716b832c55c1ac8358518699463c283531`  
		Last Modified: Fri, 03 Sep 2021 07:32:34 GMT  
		Size: 302.8 KB (302783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e310a26d6c423307259b327d87b6003c1b725fc94cad8b93d86d0e7ed643cc`  
		Last Modified: Fri, 03 Sep 2021 07:32:47 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
