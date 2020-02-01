## `neurodebian:nd80-non-free`

```console
$ docker pull neurodebian@sha256:ea23707ff1653e9aa97c2be199a01109425d9ae75eadbdf5fb02297130670032
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd80-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:77dd2fca17a76a9d804a96f2900d2dd4f95a3986f080d1ea9b424751da278701
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54694961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0010d0a1868290f990a823ba3261c37aded843397786b65acac2b8ed0fe71524`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:21:06 GMT
ADD file:2ff99c4b1a4acaafb9f4705b01b8d997c1af388f3732ed81d317a1c52f4ec30e in / 
# Sat, 01 Feb 2020 17:21:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:08:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:08:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 01 Feb 2020 22:08:49 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jessie main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jessie main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 01 Feb 2020 22:10:34 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:10:44 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:be2ea31e65ce4ed34b999c4be891da1ed0e4c259d9ccdebc7e0ac094771f30af`  
		Last Modified: Sat, 01 Feb 2020 17:26:36 GMT  
		Size: 54.4 MB (54389437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c911be648906b2964ebd4396a9e0af3dca6e7d4476a6383f20c619458832cb`  
		Last Modified: Sat, 01 Feb 2020 22:13:07 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e621326e763977841b7d409f4f6e7084b8e51db668e9d8299c9ce687f19939`  
		Last Modified: Sat, 01 Feb 2020 22:13:07 GMT  
		Size: 3.2 KB (3154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf14d5ea04955bde7027dae52e9589bab522753dc223700527cb47027959d3b`  
		Last Modified: Sat, 01 Feb 2020 22:13:07 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f0b91bd4d9c2ff7b1deea29720373132b735d22d60652a01a08bff5cd8b383`  
		Last Modified: Sat, 01 Feb 2020 22:13:07 GMT  
		Size: 301.5 KB (301467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5931f7ad5a8d93c1b3b501242aa141258bf049ac2b8b215f45d490909339304`  
		Last Modified: Sat, 01 Feb 2020 22:13:10 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
