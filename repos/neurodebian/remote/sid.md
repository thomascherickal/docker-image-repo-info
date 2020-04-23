## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:fd79013d3164724c4c5dc08748804d4ff62f90fc67ce21a70f700fa7b22eb8dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:266e606242e2cd640420ebe56e857b573ffb3872c1dc400bd256fe24d5dc6062
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63085048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e214f3c8f8e6de3be29c770d06036ec0a894b27afa698cf5a24a08983f98aa5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:21:58 GMT
ADD file:5d2d72d29ae1c01dc7f5bf337c78d40925a9843052910f79f066f681a2ec43e6 in / 
# Thu, 23 Apr 2020 00:21:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 02:28:52 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 02:28:54 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 23 Apr 2020 02:28:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 23 Apr 2020 02:29:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bbc6b8c460d7ed40af9e8f69693608780022541107dbb47c4a717e0a15e84f4`  
		Last Modified: Thu, 23 Apr 2020 00:26:48 GMT  
		Size: 52.0 MB (51979787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2086fb3017ac7dd6883ae68578f985009c64d8d15ddd5625f8b16fb4f3adea12`  
		Last Modified: Thu, 23 Apr 2020 02:30:31 GMT  
		Size: 10.8 MB (10803807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64fac0514f6232d52f7b930f831549f765d94d600a1fbececfe621832f11311`  
		Last Modified: Thu, 23 Apr 2020 02:30:30 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2e148f749066d7095c52dc71ad553f8231a14ff8b408d8e02c3b0f6bc69246`  
		Last Modified: Thu, 23 Apr 2020 02:30:30 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1763588ac2d148527e1d88e2ca14f740e7dcc9e8b54eec7aaa15eb486bfce5`  
		Last Modified: Thu, 23 Apr 2020 02:30:30 GMT  
		Size: 299.4 KB (299448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
