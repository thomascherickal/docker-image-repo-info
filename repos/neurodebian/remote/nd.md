## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:d2c65918ec2833688a37fe5a66aee4a458b46749b46c3a5a2011552b76da3fa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:80456a2b04d576a4e3ecbace9a3a9cfc3b9b136baf6387a956e4ba4a45e4becd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66532009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e283816aa9dd593d806b41c800af9a4d9918687447a327368e1e33301266a62`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:46:20 GMT
ADD file:cac9ad9d988141c80929e8c31f4cb388618dac0bbc048d4c5e3b8029c85c576d in / 
# Thu, 22 Jul 2021 00:46:21 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:52:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:52:20 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:52:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:52:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:531fc43e70accbfd0e52721b79cfd564769d6f1b7e64a98e9f670327d4c4820e`  
		Last Modified: Thu, 22 Jul 2021 00:51:36 GMT  
		Size: 54.9 MB (54909299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3b0521fb65a0934bb4a1d4f14fa47959490f1e770573ff0167b661ced0a18d`  
		Last Modified: Thu, 22 Jul 2021 09:55:04 GMT  
		Size: 11.3 MB (11309615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a23533ff64f2ceeecade8fa281752356d34c44af48ff4ec497d4331ba721ed`  
		Last Modified: Thu, 22 Jul 2021 09:55:02 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926769d84e8a93682f125f8a8be36b6a0e4921c21bab2e609c868e8af4f135cf`  
		Last Modified: Thu, 22 Jul 2021 09:55:02 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beffb2a406ba1b596ea59338e5cc2f7a5aab2de94afc6714a62a7d92e8fff8b9`  
		Last Modified: Thu, 22 Jul 2021 09:55:02 GMT  
		Size: 311.1 KB (311086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
