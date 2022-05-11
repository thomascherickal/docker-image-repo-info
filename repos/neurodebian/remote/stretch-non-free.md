## `neurodebian:stretch-non-free`

```console
$ docker pull neurodebian@sha256:2d0da3d98be0048a2d00b682ba16760d3dc29a56bdc379b1478aa8418d41cda7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:stretch-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:75239f666e9143dd9a1a90880cca3e1bc40d5a84c5c5c5e65e1cdde41c7d0b98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52296804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9985e2c91371d4035a90bc57c330ab7eefcf13051948445743dbc17fb509a0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 10:05:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:05:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 11 May 2022 10:05:42 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 11 May 2022 10:05:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:05:48 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bde9b14b349a09e02be38b65d889b9fc5e8d67270d490da9e7ad63eb4a95d1`  
		Last Modified: Wed, 11 May 2022 10:07:47 GMT  
		Size: 6.6 MB (6572743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2058dbf431fd9297cc81f8eb2072c2012b58c505c0363cf3a1a403091e1dcc56`  
		Last Modified: Wed, 11 May 2022 10:07:46 GMT  
		Size: 3.2 KB (3156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ac9348c3703d5e3dec451e2fbbd6f6418cf122cf24205208213037036a2a4c`  
		Last Modified: Wed, 11 May 2022 10:07:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cecd15d6f063561e22caf077f6635f2162a57ef48894e6114c4ffd9a4e03d3`  
		Last Modified: Wed, 11 May 2022 10:07:47 GMT  
		Size: 292.3 KB (292291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd64132722a4d71c7e5fcb10a3f1ef8405c9d89064497701e94021ff62607244`  
		Last Modified: Wed, 11 May 2022 10:07:57 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
