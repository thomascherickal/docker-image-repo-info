## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:8e86139340156ad6e98c9af819ec1db0e36fb3daef1ab1a34d6d9fd1d3b03aec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:28318431ae819653428a5b70d234c9ff8a037001aeed9adceb90fff7466dc3c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64936724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:734847727feb8e61c9dca141f01bb271b08de8aa67ee498026d1e1f0ca672b77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:09 GMT
ADD file:730ef8e3327df644cd47994a561a489bfcce5da8103cc8eb34e67321a36df2ba in / 
# Tue, 12 Jan 2021 00:32:09 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:25:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:25:12 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 12 Jan 2021 10:25:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 12 Jan 2021 10:25:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:25:30 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:b802c2c29a7757c7475a0b343a18a46b6b27dde9e3fb6b4db61c68ea197b51d2`  
		Last Modified: Tue, 12 Jan 2021 00:38:04 GMT  
		Size: 53.6 MB (53566443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01c3d8ccd25913989c2dd4149c8d52bd60b5c5a9d4cbfa2ae118b46dddf11a9`  
		Last Modified: Tue, 12 Jan 2021 10:28:09 GMT  
		Size: 11.1 MB (11068165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f191dc33357288191e12d23395b749a493fd055bcd9ef4b4426466d7507c6`  
		Last Modified: Tue, 12 Jan 2021 10:28:07 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0947614c31027c0e46a506acce1ae2b2f909b9e999cb2efa282829dd4d470b25`  
		Last Modified: Tue, 12 Jan 2021 10:28:08 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d13d5e1191407c05105818f76dcaefb8934e4e532e1c0670dc7640679a910b`  
		Last Modified: Tue, 12 Jan 2021 10:28:07 GMT  
		Size: 299.7 KB (299737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0741446f8ed09bc8d1b9cab998a1464c09c33bbd0fb829d32c8657ad4d2dd5`  
		Last Modified: Tue, 12 Jan 2021 10:28:18 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
