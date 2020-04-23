## `neurodebian:stretch`

```console
$ docker pull neurodebian@sha256:7d6f5d243302dd3dc83b0795d128d06ad4659a2b46547a40979833db76f7b9b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:stretch` - linux; amd64

```console
$ docker pull neurodebian@sha256:d16a2f24ada75b3e62779c7e00d2a71a86be47289ea1eb62ef34f48328ca1c76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52238018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4775b65eb43888686af5f027cec8f636d0ff99ae3569b59bcae0f1cc12d4f65a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 02:27:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 02:27:20 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 23 Apr 2020 02:27:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 23 Apr 2020 02:27:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cece94a11a6600cceafd6c2d97ce6d83731209693eec393859dd11830b119614`  
		Last Modified: Thu, 23 Apr 2020 02:29:57 GMT  
		Size: 6.6 MB (6566585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663ad87c6b6b1a31af198c1f64934e0734ddee59ff0bb525d868c9336ba6206c`  
		Last Modified: Thu, 23 Apr 2020 02:29:55 GMT  
		Size: 3.2 KB (3152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f631e6b5ca718f97825f945e5e795b8a5f720f653419f38c999336044b4c76`  
		Last Modified: Thu, 23 Apr 2020 02:29:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7ad0f4e501e413b13215b1bbe3988e648e5cc6302ce107a8f0f5b4098d32b`  
		Last Modified: Thu, 23 Apr 2020 02:29:56 GMT  
		Size: 292.1 KB (292086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
