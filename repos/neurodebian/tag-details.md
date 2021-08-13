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
$ docker pull neurodebian@sha256:40592492b9cae174140033219405eccf96213f0a66ea8747b12a463622edc8dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:451d9dafb1761cdf796aaa3f9bd0d6d18783769193b9c3b762e794486c4d07ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31765376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:714338cfdd48d5d70e55de7cd452321932c3a1cbf7ed5b9dfa712720c07eb328`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:13:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:13:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e938ab6c3a5cf1c29298043d3d5c68195eec69585541aa9a6bb749be67881c51`  
		Last Modified: Tue, 27 Jul 2021 00:17:12 GMT  
		Size: 4.8 MB (4813118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7870bda0883ce8d4f86ede7a7881a3366d112673fe11cc38223ef4510228bf53`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 3.2 KB (3154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9662eb146b3a44cd5c3251fd7622e852c35e6c4b810c3685b04f29d89a9bd731`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2653b42c5af817f901660031c386465e53297b18053e5d8a6a62280b13a4f5d2`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 239.8 KB (239821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bionic-non-free`

```console
$ docker pull neurodebian@sha256:799ea3936e5f9184b1d8828590ac89c4dbdbe23719d234046e9f69b30415877d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bionic-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:293f8209bf213ba2b9ce8fd4c487adad9b6af8c0a26b1dc871f766d08d029fed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31765632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa69c51ac01c99497165137e1317c5447591d002600924d32828605f04224f44`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:13:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:13:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:43 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e938ab6c3a5cf1c29298043d3d5c68195eec69585541aa9a6bb749be67881c51`  
		Last Modified: Tue, 27 Jul 2021 00:17:12 GMT  
		Size: 4.8 MB (4813118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7870bda0883ce8d4f86ede7a7881a3366d112673fe11cc38223ef4510228bf53`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 3.2 KB (3154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9662eb146b3a44cd5c3251fd7622e852c35e6c4b810c3685b04f29d89a9bd731`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2653b42c5af817f901660031c386465e53297b18053e5d8a6a62280b13a4f5d2`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 239.8 KB (239821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0e41b964cb330ae3f324759621ac01ea88e9e576bad4e242ad8d109a91ff71`  
		Last Modified: Tue, 27 Jul 2021 00:17:24 GMT  
		Size: 256.0 B  
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
$ docker pull neurodebian@sha256:dfe56cdfbaba469a68a34265558fe3653d29ce4bf4f8873582b2284631cb9401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:d4c6391daea504d855fe42504ebfc6d07f1653badc4724040f50a8b75744d114
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34296820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f97ff2718a58ec8de130e3d73fba84de56aa226494ae818cf58063dd9e33b5a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:13:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:14:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870d1e2acc9261e5c3a40b500f5959e6394d09583b3467f279e6b40fa9ed0faa`  
		Last Modified: Tue, 27 Jul 2021 00:17:36 GMT  
		Size: 5.5 MB (5488799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f682b7475d2896a202cbcefb58ae71d2bf958761ac8068be9ae2f58c0a012bb6`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5c473424a3f78f98ed3c2f554c0d343e02cb12efc7f6d2e1b591f43756d58f`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f546e25b59926a75cc53a386fc97e72f3893848614566fda6e2fa026b7dd1`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 238.1 KB (238065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal-non-free`

```console
$ docker pull neurodebian@sha256:51e50f2fef713c938fd8f0e9b621f18446b5ee9fb9d2d6140a61a8d6f2054e07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:focal-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:08c3a5fbff55830503f374ff412b3aecba1f0d3923b11cbd00c6d307885ac878
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34297075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9818eb64c7a6c42e291d4257c8c876f5ec06c640580ae2167c2696a0f268a1e0`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:13:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:14:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:14:05 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870d1e2acc9261e5c3a40b500f5959e6394d09583b3467f279e6b40fa9ed0faa`  
		Last Modified: Tue, 27 Jul 2021 00:17:36 GMT  
		Size: 5.5 MB (5488799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f682b7475d2896a202cbcefb58ae71d2bf958761ac8068be9ae2f58c0a012bb6`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5c473424a3f78f98ed3c2f554c0d343e02cb12efc7f6d2e1b591f43756d58f`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f546e25b59926a75cc53a386fc97e72f3893848614566fda6e2fa026b7dd1`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 238.1 KB (238065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5b9bcdfe52b5bc32583670eccca7273dc04e6ed5fe25571d3d3843785ce7e2`  
		Last Modified: Tue, 27 Jul 2021 00:17:46 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:hirsute`

```console
$ docker pull neurodebian@sha256:7385a5023129b01a4b02ed9229e193d33810441449993c9f0f82d258cd47143b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:hirsute` - linux; amd64

```console
$ docker pull neurodebian@sha256:bff1efcd9743c627506e21e0d1dc5f455ff4963b1c5168a812ec623c3cb9d3dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37686774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c59636c0452ae01455d116c48f4ac2ebfc4e6058b46a920090363ca3d157695f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:15:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:15:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:15:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian hirsute main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel hirsute main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:15:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56df5ecf752059653014e714bae6507778c2fd9f6c3f864fdeb0f11be5318b`  
		Last Modified: Tue, 27 Jul 2021 00:18:24 GMT  
		Size: 5.6 MB (5597737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d996b67eeee2532d9643e28004d43fba9c80c19ac98f2b5378cc7fd200041`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35723c871426551f5e5c91aa3caf285e3fbdd3819e9baba7432cc48fa90afc25`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df43dcede292226ffbef4971d7b79425f61a336e7bf892f24f89f0cde937e57`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 249.5 KB (249455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:hirsute-non-free`

```console
$ docker pull neurodebian@sha256:dc1891c2764c95560eb7a56f32d5422ce7067031afe7915a82db5233d60bfe40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:hirsute-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:a255713afcc6cc708ac499c0b89e5bd2d9623c2d5f38b83c8964a323ea4b0030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37687033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9445c97ade590117897e42cddf4822b60f20bd87239e97e4bbd859e27dc8608e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:15:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:15:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:15:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian hirsute main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel hirsute main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:15:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:15:45 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56df5ecf752059653014e714bae6507778c2fd9f6c3f864fdeb0f11be5318b`  
		Last Modified: Tue, 27 Jul 2021 00:18:24 GMT  
		Size: 5.6 MB (5597737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d996b67eeee2532d9643e28004d43fba9c80c19ac98f2b5378cc7fd200041`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35723c871426551f5e5c91aa3caf285e3fbdd3819e9baba7432cc48fa90afc25`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df43dcede292226ffbef4971d7b79425f61a336e7bf892f24f89f0cde937e57`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 249.5 KB (249455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dafb5cb912e6be0079cd434fc4fb0c83d60571d2b29cca69b8bb32cfb2babb3`  
		Last Modified: Tue, 27 Jul 2021 00:18:34 GMT  
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
$ docker pull neurodebian@sha256:43b573d833942d586f9a7d4a1c3f1ca209077a20b2a90c26cb02b0fa61b03156
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd16.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:3160d9542153b47caf8d069cbc0db22d1638ad4adbd353f1259c21355f99b6ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00f1bda86cb8ade0c529bcb17fda696383d42d0188167b4119599fb18acdbab3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 00:13:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:13:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7416d41f03136eeac7efb16c3fd8a6589880fff5bda819b3a1e6066c41fef7`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bd79c96d093dd72ba4bbd9c6352b1fb0f299189cdc0d6388c894f24eec8714`  
		Last Modified: Tue, 27 Jul 2021 00:16:48 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb360a6236175933715f7da41d199cb387954378bed350ccbcccc94565dfefe`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bfb7b9c9a2ce4ec8233a80b6131f224640f54ca2b6af5dcde3f11b71f315d4`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 227.2 KB (227170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd16.04-non-free`

```console
$ docker pull neurodebian@sha256:822e4ac31d3f0aadb858981a3ee4ece7f5d77edb5fb8f6b81efb166e3be2699a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd16.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:62ea27a9925c741937b8763cdb75ecd8c3dfbca34503701c7eb16b37f277c439
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21bb46914f12361be318974e8b6196f2a48122d7c2eaa4d987cd4c9f60d09626`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 00:13:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:13:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:19 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7416d41f03136eeac7efb16c3fd8a6589880fff5bda819b3a1e6066c41fef7`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bd79c96d093dd72ba4bbd9c6352b1fb0f299189cdc0d6388c894f24eec8714`  
		Last Modified: Tue, 27 Jul 2021 00:16:48 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb360a6236175933715f7da41d199cb387954378bed350ccbcccc94565dfefe`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bfb7b9c9a2ce4ec8233a80b6131f224640f54ca2b6af5dcde3f11b71f315d4`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 227.2 KB (227170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787a536fe6fc734fba11687bdfb5bf9d581534aadb3907eb628b70239dff16e4`  
		Last Modified: Tue, 27 Jul 2021 00:17:00 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04`

```console
$ docker pull neurodebian@sha256:40592492b9cae174140033219405eccf96213f0a66ea8747b12a463622edc8dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd18.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:451d9dafb1761cdf796aaa3f9bd0d6d18783769193b9c3b762e794486c4d07ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31765376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:714338cfdd48d5d70e55de7cd452321932c3a1cbf7ed5b9dfa712720c07eb328`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:13:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:13:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e938ab6c3a5cf1c29298043d3d5c68195eec69585541aa9a6bb749be67881c51`  
		Last Modified: Tue, 27 Jul 2021 00:17:12 GMT  
		Size: 4.8 MB (4813118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7870bda0883ce8d4f86ede7a7881a3366d112673fe11cc38223ef4510228bf53`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 3.2 KB (3154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9662eb146b3a44cd5c3251fd7622e852c35e6c4b810c3685b04f29d89a9bd731`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2653b42c5af817f901660031c386465e53297b18053e5d8a6a62280b13a4f5d2`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 239.8 KB (239821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04-non-free`

```console
$ docker pull neurodebian@sha256:799ea3936e5f9184b1d8828590ac89c4dbdbe23719d234046e9f69b30415877d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd18.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:293f8209bf213ba2b9ce8fd4c487adad9b6af8c0a26b1dc871f766d08d029fed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31765632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa69c51ac01c99497165137e1317c5447591d002600924d32828605f04224f44`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:13:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:13:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:43 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e938ab6c3a5cf1c29298043d3d5c68195eec69585541aa9a6bb749be67881c51`  
		Last Modified: Tue, 27 Jul 2021 00:17:12 GMT  
		Size: 4.8 MB (4813118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7870bda0883ce8d4f86ede7a7881a3366d112673fe11cc38223ef4510228bf53`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 3.2 KB (3154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9662eb146b3a44cd5c3251fd7622e852c35e6c4b810c3685b04f29d89a9bd731`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2653b42c5af817f901660031c386465e53297b18053e5d8a6a62280b13a4f5d2`  
		Last Modified: Tue, 27 Jul 2021 00:17:11 GMT  
		Size: 239.8 KB (239821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0e41b964cb330ae3f324759621ac01ea88e9e576bad4e242ad8d109a91ff71`  
		Last Modified: Tue, 27 Jul 2021 00:17:24 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04`

```console
$ docker pull neurodebian@sha256:dfe56cdfbaba469a68a34265558fe3653d29ce4bf4f8873582b2284631cb9401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd20.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:d4c6391daea504d855fe42504ebfc6d07f1653badc4724040f50a8b75744d114
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34296820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f97ff2718a58ec8de130e3d73fba84de56aa226494ae818cf58063dd9e33b5a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:13:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:14:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870d1e2acc9261e5c3a40b500f5959e6394d09583b3467f279e6b40fa9ed0faa`  
		Last Modified: Tue, 27 Jul 2021 00:17:36 GMT  
		Size: 5.5 MB (5488799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f682b7475d2896a202cbcefb58ae71d2bf958761ac8068be9ae2f58c0a012bb6`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5c473424a3f78f98ed3c2f554c0d343e02cb12efc7f6d2e1b591f43756d58f`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f546e25b59926a75cc53a386fc97e72f3893848614566fda6e2fa026b7dd1`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 238.1 KB (238065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04-non-free`

```console
$ docker pull neurodebian@sha256:51e50f2fef713c938fd8f0e9b621f18446b5ee9fb9d2d6140a61a8d6f2054e07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd20.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:08c3a5fbff55830503f374ff412b3aecba1f0d3923b11cbd00c6d307885ac878
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34297075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9818eb64c7a6c42e291d4257c8c876f5ec06c640580ae2167c2696a0f268a1e0`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:13:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:14:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:14:05 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870d1e2acc9261e5c3a40b500f5959e6394d09583b3467f279e6b40fa9ed0faa`  
		Last Modified: Tue, 27 Jul 2021 00:17:36 GMT  
		Size: 5.5 MB (5488799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f682b7475d2896a202cbcefb58ae71d2bf958761ac8068be9ae2f58c0a012bb6`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5c473424a3f78f98ed3c2f554c0d343e02cb12efc7f6d2e1b591f43756d58f`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f546e25b59926a75cc53a386fc97e72f3893848614566fda6e2fa026b7dd1`  
		Last Modified: Tue, 27 Jul 2021 00:17:34 GMT  
		Size: 238.1 KB (238065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5b9bcdfe52b5bc32583670eccca7273dc04e6ed5fe25571d3d3843785ce7e2`  
		Last Modified: Tue, 27 Jul 2021 00:17:46 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd21.04`

```console
$ docker pull neurodebian@sha256:7385a5023129b01a4b02ed9229e193d33810441449993c9f0f82d258cd47143b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd21.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:bff1efcd9743c627506e21e0d1dc5f455ff4963b1c5168a812ec623c3cb9d3dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37686774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c59636c0452ae01455d116c48f4ac2ebfc4e6058b46a920090363ca3d157695f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:15:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:15:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:15:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian hirsute main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel hirsute main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:15:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56df5ecf752059653014e714bae6507778c2fd9f6c3f864fdeb0f11be5318b`  
		Last Modified: Tue, 27 Jul 2021 00:18:24 GMT  
		Size: 5.6 MB (5597737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d996b67eeee2532d9643e28004d43fba9c80c19ac98f2b5378cc7fd200041`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35723c871426551f5e5c91aa3caf285e3fbdd3819e9baba7432cc48fa90afc25`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df43dcede292226ffbef4971d7b79425f61a336e7bf892f24f89f0cde937e57`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 249.5 KB (249455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd21.04-non-free`

```console
$ docker pull neurodebian@sha256:dc1891c2764c95560eb7a56f32d5422ce7067031afe7915a82db5233d60bfe40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd21.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:a255713afcc6cc708ac499c0b89e5bd2d9623c2d5f38b83c8964a323ea4b0030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37687033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9445c97ade590117897e42cddf4822b60f20bd87239e97e4bbd859e27dc8608e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:15:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:15:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:15:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian hirsute main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel hirsute main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:15:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:15:45 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56df5ecf752059653014e714bae6507778c2fd9f6c3f864fdeb0f11be5318b`  
		Last Modified: Tue, 27 Jul 2021 00:18:24 GMT  
		Size: 5.6 MB (5597737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d996b67eeee2532d9643e28004d43fba9c80c19ac98f2b5378cc7fd200041`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35723c871426551f5e5c91aa3caf285e3fbdd3819e9baba7432cc48fa90afc25`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df43dcede292226ffbef4971d7b79425f61a336e7bf892f24f89f0cde937e57`  
		Last Modified: Tue, 27 Jul 2021 00:18:23 GMT  
		Size: 249.5 KB (249455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dafb5cb912e6be0079cd434fc4fb0c83d60571d2b29cca69b8bb32cfb2babb3`  
		Last Modified: Tue, 27 Jul 2021 00:18:34 GMT  
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
$ docker pull neurodebian@sha256:43b573d833942d586f9a7d4a1c3f1ca209077a20b2a90c26cb02b0fa61b03156
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:xenial` - linux; amd64

```console
$ docker pull neurodebian@sha256:3160d9542153b47caf8d069cbc0db22d1638ad4adbd353f1259c21355f99b6ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00f1bda86cb8ade0c529bcb17fda696383d42d0188167b4119599fb18acdbab3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 00:13:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:13:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7416d41f03136eeac7efb16c3fd8a6589880fff5bda819b3a1e6066c41fef7`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bd79c96d093dd72ba4bbd9c6352b1fb0f299189cdc0d6388c894f24eec8714`  
		Last Modified: Tue, 27 Jul 2021 00:16:48 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb360a6236175933715f7da41d199cb387954378bed350ccbcccc94565dfefe`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bfb7b9c9a2ce4ec8233a80b6131f224640f54ca2b6af5dcde3f11b71f315d4`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 227.2 KB (227170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:xenial-non-free`

```console
$ docker pull neurodebian@sha256:822e4ac31d3f0aadb858981a3ee4ece7f5d77edb5fb8f6b81efb166e3be2699a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:xenial-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:62ea27a9925c741937b8763cdb75ecd8c3dfbca34503701c7eb16b37f277c439
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21bb46914f12361be318974e8b6196f2a48122d7c2eaa4d987cd4c9f60d09626`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 00:13:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 27 Jul 2021 00:13:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 27 Jul 2021 00:13:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:13:19 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7416d41f03136eeac7efb16c3fd8a6589880fff5bda819b3a1e6066c41fef7`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bd79c96d093dd72ba4bbd9c6352b1fb0f299189cdc0d6388c894f24eec8714`  
		Last Modified: Tue, 27 Jul 2021 00:16:48 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb360a6236175933715f7da41d199cb387954378bed350ccbcccc94565dfefe`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bfb7b9c9a2ce4ec8233a80b6131f224640f54ca2b6af5dcde3f11b71f315d4`  
		Last Modified: Tue, 27 Jul 2021 00:16:47 GMT  
		Size: 227.2 KB (227170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787a536fe6fc734fba11687bdfb5bf9d581534aadb3907eb628b70239dff16e4`  
		Last Modified: Tue, 27 Jul 2021 00:17:00 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
