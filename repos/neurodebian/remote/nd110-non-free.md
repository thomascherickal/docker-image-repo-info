## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:eec076bba76a4a06b5cc303e126aa3819951342ec2c9f6fcddaba3de0e2ab940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:0b8bddc6f51a47633082635d9ad68b74cef195e54b7fa1d1fdd2d2f1498c0670
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66542162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83e989b5a73ef06056ea9b2e5a7a7b71422022e081bad485b67e3482b420fafb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:41:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 18:41:19 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 21 Dec 2021 18:41:20 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 21 Dec 2021 18:41:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 18:41:27 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f80dc452cc935161761dfaf49aa5057016c59731becfa6be48b522efd5d5846`  
		Last Modified: Tue, 21 Dec 2021 18:43:29 GMT  
		Size: 11.3 MB (11309501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae05a95b32c0be46ad219a06765bd8dcf1542fca4bec2d1823a0bf35494331f`  
		Last Modified: Tue, 21 Dec 2021 18:43:28 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d007db81074cee5ffd9b1b23cceb22da63f94db378440fcd16903be7778fc9`  
		Last Modified: Tue, 21 Dec 2021 18:43:28 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0d1d4d049e1f0547c596f2e0a7b1edaeb9c5d69f54784a5becbd0eb8c137db`  
		Last Modified: Tue, 21 Dec 2021 18:43:28 GMT  
		Size: 311.2 KB (311243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3e03657e3279c9ff8830c38f923084e355b25b00a8a4aeebaa9f5afab5877d`  
		Last Modified: Tue, 21 Dec 2021 18:43:48 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
