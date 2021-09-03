## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:d2c370c2713abfe4cb58f3758d04b869ee60b39f1ce83f00d7d6d393d3dd2da9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:f709f5e4393d9956a076448ecda462059ff557a0b3076ec8a01561e8a344e8a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61240723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c05c55972abcfd0e29e69df6aa8297087434c8eb397946d2e5ef4b9738581a06`
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
