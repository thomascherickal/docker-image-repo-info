<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neurodebian`

-	[`neurodebian:bionic`](#neurodebianbionic)
-	[`neurodebian:bionic-non-free`](#neurodebianbionic-non-free)
-	[`neurodebian:bullseye`](#neurodebianbullseye)
-	[`neurodebian:bullseye-non-free`](#neurodebianbullseye-non-free)
-	[`neurodebian:buster`](#neurodebianbuster)
-	[`neurodebian:buster-non-free`](#neurodebianbuster-non-free)
-	[`neurodebian:focal`](#neurodebianfocal)
-	[`neurodebian:focal-non-free`](#neurodebianfocal-non-free)
-	[`neurodebian:groovy`](#neurodebiangroovy)
-	[`neurodebian:groovy-non-free`](#neurodebiangroovy-non-free)
-	[`neurodebian:hirsute`](#neurodebianhirsute)
-	[`neurodebian:hirsute-non-free`](#neurodebianhirsute-non-free)
-	[`neurodebian:latest`](#neurodebianlatest)
-	[`neurodebian:nd`](#neurodebiannd)
-	[`neurodebian:nd-non-free`](#neurodebiannd-non-free)
-	[`neurodebian:nd100`](#neurodebiannd100)
-	[`neurodebian:nd100-non-free`](#neurodebiannd100-non-free)
-	[`neurodebian:nd110`](#neurodebiannd110)
-	[`neurodebian:nd110-non-free`](#neurodebiannd110-non-free)
-	[`neurodebian:nd16.04`](#neurodebiannd1604)
-	[`neurodebian:nd16.04-non-free`](#neurodebiannd1604-non-free)
-	[`neurodebian:nd18.04`](#neurodebiannd1804)
-	[`neurodebian:nd18.04-non-free`](#neurodebiannd1804-non-free)
-	[`neurodebian:nd20.04`](#neurodebiannd2004)
-	[`neurodebian:nd20.04-non-free`](#neurodebiannd2004-non-free)
-	[`neurodebian:nd20.10`](#neurodebiannd2010)
-	[`neurodebian:nd20.10-non-free`](#neurodebiannd2010-non-free)
-	[`neurodebian:nd21.04`](#neurodebiannd2104)
-	[`neurodebian:nd21.04-non-free`](#neurodebiannd2104-non-free)
-	[`neurodebian:nd90`](#neurodebiannd90)
-	[`neurodebian:nd90-non-free`](#neurodebiannd90-non-free)
-	[`neurodebian:non-free`](#neurodebiannon-free)
-	[`neurodebian:sid`](#neurodebiansid)
-	[`neurodebian:sid-non-free`](#neurodebiansid-non-free)
-	[`neurodebian:stretch`](#neurodebianstretch)
-	[`neurodebian:stretch-non-free`](#neurodebianstretch-non-free)
-	[`neurodebian:xenial`](#neurodebianxenial)
-	[`neurodebian:xenial-non-free`](#neurodebianxenial-non-free)

## `neurodebian:bionic`

```console
$ docker pull neurodebian@sha256:b0fd331f66e6c33eec1df7459fe4538498b2f478b879a5ad5289f7429943ea0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:4c7bf5a8f54ef4afda97fc9a5264fe20e0d66bc5c1c439dbc291e8127ca3b064
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31762983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ace3adcfa36fa9382e4997f808d2e5cf28834840f0af2f289ef23adb70e8d3d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:19:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:19:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:19:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194ba06a10736483e9750b491863cf4336dcd732e10ee8814e3354d755b414d0`  
		Last Modified: Wed, 14 Jul 2021 01:21:58 GMT  
		Size: 4.8 MB (4813364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e6acf54af43301de699d81bb6d7b73f55735de436d46260fc8e091842cbb39`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 3.2 KB (3158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a933b73acd672d58eead763c7c6f90165df957814a67d1a9aae03bdd6f664b57`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe8a6ce38f60ddcc289d988557d337cae7d388774054bfe84a232b716b56cff`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 240.1 KB (240071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bionic-non-free`

```console
$ docker pull neurodebian@sha256:83480bf0323c5ed0fbb8540d2f820d3ebe58c0fc1d156371bffcb24e8265ede7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bionic-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:766c57564bb0598f46f8161c6633ec683d5c3a1a91fff2097f2b4e08eeac116e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31763237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8754d66c16bf54ee0f03aac8333ca71ab49561cccbacf918d3f06d72932dedab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:19:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:19:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:19:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:30 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194ba06a10736483e9750b491863cf4336dcd732e10ee8814e3354d755b414d0`  
		Last Modified: Wed, 14 Jul 2021 01:21:58 GMT  
		Size: 4.8 MB (4813364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e6acf54af43301de699d81bb6d7b73f55735de436d46260fc8e091842cbb39`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 3.2 KB (3158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a933b73acd672d58eead763c7c6f90165df957814a67d1a9aae03bdd6f664b57`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe8a6ce38f60ddcc289d988557d337cae7d388774054bfe84a232b716b56cff`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 240.1 KB (240071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030c45867bc6edf34c816e0f78c2a8ca4db22c978caaa58a54b01b2a57298c75`  
		Last Modified: Wed, 14 Jul 2021 01:22:08 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:2625e7de7abd3d04ee57f37abc72558026048e8cc0023c85172483d478234569
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:0343475923907c9b0cb0d89e641a15e43a21a575aeecb7da3728ac287f81bef7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66527511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538cbb0a079bab74399e2747907f54adb09fe1eec0d5aac09fc130aaa5e7286c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:02 GMT
ADD file:fca2ea6b8fc69f3efb8a2f21cd3877d23a9ee3fbeee6ebe4fe21541cd1606a8c in / 
# Thu, 22 Jul 2021 00:45:03 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:57 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:58 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:59 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:52:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a72d62e9d2fef13cf62e5d212cc6a3751b5c388cc6657bebf4dabc0ca3603cb`  
		Last Modified: Thu, 22 Jul 2021 00:49:21 GMT  
		Size: 54.9 MB (54904849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f80af7c5f675200465ac739aa50787ad204858b7e71bb0a4ce96ed41e44d53`  
		Last Modified: Thu, 22 Jul 2021 09:54:42 GMT  
		Size: 11.3 MB (11309473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70904cebde341b794981e76734af21ac7319970107e56dc693bb209e413cd75f`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e537da9c3e2291faac290662b5c173737fdea9b60ba742794e974b604ecb76`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0950288e46c4a44c74f59f4162507b0387c96e3bfdf4c4d0a291dba6da95b498`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 311.2 KB (311175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:d114345bcb88b9ffc5807bd5a5291bf4bbc3261c89c243058934b25a45749545
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:7ec317e248f35956bf13829624ed3582903405152fe85169d7fe220841b4f77f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66527875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:553f1110a311b87b8fc6ba1cd9c3bb2e24cdb9883c262931c914f0b4d1ba663d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:02 GMT
ADD file:fca2ea6b8fc69f3efb8a2f21cd3877d23a9ee3fbeee6ebe4fe21541cd1606a8c in / 
# Thu, 22 Jul 2021 00:45:03 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:57 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:58 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:59 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:52:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:52:08 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:7a72d62e9d2fef13cf62e5d212cc6a3751b5c388cc6657bebf4dabc0ca3603cb`  
		Last Modified: Thu, 22 Jul 2021 00:49:21 GMT  
		Size: 54.9 MB (54904849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f80af7c5f675200465ac739aa50787ad204858b7e71bb0a4ce96ed41e44d53`  
		Last Modified: Thu, 22 Jul 2021 09:54:42 GMT  
		Size: 11.3 MB (11309473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70904cebde341b794981e76734af21ac7319970107e56dc693bb209e413cd75f`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e537da9c3e2291faac290662b5c173737fdea9b60ba742794e974b604ecb76`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0950288e46c4a44c74f59f4162507b0387c96e3bfdf4c4d0a291dba6da95b498`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 311.2 KB (311175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ad9313e27a86504e430ca0d38e8e983b794ee5e7f5550e4e3603d9855dd4ef`  
		Last Modified: Thu, 22 Jul 2021 09:54:52 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:3ea779c45743abd02464e211b4c6816184780f088d18f7739e2a735d2b7bfca6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:5fb8ea9a5123dde129b86a480b1d341462c8e0ef22dce6eadd75cfab37eef467
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61240359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a50ad57636ca67a54ee8207060850dca605fda2affdadc364fb29b59539f43`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff66d7acb9e05c47e0621027afb45a8dfa4665301a45f8f794a16bd8c8ae8205`  
		Last Modified: Thu, 22 Jul 2021 09:54:11 GMT  
		Size: 10.5 MB (10499949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac627f2d764f56d7380099754dd943f54a31247e9400d632a215b8bc4ec5fa2`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33c3e9e07dc85213c696c81aff06d286ba379571b799845954b6cc776457e5f`  
		Last Modified: Thu, 22 Jul 2021 09:54:09 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c4b1dfc179a7cb39a5bcbff0f4d529c84d1fab9395e799ab8a0350c620e58`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 302.8 KB (302773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:c53593105b6976b3e1b0a7471aeedcd6a1893b585fde59c17ff7ac1456694b01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:0ed1185fa7c3ad9fbcd0fb3f165204cf75508f9a98563c4a5209ea677a6c7902
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61240723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:310ef8d41a0013c86b5d8085e5839affed1cc00e9e8b582738e9908d6564b539`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:45 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff66d7acb9e05c47e0621027afb45a8dfa4665301a45f8f794a16bd8c8ae8205`  
		Last Modified: Thu, 22 Jul 2021 09:54:11 GMT  
		Size: 10.5 MB (10499949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac627f2d764f56d7380099754dd943f54a31247e9400d632a215b8bc4ec5fa2`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33c3e9e07dc85213c696c81aff06d286ba379571b799845954b6cc776457e5f`  
		Last Modified: Thu, 22 Jul 2021 09:54:09 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c4b1dfc179a7cb39a5bcbff0f4d529c84d1fab9395e799ab8a0350c620e58`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 302.8 KB (302773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a42860b1360435ab5bdf409f82263bf9f069a75f834afae3bcaedd3255b6ae6`  
		Last Modified: Thu, 22 Jul 2021 09:54:26 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal`

```console
$ docker pull neurodebian@sha256:8f7876dc77c57630ce3a62c209e29e0461872bff43d73635d0806103de812f37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:e6dac86737fcbd72c411fd8ce6d55a239224738f79464a36d3898589c175956d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34294659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afaac688d6899bea91feb7e1e32ebc5558bf2f1ffed1009f28d3a9622ac8e4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:19:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:19:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:19:48 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613af0476aa971fdf7e222f06ba33ac8cf19af6cc272bfd30d31cef3dca8a55`  
		Last Modified: Wed, 14 Jul 2021 01:22:20 GMT  
		Size: 5.5 MB (5488761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7181a6ff15d1b90770aeba13bc7785303fadcaeb6e27cfcc899554cd5d6336b7`  
		Last Modified: Wed, 14 Jul 2021 01:22:19 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b5f9e69eac46a34de72ed33138bef457347213fb5293dd43b201bd2ea6e84`  
		Last Modified: Wed, 14 Jul 2021 01:22:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1976000c24c2fea28567f1a3d4d4b15a44a4b1d05ae10ebb06bf1c3ee9ca0c`  
		Last Modified: Wed, 14 Jul 2021 01:22:19 GMT  
		Size: 238.0 KB (238023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal-non-free`

```console
$ docker pull neurodebian@sha256:91b4e98452f060fdb303a62553a0edce105b00bb7618f4c544b30741ba3edccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:focal-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:05ae565ed4e411760249ff2bc2fe02a6eb76a56604cee4ad7857ab75178acf95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34294916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651d24e05475991c4ce4d257ebeac31f86c1755a552f2254f4fd6eedfdef436c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:19:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:19:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:19:48 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:52 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613af0476aa971fdf7e222f06ba33ac8cf19af6cc272bfd30d31cef3dca8a55`  
		Last Modified: Wed, 14 Jul 2021 01:22:20 GMT  
		Size: 5.5 MB (5488761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7181a6ff15d1b90770aeba13bc7785303fadcaeb6e27cfcc899554cd5d6336b7`  
		Last Modified: Wed, 14 Jul 2021 01:22:19 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b5f9e69eac46a34de72ed33138bef457347213fb5293dd43b201bd2ea6e84`  
		Last Modified: Wed, 14 Jul 2021 01:22:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1976000c24c2fea28567f1a3d4d4b15a44a4b1d05ae10ebb06bf1c3ee9ca0c`  
		Last Modified: Wed, 14 Jul 2021 01:22:19 GMT  
		Size: 238.0 KB (238023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a6a0ae191ee945793986c336fcb14e69096ef113af114fd900c343201e5781`  
		Last Modified: Wed, 14 Jul 2021 01:22:31 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:groovy`

```console
$ docker pull neurodebian@sha256:40b8b4f970d3c3152690a007450670aa5860900a5ff8238fc01ccc8c352748ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:groovy` - linux; amd64

```console
$ docker pull neurodebian@sha256:a82c4bbcd711692bb9e33fa9f35f532fa152b9edaa0a322aeeeb538d10b18f08
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37194238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffcd1d0e214437d8f646c7e48826e769a3d1b0ede560f663b79e57ac1a0f0a66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:45 GMT
ADD file:aa87e1d15a8d4e3640ec67e03ae6c4421158f4c64c838d701d82eb34722a2e3a in / 
# Tue, 13 Jul 2021 22:29:46 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:20:11 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:20:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian groovy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel groovy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:20:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87103eef5146121c4b54992b41b2da8c9e671d21961ba24cfe5c1756737d5698`  
		Last Modified: Tue, 13 Jul 2021 22:31:40 GMT  
		Size: 31.3 MB (31341566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f1d104b6aee3f867817b0367346635b4e81879e7479396f19baf28f2828dbf`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 5.6 MB (5595819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc654e221832c02bf3841a83892315a0a023cf8eba64014112cf871e1d1f24e`  
		Last Modified: Wed, 14 Jul 2021 01:22:41 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b3fdda8a5369e25b836dc7654e4af4d201272b291e457b8a98e061c0a1a04d`  
		Last Modified: Wed, 14 Jul 2021 01:22:41 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab0b42f706e33c968656cb598d7cdbe2bd933bbce751831eab849fc9d091af`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 254.8 KB (254838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:groovy-non-free`

```console
$ docker pull neurodebian@sha256:2f59bba9f75c24fbe940f68c286baf4e8b2d0ddb3f0fbd39e8999860d7b7f721
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:groovy-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:d00a28546b4b0d52d87df02841ee322bdff41ee07b333d128d435cb1812d84e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37194497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbcffd9fd342f012852cb953b82f2c19a136ebfa0b51b59be9c48b8358db6d0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:45 GMT
ADD file:aa87e1d15a8d4e3640ec67e03ae6c4421158f4c64c838d701d82eb34722a2e3a in / 
# Tue, 13 Jul 2021 22:29:46 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:20:11 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:20:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian groovy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel groovy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:20:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:25 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:87103eef5146121c4b54992b41b2da8c9e671d21961ba24cfe5c1756737d5698`  
		Last Modified: Tue, 13 Jul 2021 22:31:40 GMT  
		Size: 31.3 MB (31341566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f1d104b6aee3f867817b0367346635b4e81879e7479396f19baf28f2828dbf`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 5.6 MB (5595819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc654e221832c02bf3841a83892315a0a023cf8eba64014112cf871e1d1f24e`  
		Last Modified: Wed, 14 Jul 2021 01:22:41 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b3fdda8a5369e25b836dc7654e4af4d201272b291e457b8a98e061c0a1a04d`  
		Last Modified: Wed, 14 Jul 2021 01:22:41 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab0b42f706e33c968656cb598d7cdbe2bd933bbce751831eab849fc9d091af`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 254.8 KB (254838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7680de57801808a2ef51514e6555e631ae9b8de6c0ce8aa7029c027fe5eaebaf`  
		Last Modified: Wed, 14 Jul 2021 01:22:52 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:hirsute`

```console
$ docker pull neurodebian@sha256:f58e887ef774d54aaff62f1d4b42e998f81ed9fc383793dafb90a9f6c59b7dfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:hirsute` - linux; amd64

```console
$ docker pull neurodebian@sha256:309620dae2b4f329d278e7ced27ea06597d01fd28926c552ff9a20932d46216a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37688094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c63775aa45dc7839be067a59162b91a6726ccdd57e367159b496f0710b12e30a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:57 GMT
ADD file:af305d3eb867f312743f97d1cbed14ee2a155fdfed4621c72a8e8cf25355660c in / 
# Tue, 13 Jul 2021 22:29:57 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:20:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:20:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian hirsute main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel hirsute main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:20:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:966b3c5c8637e41360eed39a59e6c16ee1e986f7f2b92244e4d39f7ca6669618`  
		Last Modified: Tue, 13 Jul 2021 22:31:57 GMT  
		Size: 31.8 MB (31836858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6174bb4728b14be1ee1b3dc8c9856679c536960bf2cdeb5739d9776968641e`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 5.6 MB (5598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11e5a9b959c308ffb520739593aae1d3d73f2795b2b364fc618a749251f7162`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c62c59144a54d5082baddb64ce4afb511b973a905db04401bab9ed6ef686c9`  
		Last Modified: Wed, 14 Jul 2021 01:23:02 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07c9680d47b4272f33a0c462cf6547f8721c0bcf2bf152c26ab458691c43ae0`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 250.4 KB (250422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:hirsute-non-free`

```console
$ docker pull neurodebian@sha256:fae34ae4ede0fc837cf0b7e8f27d43d401d3c6846c47e07a3a3a2a7ac567b3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:hirsute-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:967d0f18a999a175f6757bbcac24b304c79fa0ff2edd91604d75c7d648c7c78e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37688353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ec1f95ed830f7eabfa1e441f0bf0b1828ac253b1ef4de221cb0df127aa1e4a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:57 GMT
ADD file:af305d3eb867f312743f97d1cbed14ee2a155fdfed4621c72a8e8cf25355660c in / 
# Tue, 13 Jul 2021 22:29:57 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:20:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:20:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian hirsute main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel hirsute main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:20:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:54 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:966b3c5c8637e41360eed39a59e6c16ee1e986f7f2b92244e4d39f7ca6669618`  
		Last Modified: Tue, 13 Jul 2021 22:31:57 GMT  
		Size: 31.8 MB (31836858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6174bb4728b14be1ee1b3dc8c9856679c536960bf2cdeb5739d9776968641e`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 5.6 MB (5598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11e5a9b959c308ffb520739593aae1d3d73f2795b2b364fc618a749251f7162`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c62c59144a54d5082baddb64ce4afb511b973a905db04401bab9ed6ef686c9`  
		Last Modified: Wed, 14 Jul 2021 01:23:02 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07c9680d47b4272f33a0c462cf6547f8721c0bcf2bf152c26ab458691c43ae0`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 250.4 KB (250422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea77cc98717c64aef1424fa72704630a0d800ec82634b96ad3fe3d833abfc1cf`  
		Last Modified: Wed, 14 Jul 2021 01:23:16 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:3ea779c45743abd02464e211b4c6816184780f088d18f7739e2a735d2b7bfca6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:5fb8ea9a5123dde129b86a480b1d341462c8e0ef22dce6eadd75cfab37eef467
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61240359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a50ad57636ca67a54ee8207060850dca605fda2affdadc364fb29b59539f43`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff66d7acb9e05c47e0621027afb45a8dfa4665301a45f8f794a16bd8c8ae8205`  
		Last Modified: Thu, 22 Jul 2021 09:54:11 GMT  
		Size: 10.5 MB (10499949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac627f2d764f56d7380099754dd943f54a31247e9400d632a215b8bc4ec5fa2`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33c3e9e07dc85213c696c81aff06d286ba379571b799845954b6cc776457e5f`  
		Last Modified: Thu, 22 Jul 2021 09:54:09 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c4b1dfc179a7cb39a5bcbff0f4d529c84d1fab9395e799ab8a0350c620e58`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 302.8 KB (302773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:2ee65aa92aad3610cc167554c656d5dbe94b063975c5c8aa7d74033e3d34b2e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:082ca4751fb886450170ef204a85b03b2f99fe2dc807f85763ffb3aa955b1455
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66532325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce77c88e1b97352a7d6577b575a7320dafb73d776f427a62f6d81a0e9bd52e6c`
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
# Thu, 22 Jul 2021 09:52:30 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
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
	-	`sha256:0974a17fac1ea186c3ba9c50cf8ef1e640af0298dfb84c2e683cc1571d20bc71`  
		Last Modified: Thu, 22 Jul 2021 09:55:14 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100`

```console
$ docker pull neurodebian@sha256:3ea779c45743abd02464e211b4c6816184780f088d18f7739e2a735d2b7bfca6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd100` - linux; amd64

```console
$ docker pull neurodebian@sha256:5fb8ea9a5123dde129b86a480b1d341462c8e0ef22dce6eadd75cfab37eef467
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61240359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a50ad57636ca67a54ee8207060850dca605fda2affdadc364fb29b59539f43`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff66d7acb9e05c47e0621027afb45a8dfa4665301a45f8f794a16bd8c8ae8205`  
		Last Modified: Thu, 22 Jul 2021 09:54:11 GMT  
		Size: 10.5 MB (10499949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac627f2d764f56d7380099754dd943f54a31247e9400d632a215b8bc4ec5fa2`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33c3e9e07dc85213c696c81aff06d286ba379571b799845954b6cc776457e5f`  
		Last Modified: Thu, 22 Jul 2021 09:54:09 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c4b1dfc179a7cb39a5bcbff0f4d529c84d1fab9395e799ab8a0350c620e58`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 302.8 KB (302773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:c53593105b6976b3e1b0a7471aeedcd6a1893b585fde59c17ff7ac1456694b01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:0ed1185fa7c3ad9fbcd0fb3f165204cf75508f9a98563c4a5209ea677a6c7902
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61240723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:310ef8d41a0013c86b5d8085e5839affed1cc00e9e8b582738e9908d6564b539`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:45 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff66d7acb9e05c47e0621027afb45a8dfa4665301a45f8f794a16bd8c8ae8205`  
		Last Modified: Thu, 22 Jul 2021 09:54:11 GMT  
		Size: 10.5 MB (10499949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac627f2d764f56d7380099754dd943f54a31247e9400d632a215b8bc4ec5fa2`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33c3e9e07dc85213c696c81aff06d286ba379571b799845954b6cc776457e5f`  
		Last Modified: Thu, 22 Jul 2021 09:54:09 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c4b1dfc179a7cb39a5bcbff0f4d529c84d1fab9395e799ab8a0350c620e58`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 302.8 KB (302773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a42860b1360435ab5bdf409f82263bf9f069a75f834afae3bcaedd3255b6ae6`  
		Last Modified: Thu, 22 Jul 2021 09:54:26 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110`

```console
$ docker pull neurodebian@sha256:2625e7de7abd3d04ee57f37abc72558026048e8cc0023c85172483d478234569
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd110` - linux; amd64

```console
$ docker pull neurodebian@sha256:0343475923907c9b0cb0d89e641a15e43a21a575aeecb7da3728ac287f81bef7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66527511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538cbb0a079bab74399e2747907f54adb09fe1eec0d5aac09fc130aaa5e7286c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:02 GMT
ADD file:fca2ea6b8fc69f3efb8a2f21cd3877d23a9ee3fbeee6ebe4fe21541cd1606a8c in / 
# Thu, 22 Jul 2021 00:45:03 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:57 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:58 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:59 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:52:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a72d62e9d2fef13cf62e5d212cc6a3751b5c388cc6657bebf4dabc0ca3603cb`  
		Last Modified: Thu, 22 Jul 2021 00:49:21 GMT  
		Size: 54.9 MB (54904849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f80af7c5f675200465ac739aa50787ad204858b7e71bb0a4ce96ed41e44d53`  
		Last Modified: Thu, 22 Jul 2021 09:54:42 GMT  
		Size: 11.3 MB (11309473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70904cebde341b794981e76734af21ac7319970107e56dc693bb209e413cd75f`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e537da9c3e2291faac290662b5c173737fdea9b60ba742794e974b604ecb76`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0950288e46c4a44c74f59f4162507b0387c96e3bfdf4c4d0a291dba6da95b498`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 311.2 KB (311175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:d114345bcb88b9ffc5807bd5a5291bf4bbc3261c89c243058934b25a45749545
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:7ec317e248f35956bf13829624ed3582903405152fe85169d7fe220841b4f77f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66527875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:553f1110a311b87b8fc6ba1cd9c3bb2e24cdb9883c262931c914f0b4d1ba663d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:02 GMT
ADD file:fca2ea6b8fc69f3efb8a2f21cd3877d23a9ee3fbeee6ebe4fe21541cd1606a8c in / 
# Thu, 22 Jul 2021 00:45:03 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:57 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:58 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:59 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:52:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:52:08 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:7a72d62e9d2fef13cf62e5d212cc6a3751b5c388cc6657bebf4dabc0ca3603cb`  
		Last Modified: Thu, 22 Jul 2021 00:49:21 GMT  
		Size: 54.9 MB (54904849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f80af7c5f675200465ac739aa50787ad204858b7e71bb0a4ce96ed41e44d53`  
		Last Modified: Thu, 22 Jul 2021 09:54:42 GMT  
		Size: 11.3 MB (11309473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70904cebde341b794981e76734af21ac7319970107e56dc693bb209e413cd75f`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e537da9c3e2291faac290662b5c173737fdea9b60ba742794e974b604ecb76`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0950288e46c4a44c74f59f4162507b0387c96e3bfdf4c4d0a291dba6da95b498`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 311.2 KB (311175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ad9313e27a86504e430ca0d38e8e983b794ee5e7f5550e4e3603d9855dd4ef`  
		Last Modified: Thu, 22 Jul 2021 09:54:52 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd16.04`

```console
$ docker pull neurodebian@sha256:706422ad8751b16d4421f5c37474d10da64d708f89d0d19eae16587c32b2a0b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd16.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:4471dff78eb2b61d7c0fe05c386984cee1ecffe25994d149995dd32d4c77900f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46728844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81ebe285f4f396273f6e8f2b6ef3ef3f9e05f6fa87a6d16ffb9e12ce02da140`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 04:51:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:51:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 18 Jun 2021 04:51:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 18 Jun 2021 04:51:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27db3f87344ee4f403c5257877584f0b0319c19914fa2953e351715240aa547`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d325b9a44fc4bfd2ef838143c6afeeed1fbf4929cc69351b13790404151baf`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 3.1 KB (3150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a309011e84c623c2b39ed13ff0f62d5c0f40e9ae798cdf37fba510c34711c6`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea488f510caf428861b3edf4b32605992b348a0f4ec00ee2e81a581d8e80f80`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 226.9 KB (226939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd16.04-non-free`

```console
$ docker pull neurodebian@sha256:937cdaf8ad5054fd931a11a6bb0a8b4c0840a0a115540e98879ea449f69e1dbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd16.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:0041163886c00bd41f9d9eaf5748fbc5b2e178e4d191beb751fb7e2659256870
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:816d85192005dbf8618fa9b54d5b0ae148f0cf0104fb9268b604dad9648aa060`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 04:51:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:51:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 18 Jun 2021 04:51:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 18 Jun 2021 04:51:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:51:57 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27db3f87344ee4f403c5257877584f0b0319c19914fa2953e351715240aa547`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d325b9a44fc4bfd2ef838143c6afeeed1fbf4929cc69351b13790404151baf`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 3.1 KB (3150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a309011e84c623c2b39ed13ff0f62d5c0f40e9ae798cdf37fba510c34711c6`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea488f510caf428861b3edf4b32605992b348a0f4ec00ee2e81a581d8e80f80`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 226.9 KB (226939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901921b5a6b1c35d7c4d2819f403cac6c89c2165b3d2c26ed9a7741007b3aae`  
		Last Modified: Fri, 18 Jun 2021 04:54:51 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04`

```console
$ docker pull neurodebian@sha256:b0fd331f66e6c33eec1df7459fe4538498b2f478b879a5ad5289f7429943ea0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd18.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:4c7bf5a8f54ef4afda97fc9a5264fe20e0d66bc5c1c439dbc291e8127ca3b064
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31762983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ace3adcfa36fa9382e4997f808d2e5cf28834840f0af2f289ef23adb70e8d3d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:19:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:19:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:19:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194ba06a10736483e9750b491863cf4336dcd732e10ee8814e3354d755b414d0`  
		Last Modified: Wed, 14 Jul 2021 01:21:58 GMT  
		Size: 4.8 MB (4813364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e6acf54af43301de699d81bb6d7b73f55735de436d46260fc8e091842cbb39`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 3.2 KB (3158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a933b73acd672d58eead763c7c6f90165df957814a67d1a9aae03bdd6f664b57`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe8a6ce38f60ddcc289d988557d337cae7d388774054bfe84a232b716b56cff`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 240.1 KB (240071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04-non-free`

```console
$ docker pull neurodebian@sha256:83480bf0323c5ed0fbb8540d2f820d3ebe58c0fc1d156371bffcb24e8265ede7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd18.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:766c57564bb0598f46f8161c6633ec683d5c3a1a91fff2097f2b4e08eeac116e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31763237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8754d66c16bf54ee0f03aac8333ca71ab49561cccbacf918d3f06d72932dedab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:19:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:19:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:19:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:30 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194ba06a10736483e9750b491863cf4336dcd732e10ee8814e3354d755b414d0`  
		Last Modified: Wed, 14 Jul 2021 01:21:58 GMT  
		Size: 4.8 MB (4813364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e6acf54af43301de699d81bb6d7b73f55735de436d46260fc8e091842cbb39`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 3.2 KB (3158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a933b73acd672d58eead763c7c6f90165df957814a67d1a9aae03bdd6f664b57`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe8a6ce38f60ddcc289d988557d337cae7d388774054bfe84a232b716b56cff`  
		Last Modified: Wed, 14 Jul 2021 01:21:57 GMT  
		Size: 240.1 KB (240071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030c45867bc6edf34c816e0f78c2a8ca4db22c978caaa58a54b01b2a57298c75`  
		Last Modified: Wed, 14 Jul 2021 01:22:08 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04`

```console
$ docker pull neurodebian@sha256:8f7876dc77c57630ce3a62c209e29e0461872bff43d73635d0806103de812f37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd20.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:e6dac86737fcbd72c411fd8ce6d55a239224738f79464a36d3898589c175956d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34294659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afaac688d6899bea91feb7e1e32ebc5558bf2f1ffed1009f28d3a9622ac8e4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:19:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:19:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:19:48 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613af0476aa971fdf7e222f06ba33ac8cf19af6cc272bfd30d31cef3dca8a55`  
		Last Modified: Wed, 14 Jul 2021 01:22:20 GMT  
		Size: 5.5 MB (5488761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7181a6ff15d1b90770aeba13bc7785303fadcaeb6e27cfcc899554cd5d6336b7`  
		Last Modified: Wed, 14 Jul 2021 01:22:19 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b5f9e69eac46a34de72ed33138bef457347213fb5293dd43b201bd2ea6e84`  
		Last Modified: Wed, 14 Jul 2021 01:22:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1976000c24c2fea28567f1a3d4d4b15a44a4b1d05ae10ebb06bf1c3ee9ca0c`  
		Last Modified: Wed, 14 Jul 2021 01:22:19 GMT  
		Size: 238.0 KB (238023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04-non-free`

```console
$ docker pull neurodebian@sha256:91b4e98452f060fdb303a62553a0edce105b00bb7618f4c544b30741ba3edccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd20.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:05ae565ed4e411760249ff2bc2fe02a6eb76a56604cee4ad7857ab75178acf95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34294916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651d24e05475991c4ce4d257ebeac31f86c1755a552f2254f4fd6eedfdef436c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:19:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:19:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:19:48 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:19:52 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613af0476aa971fdf7e222f06ba33ac8cf19af6cc272bfd30d31cef3dca8a55`  
		Last Modified: Wed, 14 Jul 2021 01:22:20 GMT  
		Size: 5.5 MB (5488761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7181a6ff15d1b90770aeba13bc7785303fadcaeb6e27cfcc899554cd5d6336b7`  
		Last Modified: Wed, 14 Jul 2021 01:22:19 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b5f9e69eac46a34de72ed33138bef457347213fb5293dd43b201bd2ea6e84`  
		Last Modified: Wed, 14 Jul 2021 01:22:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1976000c24c2fea28567f1a3d4d4b15a44a4b1d05ae10ebb06bf1c3ee9ca0c`  
		Last Modified: Wed, 14 Jul 2021 01:22:19 GMT  
		Size: 238.0 KB (238023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a6a0ae191ee945793986c336fcb14e69096ef113af114fd900c343201e5781`  
		Last Modified: Wed, 14 Jul 2021 01:22:31 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.10`

```console
$ docker pull neurodebian@sha256:40b8b4f970d3c3152690a007450670aa5860900a5ff8238fc01ccc8c352748ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd20.10` - linux; amd64

```console
$ docker pull neurodebian@sha256:a82c4bbcd711692bb9e33fa9f35f532fa152b9edaa0a322aeeeb538d10b18f08
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37194238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffcd1d0e214437d8f646c7e48826e769a3d1b0ede560f663b79e57ac1a0f0a66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:45 GMT
ADD file:aa87e1d15a8d4e3640ec67e03ae6c4421158f4c64c838d701d82eb34722a2e3a in / 
# Tue, 13 Jul 2021 22:29:46 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:20:11 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:20:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian groovy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel groovy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:20:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87103eef5146121c4b54992b41b2da8c9e671d21961ba24cfe5c1756737d5698`  
		Last Modified: Tue, 13 Jul 2021 22:31:40 GMT  
		Size: 31.3 MB (31341566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f1d104b6aee3f867817b0367346635b4e81879e7479396f19baf28f2828dbf`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 5.6 MB (5595819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc654e221832c02bf3841a83892315a0a023cf8eba64014112cf871e1d1f24e`  
		Last Modified: Wed, 14 Jul 2021 01:22:41 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b3fdda8a5369e25b836dc7654e4af4d201272b291e457b8a98e061c0a1a04d`  
		Last Modified: Wed, 14 Jul 2021 01:22:41 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab0b42f706e33c968656cb598d7cdbe2bd933bbce751831eab849fc9d091af`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 254.8 KB (254838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.10-non-free`

```console
$ docker pull neurodebian@sha256:2f59bba9f75c24fbe940f68c286baf4e8b2d0ddb3f0fbd39e8999860d7b7f721
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd20.10-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:d00a28546b4b0d52d87df02841ee322bdff41ee07b333d128d435cb1812d84e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37194497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbcffd9fd342f012852cb953b82f2c19a136ebfa0b51b59be9c48b8358db6d0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:45 GMT
ADD file:aa87e1d15a8d4e3640ec67e03ae6c4421158f4c64c838d701d82eb34722a2e3a in / 
# Tue, 13 Jul 2021 22:29:46 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:20:11 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:20:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian groovy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel groovy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:20:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:25 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:87103eef5146121c4b54992b41b2da8c9e671d21961ba24cfe5c1756737d5698`  
		Last Modified: Tue, 13 Jul 2021 22:31:40 GMT  
		Size: 31.3 MB (31341566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f1d104b6aee3f867817b0367346635b4e81879e7479396f19baf28f2828dbf`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 5.6 MB (5595819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc654e221832c02bf3841a83892315a0a023cf8eba64014112cf871e1d1f24e`  
		Last Modified: Wed, 14 Jul 2021 01:22:41 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b3fdda8a5369e25b836dc7654e4af4d201272b291e457b8a98e061c0a1a04d`  
		Last Modified: Wed, 14 Jul 2021 01:22:41 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab0b42f706e33c968656cb598d7cdbe2bd933bbce751831eab849fc9d091af`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 254.8 KB (254838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7680de57801808a2ef51514e6555e631ae9b8de6c0ce8aa7029c027fe5eaebaf`  
		Last Modified: Wed, 14 Jul 2021 01:22:52 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd21.04`

```console
$ docker pull neurodebian@sha256:f58e887ef774d54aaff62f1d4b42e998f81ed9fc383793dafb90a9f6c59b7dfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd21.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:309620dae2b4f329d278e7ced27ea06597d01fd28926c552ff9a20932d46216a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37688094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c63775aa45dc7839be067a59162b91a6726ccdd57e367159b496f0710b12e30a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:57 GMT
ADD file:af305d3eb867f312743f97d1cbed14ee2a155fdfed4621c72a8e8cf25355660c in / 
# Tue, 13 Jul 2021 22:29:57 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:20:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:20:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian hirsute main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel hirsute main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:20:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:966b3c5c8637e41360eed39a59e6c16ee1e986f7f2b92244e4d39f7ca6669618`  
		Last Modified: Tue, 13 Jul 2021 22:31:57 GMT  
		Size: 31.8 MB (31836858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6174bb4728b14be1ee1b3dc8c9856679c536960bf2cdeb5739d9776968641e`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 5.6 MB (5598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11e5a9b959c308ffb520739593aae1d3d73f2795b2b364fc618a749251f7162`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c62c59144a54d5082baddb64ce4afb511b973a905db04401bab9ed6ef686c9`  
		Last Modified: Wed, 14 Jul 2021 01:23:02 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07c9680d47b4272f33a0c462cf6547f8721c0bcf2bf152c26ab458691c43ae0`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 250.4 KB (250422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd21.04-non-free`

```console
$ docker pull neurodebian@sha256:fae34ae4ede0fc837cf0b7e8f27d43d401d3c6846c47e07a3a3a2a7ac567b3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd21.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:967d0f18a999a175f6757bbcac24b304c79fa0ff2edd91604d75c7d648c7c78e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37688353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ec1f95ed830f7eabfa1e441f0bf0b1828ac253b1ef4de221cb0df127aa1e4a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:57 GMT
ADD file:af305d3eb867f312743f97d1cbed14ee2a155fdfed4621c72a8e8cf25355660c in / 
# Tue, 13 Jul 2021 22:29:57 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:20:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 14 Jul 2021 01:20:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian hirsute main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel hirsute main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 14 Jul 2021 01:20:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:20:54 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:966b3c5c8637e41360eed39a59e6c16ee1e986f7f2b92244e4d39f7ca6669618`  
		Last Modified: Tue, 13 Jul 2021 22:31:57 GMT  
		Size: 31.8 MB (31836858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6174bb4728b14be1ee1b3dc8c9856679c536960bf2cdeb5739d9776968641e`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 5.6 MB (5598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11e5a9b959c308ffb520739593aae1d3d73f2795b2b364fc618a749251f7162`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c62c59144a54d5082baddb64ce4afb511b973a905db04401bab9ed6ef686c9`  
		Last Modified: Wed, 14 Jul 2021 01:23:02 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07c9680d47b4272f33a0c462cf6547f8721c0bcf2bf152c26ab458691c43ae0`  
		Last Modified: Wed, 14 Jul 2021 01:23:03 GMT  
		Size: 250.4 KB (250422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea77cc98717c64aef1424fa72704630a0d800ec82634b96ad3fe3d833abfc1cf`  
		Last Modified: Wed, 14 Jul 2021 01:23:16 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd90`

```console
$ docker pull neurodebian@sha256:bd574d6c76263e7aac3a2ae913f7d2d3299fe9546da7908ec9819e7ede27b52e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd90` - linux; amd64

```console
$ docker pull neurodebian@sha256:97e0871503b842e669053e9f99e5793b77aea5203dd2984de0ee03842c1360f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52247126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2fbd5aa4b4cad8ad53e6588de4d5c5917e1a1e1ce67dfca4d88fce3c006a35f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:05 GMT
ADD file:fc9409352ad67880b83ccf1ccd1587eb2666715eae04e4dd98fca919f1bb98d7 in / 
# Thu, 22 Jul 2021 00:47:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:23 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08224db8ce18b31a78a0a26d1b344d173528e50a7067797c9df4de5d8df353e2`  
		Last Modified: Thu, 22 Jul 2021 00:52:52 GMT  
		Size: 45.4 MB (45379781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289adce44c74cd3a9501987ddec1de9c56dbb545616cbfea0b4b2a956ae56e72`  
		Last Modified: Thu, 22 Jul 2021 09:53:47 GMT  
		Size: 6.6 MB (6571690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fde85f89658efa8b979f1de6a0663239b9f4c362692e305ee64910699d9cd8`  
		Last Modified: Thu, 22 Jul 2021 09:53:46 GMT  
		Size: 3.2 KB (3156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4e487d6d5d279e94dd8d7a0f1e4ce1b64782718dfce3b1097823b14cc0938`  
		Last Modified: Thu, 22 Jul 2021 09:53:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9fd062465c63ea7dd9b47b082b1aae8acf40f8986201be095fe539191b7ae5`  
		Last Modified: Thu, 22 Jul 2021 09:53:46 GMT  
		Size: 292.3 KB (292252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd90-non-free`

```console
$ docker pull neurodebian@sha256:0427c0b2c1c96eab6f4dac204a5cac90882dc9c31a43dd948b1fca4696c8f84f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd90-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:fe740e83c05cdb2e59d41691420443e5fc39be63637b5572e087a78bf04cb774
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52247488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0de1e83652d0a43f0f05482f00dcbb0e6ffbdc7275c427ec70094baf6befc938`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:05 GMT
ADD file:fc9409352ad67880b83ccf1ccd1587eb2666715eae04e4dd98fca919f1bb98d7 in / 
# Thu, 22 Jul 2021 00:47:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:23 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:26 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:08224db8ce18b31a78a0a26d1b344d173528e50a7067797c9df4de5d8df353e2`  
		Last Modified: Thu, 22 Jul 2021 00:52:52 GMT  
		Size: 45.4 MB (45379781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289adce44c74cd3a9501987ddec1de9c56dbb545616cbfea0b4b2a956ae56e72`  
		Last Modified: Thu, 22 Jul 2021 09:53:47 GMT  
		Size: 6.6 MB (6571690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fde85f89658efa8b979f1de6a0663239b9f4c362692e305ee64910699d9cd8`  
		Last Modified: Thu, 22 Jul 2021 09:53:46 GMT  
		Size: 3.2 KB (3156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4e487d6d5d279e94dd8d7a0f1e4ce1b64782718dfce3b1097823b14cc0938`  
		Last Modified: Thu, 22 Jul 2021 09:53:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9fd062465c63ea7dd9b47b082b1aae8acf40f8986201be095fe539191b7ae5`  
		Last Modified: Thu, 22 Jul 2021 09:53:46 GMT  
		Size: 292.3 KB (292252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9fb36130a8fab9876e15dea4761044754c3ba091cb0685efed82f701c01bad`  
		Last Modified: Thu, 22 Jul 2021 09:53:58 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:non-free`

```console
$ docker pull neurodebian@sha256:c53593105b6976b3e1b0a7471aeedcd6a1893b585fde59c17ff7ac1456694b01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:0ed1185fa7c3ad9fbcd0fb3f165204cf75508f9a98563c4a5209ea677a6c7902
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61240723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:310ef8d41a0013c86b5d8085e5839affed1cc00e9e8b582738e9908d6564b539`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:45 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff66d7acb9e05c47e0621027afb45a8dfa4665301a45f8f794a16bd8c8ae8205`  
		Last Modified: Thu, 22 Jul 2021 09:54:11 GMT  
		Size: 10.5 MB (10499949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac627f2d764f56d7380099754dd943f54a31247e9400d632a215b8bc4ec5fa2`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33c3e9e07dc85213c696c81aff06d286ba379571b799845954b6cc776457e5f`  
		Last Modified: Thu, 22 Jul 2021 09:54:09 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c4b1dfc179a7cb39a5bcbff0f4d529c84d1fab9395e799ab8a0350c620e58`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 302.8 KB (302773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a42860b1360435ab5bdf409f82263bf9f069a75f834afae3bcaedd3255b6ae6`  
		Last Modified: Thu, 22 Jul 2021 09:54:26 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:d2c65918ec2833688a37fe5a66aee4a458b46749b46c3a5a2011552b76da3fa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:sid` - linux; amd64

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

## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:2ee65aa92aad3610cc167554c656d5dbe94b063975c5c8aa7d74033e3d34b2e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:082ca4751fb886450170ef204a85b03b2f99fe2dc807f85763ffb3aa955b1455
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66532325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce77c88e1b97352a7d6577b575a7320dafb73d776f427a62f6d81a0e9bd52e6c`
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
# Thu, 22 Jul 2021 09:52:30 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
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
	-	`sha256:0974a17fac1ea186c3ba9c50cf8ef1e640af0298dfb84c2e683cc1571d20bc71`  
		Last Modified: Thu, 22 Jul 2021 09:55:14 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:stretch`

```console
$ docker pull neurodebian@sha256:bd574d6c76263e7aac3a2ae913f7d2d3299fe9546da7908ec9819e7ede27b52e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:stretch` - linux; amd64

```console
$ docker pull neurodebian@sha256:97e0871503b842e669053e9f99e5793b77aea5203dd2984de0ee03842c1360f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52247126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2fbd5aa4b4cad8ad53e6588de4d5c5917e1a1e1ce67dfca4d88fce3c006a35f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:05 GMT
ADD file:fc9409352ad67880b83ccf1ccd1587eb2666715eae04e4dd98fca919f1bb98d7 in / 
# Thu, 22 Jul 2021 00:47:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:23 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08224db8ce18b31a78a0a26d1b344d173528e50a7067797c9df4de5d8df353e2`  
		Last Modified: Thu, 22 Jul 2021 00:52:52 GMT  
		Size: 45.4 MB (45379781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289adce44c74cd3a9501987ddec1de9c56dbb545616cbfea0b4b2a956ae56e72`  
		Last Modified: Thu, 22 Jul 2021 09:53:47 GMT  
		Size: 6.6 MB (6571690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fde85f89658efa8b979f1de6a0663239b9f4c362692e305ee64910699d9cd8`  
		Last Modified: Thu, 22 Jul 2021 09:53:46 GMT  
		Size: 3.2 KB (3156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4e487d6d5d279e94dd8d7a0f1e4ce1b64782718dfce3b1097823b14cc0938`  
		Last Modified: Thu, 22 Jul 2021 09:53:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9fd062465c63ea7dd9b47b082b1aae8acf40f8986201be095fe539191b7ae5`  
		Last Modified: Thu, 22 Jul 2021 09:53:46 GMT  
		Size: 292.3 KB (292252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:stretch-non-free`

```console
$ docker pull neurodebian@sha256:0427c0b2c1c96eab6f4dac204a5cac90882dc9c31a43dd948b1fca4696c8f84f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:stretch-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:fe740e83c05cdb2e59d41691420443e5fc39be63637b5572e087a78bf04cb774
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52247488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0de1e83652d0a43f0f05482f00dcbb0e6ffbdc7275c427ec70094baf6befc938`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:05 GMT
ADD file:fc9409352ad67880b83ccf1ccd1587eb2666715eae04e4dd98fca919f1bb98d7 in / 
# Thu, 22 Jul 2021 00:47:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:23 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:26 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:08224db8ce18b31a78a0a26d1b344d173528e50a7067797c9df4de5d8df353e2`  
		Last Modified: Thu, 22 Jul 2021 00:52:52 GMT  
		Size: 45.4 MB (45379781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289adce44c74cd3a9501987ddec1de9c56dbb545616cbfea0b4b2a956ae56e72`  
		Last Modified: Thu, 22 Jul 2021 09:53:47 GMT  
		Size: 6.6 MB (6571690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fde85f89658efa8b979f1de6a0663239b9f4c362692e305ee64910699d9cd8`  
		Last Modified: Thu, 22 Jul 2021 09:53:46 GMT  
		Size: 3.2 KB (3156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4e487d6d5d279e94dd8d7a0f1e4ce1b64782718dfce3b1097823b14cc0938`  
		Last Modified: Thu, 22 Jul 2021 09:53:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9fd062465c63ea7dd9b47b082b1aae8acf40f8986201be095fe539191b7ae5`  
		Last Modified: Thu, 22 Jul 2021 09:53:46 GMT  
		Size: 292.3 KB (292252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9fb36130a8fab9876e15dea4761044754c3ba091cb0685efed82f701c01bad`  
		Last Modified: Thu, 22 Jul 2021 09:53:58 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:xenial`

```console
$ docker pull neurodebian@sha256:706422ad8751b16d4421f5c37474d10da64d708f89d0d19eae16587c32b2a0b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:xenial` - linux; amd64

```console
$ docker pull neurodebian@sha256:4471dff78eb2b61d7c0fe05c386984cee1ecffe25994d149995dd32d4c77900f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46728844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81ebe285f4f396273f6e8f2b6ef3ef3f9e05f6fa87a6d16ffb9e12ce02da140`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 04:51:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:51:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 18 Jun 2021 04:51:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 18 Jun 2021 04:51:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27db3f87344ee4f403c5257877584f0b0319c19914fa2953e351715240aa547`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d325b9a44fc4bfd2ef838143c6afeeed1fbf4929cc69351b13790404151baf`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 3.1 KB (3150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a309011e84c623c2b39ed13ff0f62d5c0f40e9ae798cdf37fba510c34711c6`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea488f510caf428861b3edf4b32605992b348a0f4ec00ee2e81a581d8e80f80`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 226.9 KB (226939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:xenial-non-free`

```console
$ docker pull neurodebian@sha256:937cdaf8ad5054fd931a11a6bb0a8b4c0840a0a115540e98879ea449f69e1dbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:xenial-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:0041163886c00bd41f9d9eaf5748fbc5b2e178e4d191beb751fb7e2659256870
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:816d85192005dbf8618fa9b54d5b0ae148f0cf0104fb9268b604dad9648aa060`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 04:51:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:51:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 18 Jun 2021 04:51:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 18 Jun 2021 04:51:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:51:57 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27db3f87344ee4f403c5257877584f0b0319c19914fa2953e351715240aa547`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d325b9a44fc4bfd2ef838143c6afeeed1fbf4929cc69351b13790404151baf`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 3.1 KB (3150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a309011e84c623c2b39ed13ff0f62d5c0f40e9ae798cdf37fba510c34711c6`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea488f510caf428861b3edf4b32605992b348a0f4ec00ee2e81a581d8e80f80`  
		Last Modified: Fri, 18 Jun 2021 04:54:39 GMT  
		Size: 226.9 KB (226939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901921b5a6b1c35d7c4d2819f403cac6c89c2165b3d2c26ed9a7741007b3aae`  
		Last Modified: Fri, 18 Jun 2021 04:54:51 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
