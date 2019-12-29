## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:68ed61f0db59676b5a9d5444d443e305c42903b40e07025475c826ddae51818c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:569a56f1c1b8db967ee3a5de59edc0b5c6e5c48505bee6a2f02ee5ae7b720dac
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.5 MB (62467659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fce54c1fa5f3139d8a0281b7da19972cde076e81842c54e9744a9b331a7a3240`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:22:47 GMT
ADD file:68b1541306250f957e5f1035d80f5683c1ed22e73cf2f2b563adc52424897a09 in / 
# Sat, 28 Dec 2019 04:22:47 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 23:28:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:28:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 Dec 2019 23:28:34 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 Dec 2019 23:28:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:28:43 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:d0b468739e287d7cd8fa8bcb34afb10216f12567d28caab345db8873c4246896`  
		Last Modified: Sat, 28 Dec 2019 04:27:19 GMT  
		Size: 51.5 MB (51479608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5404e4559f877062b5449d304c77ad9473966cbf395c6a8d3f8d63a3224b46a3`  
		Last Modified: Sat, 28 Dec 2019 23:29:33 GMT  
		Size: 10.7 MB (10687053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6569d0eb886537749cf92317631480e9837672e4c2d10b63550262fd8906cb`  
		Last Modified: Sat, 28 Dec 2019 23:29:32 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5e528767aac87ee94d23a3adaec175e5c826db90180e4225c937ee20416b4`  
		Last Modified: Sat, 28 Dec 2019 23:29:32 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e62500f70c81dac264123b016ff1cd2d4d6e56afb496a7bf39e4bd81a2dec2`  
		Last Modified: Sat, 28 Dec 2019 23:29:32 GMT  
		Size: 298.7 KB (298679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb24160f50bae6f737d03c0d65088d5bf217f4902f58e7cb5f7a7cf047a95a6`  
		Last Modified: Sat, 28 Dec 2019 23:29:36 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
