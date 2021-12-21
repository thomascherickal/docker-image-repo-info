## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:c564b735768fa670be885043bba616b189445c3b20abf08e9581319892dc5a45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:5db501f889518c90862643e6008cc557729c1c27ec154b9f5c0b2cdcb2223806
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67469134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2995000bd6b81d79255ed7075c4a07ca3e9c6e64b439d7489b7ca39479cda994`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:53 GMT
ADD file:ce4b0836a3fcb4df3c14bacf996ad27dde10d17f63fbf745c09d6ae62c3e2cc8 in / 
# Tue, 21 Dec 2021 01:23:54 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:41:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 18:41:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 21 Dec 2021 18:41:44 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 21 Dec 2021 18:41:48 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c476fbbe1d7eecc32473e300b1659f1eaf7c11eff20d52cd6f7471c94062564`  
		Last Modified: Tue, 21 Dec 2021 01:30:07 GMT  
		Size: 55.8 MB (55798023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee226796e9d2864a9c10e7047bcb9f22da74a77f1f5f0f27c045967f09610df2`  
		Last Modified: Tue, 21 Dec 2021 18:44:00 GMT  
		Size: 11.4 MB (11358141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808d5780b4777a498043cde7694afab5156039933094167a24aa2333aaaaf98b`  
		Last Modified: Tue, 21 Dec 2021 18:43:58 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97fda43a60634d37298b204667ee93ac310b9142296dc483de5419e0c270996`  
		Last Modified: Tue, 21 Dec 2021 18:43:58 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2dfc082fbf4f59ed25c3e95b72d993d5b43b8d3a7fce1a6a4bc342296266e6`  
		Last Modified: Tue, 21 Dec 2021 18:43:59 GMT  
		Size: 311.0 KB (310960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
