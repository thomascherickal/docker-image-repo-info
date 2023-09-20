## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:7b68448888fe4d9a1604a6f1b59a0e9fd4e4ffe9e3f2ac4e9d2915d0f6772e9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:1fcb3454549760d53b3c7ce3d16c5fbc63368b5b3e7a55e900fafb243eac40fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64056419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8595c9e3f9168c206bb7990dd891f2b82fe6d38adc1b1087db6cf55e24dbfb4d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:17 GMT
ADD file:bc0b5b71ee53adf6297821668404ace4f79c4256461b99497849721dbd8e86ae in / 
# Wed, 20 Sep 2023 04:57:18 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 05:57:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 05:57:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Sep 2023 05:57:51 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Sep 2023 05:57:55 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d036181e87bed9eb2432498f0ccbf7baa06719a2d8360c3bc9c496bd9f853a7c`  
		Last Modified: Wed, 20 Sep 2023 05:03:10 GMT  
		Size: 49.5 MB (49482728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5f448790412f2b4749596c323f460fd626e02a0a2cc2c5807fd227c9b2393f`  
		Last Modified: Wed, 20 Sep 2023 05:59:22 GMT  
		Size: 14.3 MB (14287421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46be4fb4c974cf5509873e1242391934cba1868808854057528ee20b65b371f0`  
		Last Modified: Wed, 20 Sep 2023 05:59:20 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec9aa8565bd54eb58d36ced36fad6281081fa1d832dd2c7555d1f17105b5376`  
		Last Modified: Wed, 20 Sep 2023 05:59:20 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3adfb7e9d68ffa3f542118503072e5f615786d815ea40213a0c0d7291714ad`  
		Last Modified: Wed, 20 Sep 2023 05:59:20 GMT  
		Size: 284.3 KB (284265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:6f0abafd11f5551f9838e72ee036e21ea6b63f326a8e28e201e8bd8af63ff514
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63837709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:428cf64c62402538ba3f3865b036212d6356e7b07fc5dfede2880d388667be1f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:16 GMT
ADD file:3493f4ad2710629ee9ad4c981682b2afcc1d9964cb5034de77189556f0c0e810 in / 
# Wed, 20 Sep 2023 02:45:17 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 16:39:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 16:39:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Sep 2023 16:39:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Sep 2023 16:39:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d83e3b52cf7f7a250777a05d8d2d7960fd6dba8a6438beed3879ff3c389bb01b`  
		Last Modified: Wed, 20 Sep 2023 02:50:04 GMT  
		Size: 49.5 MB (49450488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8965664119e10fdd3649f860a7bbdcd06938c9a55ed3a8f81b2baea9624c75b`  
		Last Modified: Wed, 20 Sep 2023 16:41:22 GMT  
		Size: 14.1 MB (14100489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06c78d6d0207362d99bd6c425fd11e74d75e6b59324f33e115ac94ef0fd9ff4`  
		Last Modified: Wed, 20 Sep 2023 16:41:20 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57993ec3035f119b23152e6f75a89529851fea63b51ebf0da5047a16cf6bff4c`  
		Last Modified: Wed, 20 Sep 2023 16:41:20 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfad4d7286ef19d36be182694dfd20f031ea83aeaf83172f1efe10b2c84f4a2`  
		Last Modified: Wed, 20 Sep 2023 16:41:21 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; 386

```console
$ docker pull neurodebian@sha256:491b9c8b3d7cd2efa9f041674dd484f6be2f69df48e454947df8afab99b97a4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65459826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22815772247b79196b081fdc3b1ea9f78efae6682beaaa918fc8ebd86ba4fea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:43:36 GMT
ADD file:89a1cfdf26e23095cc168a8c054aaa8afe0cb7f1b748f0dbca755e9aad935ce8 in / 
# Wed, 20 Sep 2023 00:43:37 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:51:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:51:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Sep 2023 15:51:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Sep 2023 15:51:28 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a77a25e288eca9c35f0aeada81ba65e2f4beb3d0b739a139eb41bdd87309a97b`  
		Last Modified: Wed, 20 Sep 2023 00:50:06 GMT  
		Size: 50.5 MB (50483129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00716f16669fbde1a6927877c8b01a86fadde4dba1fa729c70c2201e14dead39`  
		Last Modified: Wed, 20 Sep 2023 15:52:53 GMT  
		Size: 14.7 MB (14690576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142260c4269f1833147ea7d89316ff0d7fe446bca322be1c938c8f427b7ecc74`  
		Last Modified: Wed, 20 Sep 2023 15:52:51 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53f904f97cb7220a02a08fa85614a17ea76ee3034d7d80d3128bb31e257435d`  
		Last Modified: Wed, 20 Sep 2023 15:52:51 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba20fbcbd3f269dc55fa471a0d8557fe1660422530efd90bac3726276d870505`  
		Last Modified: Wed, 20 Sep 2023 15:52:51 GMT  
		Size: 284.1 KB (284112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
