## `neurodebian:jessie`

```console
$ docker pull neurodebian@sha256:5128613e886c974f7458f5a46c6e0698f7a10a74699bfd9da354a324b4715947
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:jessie` - linux; amd64

```console
$ docker pull neurodebian@sha256:5d3edb8b4845310ae57618d279269d22eb91764aaa01027554ad8071797605b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54694595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580df985c7fd689e629d6a842a88b816af9bc715d51829580699998889085ed7`
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
