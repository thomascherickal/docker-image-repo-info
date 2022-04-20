## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:a10f940caffddb3b8667045062ee0aec2d7b77d18099685148a54879a3e028fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:d31bd892c0d5dd55591793990a58e85a26146f4ffbc6e74e737b6fbfe3c59501
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61242238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f826ef234dd3e97db83bc1b054288a8a4238589450cd34b2fa2e774f6aaead2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:37 GMT
ADD file:7c5789fb822bda2652d7addee832c5a3d71733f0f94f97d89b0c5570c0840829 in / 
# Wed, 20 Apr 2022 04:43:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:08:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:08:36 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Apr 2022 10:08:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Apr 2022 10:08:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:08:45 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:85bed84afb9a834cf090b55d2e584abd55b4792d93b750db896f486680638344`  
		Last Modified: Wed, 20 Apr 2022 04:48:49 GMT  
		Size: 50.4 MB (50436985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f5041b1b1d700117a8831742b268df036f0f7803d7401e9068218df9a8036b`  
		Last Modified: Wed, 20 Apr 2022 10:10:50 GMT  
		Size: 10.5 MB (10500109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5182139b25431391d19580e5d88a1f1d3a5b428ed7f9cab1f2a87b2ac5e4acba`  
		Last Modified: Wed, 20 Apr 2022 10:10:49 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6a3ce489317635f650e6d5f975fca5bc1bb15aef51a929828b69e5460ff1cc`  
		Last Modified: Wed, 20 Apr 2022 10:10:49 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7746a8c162798ad15695cc789376669a5cdfef219d02a00245bedf00e8ba85`  
		Last Modified: Wed, 20 Apr 2022 10:10:50 GMT  
		Size: 302.8 KB (302773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d81245b598c1b1829bc090f605d255eb9c5bbe21719dce7c451596f8939760`  
		Last Modified: Wed, 20 Apr 2022 10:11:01 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
