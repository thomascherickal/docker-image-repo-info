## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:4b9dcf7ba02b189fded79ced04b93eccabea9381e6ad1b5ed526e6ca34a5c3a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:da62d250fd4bdf2f3c34cecc214e8f50772f12149c9e64cc20a940062067f165
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61305745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857a80b9dbcdc7ea48e99524ee929708c0367b66db19f7f708bbc81c49d79300`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:22:08 GMT
ADD file:4f8b7a35280160ec5a55323fa07ac91e294c86e2ea647ba212053983ef380bcf in / 
# Tue, 21 Nov 2023 05:22:08 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:01:59 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:02:01 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 21 Nov 2023 09:02:01 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 21 Nov 2023 09:02:05 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b32028968d56a86ac35eac062e7abba276c547ab175fb057973c469eb41db55b`  
		Last Modified: Tue, 21 Nov 2023 05:26:57 GMT  
		Size: 50.5 MB (50499471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f451a3934dd4e405d1dde860ba51678368513b19573aff4a31e37ec0366b9d`  
		Last Modified: Tue, 21 Nov 2023 09:03:41 GMT  
		Size: 10.5 MB (10504804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4affb99dfb075e560f9c1cb0540086f42280fcb523cb1ad9b1e4dacdc7a6370a`  
		Last Modified: Tue, 21 Nov 2023 09:03:40 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075cc32496ec9687c5bb5438c0ff3f5d35a14bae9d664a4632b8701809cb9c6e`  
		Last Modified: Tue, 21 Nov 2023 09:03:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e46c61d3ea200904ddfcadddf54a73182bcd89e26c3f9857dd1d7de8d66f8df`  
		Last Modified: Tue, 21 Nov 2023 09:03:40 GMT  
		Size: 299.5 KB (299459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:65ff09ea62f27d174a9ab498b66f8e078c539e277d72dde120be1d784d0b33d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60103165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9cdfc9c3f3e4a4074d910f9e1a11f5fb576f177779f1c74e9cef6d7b6e7fcd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:02 GMT
ADD file:e3f63671dca138b2b525b60f1471241941cdf4dab7f0c17cd91124978716bd93 in / 
# Wed, 01 Nov 2023 00:40:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:28:05 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:28:07 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Nov 2023 11:28:07 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Nov 2023 11:28:10 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3db7215fb502c5873a81db7c6fd3214f199f6a1d8034da9d90918ac3220b20b`  
		Last Modified: Wed, 01 Nov 2023 00:44:04 GMT  
		Size: 49.3 MB (49291092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929f0a42bee1218ebcc451261cd112239c22bce8e4e163dfacbc1c27fb0ff111`  
		Last Modified: Wed, 01 Nov 2023 11:29:36 GMT  
		Size: 10.5 MB (10510591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e0a85c2b7105ae379c7ce849dff682eb5c233ad7046b7f6fd728edf5fab473`  
		Last Modified: Wed, 01 Nov 2023 11:29:35 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47702ffaad8de982eefaca460984971aaac1b75d371e36a8d74b7ee70f74618`  
		Last Modified: Wed, 01 Nov 2023 11:29:35 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64014833cfbdf221ad8a1aeaa21acf2dc6632670a2febd0ff9837ddb3c079b24`  
		Last Modified: Wed, 01 Nov 2023 11:29:35 GMT  
		Size: 299.5 KB (299470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; 386

```console
$ docker pull neurodebian@sha256:1ecb0cac7f6e32bd00b8f0db9635e1ad0616806c7a556970468258c022c00467
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d28349190f4c8e45f6bb3133aed1283f04fffe7cf0cc59706664a2c9d3bcd591`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:26 GMT
ADD file:3a91c3eed04829ed9d8801ae9da9d5dfb67139d59f8b98f87943131fc8953b49 in / 
# Tue, 21 Nov 2023 04:40:27 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:30:33 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:30:35 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 21 Nov 2023 14:30:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 21 Nov 2023 14:30:40 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d9ff368d73b50f922dcf47b179053552ad7a9257e80ae0ef12ba15c8ca86eb6f`  
		Last Modified: Tue, 21 Nov 2023 04:45:46 GMT  
		Size: 51.3 MB (51256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d631fe7e73cce5c0cebec053d20fd52490e8475b7ddfb8aa4c12bd9b479371`  
		Last Modified: Tue, 21 Nov 2023 14:32:16 GMT  
		Size: 10.9 MB (10868370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328e908e98f102a385df52ceb1d57ca577dda9c0ca3e3d5486145e5f40f889e9`  
		Last Modified: Tue, 21 Nov 2023 14:32:14 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649bf93c2b54d5917459ae3f83205a75951604fc1d438b2eff2783ab68947191`  
		Last Modified: Tue, 21 Nov 2023 14:32:14 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a542ecd4d7636ce47718ba930c6bf8517e6edb4b32e14be5a3583fe70d943e`  
		Last Modified: Tue, 21 Nov 2023 14:32:14 GMT  
		Size: 299.4 KB (299407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
