## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:c594db3c6d9203b58aafc0b9155bc177623ae994076e45db973b6e0d64d4e068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:6176d62a802336080532244b9b5aafea8a9a389e9fb27923a073b69b61b4aec9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65082178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5c3e1e77e83b1c86d5c01a5f62e43b54e93c71efca9c0bf2b67c2b870e36beb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:21:27 GMT
ADD file:365db4cb0be9894b5b688c566f8cb6ca848aa3777c680189478799ab75fb4be5 in / 
# Wed, 11 May 2022 01:21:27 GMT
CMD ["bash"]
# Wed, 11 May 2022 10:06:52 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:06:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 11 May 2022 10:06:54 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 11 May 2022 10:06:57 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf4cf577d743a8a18a793a3887db0f30d2d2093715da6cdfc0d68ee62f6b790a`  
		Last Modified: Wed, 11 May 2022 01:27:29 GMT  
		Size: 53.1 MB (53147126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9024db2d69feb65b3983dc13cf8b40ffdf0905395a1753e32df699ad36b7baed`  
		Last Modified: Wed, 11 May 2022 10:09:13 GMT  
		Size: 11.6 MB (11641475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58885687e1aef709d6f0b83b9ac6df104eccb5730034b725af1ac327be4854b6`  
		Last Modified: Wed, 11 May 2022 10:09:12 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7ad21c5554f666113a73b8ab7726d318371ba84ef1e4114005b104a3e7530c`  
		Last Modified: Wed, 11 May 2022 10:09:12 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f975b5879abdb6ce03e3134b525a7369bbe275ba06d567526c6863968d979384`  
		Last Modified: Wed, 11 May 2022 10:09:12 GMT  
		Size: 291.6 KB (291570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
