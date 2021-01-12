## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:81c306659a95e5dd5adf8c07076887bb153c0868aae1ca86bd7bee12e62c787d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:8603aa792176ff3b5a1c40264dbb78faba13ba8b6ee063c7d2c9bd03b4d001c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68204752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fcbe5a1058f7c46f5f7092a4c8c7d9ea95314bb0a65e02f102ba936df8dda29`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:34:16 GMT
ADD file:f1c9279b9eb3b88b40c4958324519afa81185c0383ed51d5138ebf2a0eff6d7e in / 
# Tue, 12 Jan 2021 00:34:17 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:25:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:25:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 12 Jan 2021 10:25:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 12 Jan 2021 10:26:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:26:08 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:abc50f4e181143f18afce1a5282914e00abd896a798d96f7514e728b30f0988d`  
		Last Modified: Tue, 12 Jan 2021 00:41:42 GMT  
		Size: 56.8 MB (56800959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7621a27e88061ca5b2ebc50c64d58af2b9f03d50adc526e2d02e478aba0481`  
		Last Modified: Tue, 12 Jan 2021 10:28:34 GMT  
		Size: 11.1 MB (11086106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b650d6612d676c1878a192328fc69763ddcd556d8b907931f0d79bf7e4181c0`  
		Last Modified: Tue, 12 Jan 2021 10:28:33 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e191fef92eb9ed8df56ec7f4cb70e902f0be1a0a9ed4cb93537a5500a56d`  
		Last Modified: Tue, 12 Jan 2021 10:28:26 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1988ce62a69fdce1cf2ba96d62ab3985d1591a8fda08e8541229e6e99721bbe8`  
		Last Modified: Tue, 12 Jan 2021 10:28:26 GMT  
		Size: 315.4 KB (315362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ab1187e80fec9396f9b0b60bca66f55436acf74444b05769a76205d36d7e66`  
		Last Modified: Tue, 12 Jan 2021 10:28:43 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
