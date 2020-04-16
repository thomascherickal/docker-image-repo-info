## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:3e7ab16c2dc169c5e9266c8a1c783ae9abd89a82d4ca5aba7ecf0865e6de4639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:ad3842b6f5b1e8d93718ccc7931b0636ed6225a113e16aa4ab0345db31f8d958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63081563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b1d8f4b98f863642b1d9e0f137e022cec341d06e6063e0d9d5f96b666c4f13e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:25:32 GMT
ADD file:2496494632885054452c6f15317aaeace67145465fe0f719da9d3b5c95e6c8ed in / 
# Thu, 16 Apr 2020 03:25:32 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:02:07 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:02:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 16 Apr 2020 10:02:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 16 Apr 2020 10:02:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4396830990ba6684412015e660aecabd027170dd4336124dd128865a6a81898`  
		Last Modified: Thu, 16 Apr 2020 03:33:46 GMT  
		Size: 52.0 MB (51976212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0476f218e21db586c00c4fe1d49d89b6066568f2968d12e1703d518120031833`  
		Last Modified: Thu, 16 Apr 2020 10:03:49 GMT  
		Size: 10.8 MB (10803879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b02e327258d5b668d9dc51c0cae431bc97c7807a4d1d7cace91bf649ffcd4dc`  
		Last Modified: Thu, 16 Apr 2020 10:03:47 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222682a0c0edd66c0ba6405a7b14c9d53ea61465b0aefa189aa01e793252c69d`  
		Last Modified: Thu, 16 Apr 2020 10:03:47 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a27ad0492fb0c4122f67e4867539137fd28d60caedcb778c41e8213ecdad1e`  
		Last Modified: Thu, 16 Apr 2020 10:03:47 GMT  
		Size: 299.5 KB (299466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
