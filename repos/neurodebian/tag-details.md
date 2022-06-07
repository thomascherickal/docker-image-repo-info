<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neurodebian`

-	[`neurodebian:bionic`](#neurodebianbionic)
-	[`neurodebian:bionic-non-free`](#neurodebianbionic-non-free)
-	[`neurodebian:bookworm`](#neurodebianbookworm)
-	[`neurodebian:bookworm-non-free`](#neurodebianbookworm-non-free)
-	[`neurodebian:bullseye`](#neurodebianbullseye)
-	[`neurodebian:bullseye-non-free`](#neurodebianbullseye-non-free)
-	[`neurodebian:buster`](#neurodebianbuster)
-	[`neurodebian:buster-non-free`](#neurodebianbuster-non-free)
-	[`neurodebian:focal`](#neurodebianfocal)
-	[`neurodebian:focal-non-free`](#neurodebianfocal-non-free)
-	[`neurodebian:impish`](#neurodebianimpish)
-	[`neurodebian:impish-non-free`](#neurodebianimpish-non-free)
-	[`neurodebian:latest`](#neurodebianlatest)
-	[`neurodebian:nd`](#neurodebiannd)
-	[`neurodebian:nd-non-free`](#neurodebiannd-non-free)
-	[`neurodebian:nd100`](#neurodebiannd100)
-	[`neurodebian:nd100-non-free`](#neurodebiannd100-non-free)
-	[`neurodebian:nd110`](#neurodebiannd110)
-	[`neurodebian:nd110-non-free`](#neurodebiannd110-non-free)
-	[`neurodebian:nd120`](#neurodebiannd120)
-	[`neurodebian:nd120-non-free`](#neurodebiannd120-non-free)
-	[`neurodebian:nd16.04`](#neurodebiannd1604)
-	[`neurodebian:nd16.04-non-free`](#neurodebiannd1604-non-free)
-	[`neurodebian:nd18.04`](#neurodebiannd1804)
-	[`neurodebian:nd18.04-non-free`](#neurodebiannd1804-non-free)
-	[`neurodebian:nd20.04`](#neurodebiannd2004)
-	[`neurodebian:nd20.04-non-free`](#neurodebiannd2004-non-free)
-	[`neurodebian:nd21.10`](#neurodebiannd2110)
-	[`neurodebian:nd21.10-non-free`](#neurodebiannd2110-non-free)
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
$ docker pull neurodebian@sha256:24dbb94d281291cb1e04b6108e5eaca921dfee07b976021bf1dccd7d516833b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:375123cc33c1c024fb8429f011c99b58c87203c5a4a936adfaa84064dee99f3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31771462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3bbfb1b8f311ec84d7ab789e1111bcaf2f73b4ff6fb1611454c72a12352a8a4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:37:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:37:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:37:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2b3981bc62720e6e1f9f8b6fd2d4af6b8dc0d5d1d930cad27b75a30d93221`  
		Last Modified: Tue, 07 Jun 2022 00:39:28 GMT  
		Size: 4.8 MB (4817739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff80362b7a8a66dc0750954a4c03f08846b9241ac54372ec5bae9d12540d468`  
		Last Modified: Tue, 07 Jun 2022 00:39:27 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d453cada745b8af1182eb78a54478ae0375ac8f0b4b908d273b10429bcd7ec81`  
		Last Modified: Tue, 07 Jun 2022 00:39:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f79b6a697fd3011ea990d9d8ef464697221eacc2d053352e61632bcb16d3c3`  
		Last Modified: Tue, 07 Jun 2022 00:39:27 GMT  
		Size: 240.2 KB (240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bionic-non-free`

```console
$ docker pull neurodebian@sha256:d9f97ebb267aa7ecef9b61d57a119f4c1938d73201aa1a0915b356ac6c74858d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bionic-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:52db60494f9b1f9ed71c583e724777aea45be1f56982bbdbb06faae6efbb384e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31771718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2d6fea5ab69bb8a2c661a8b8ccb7226fbd7c8b58f1e12a5cff9753a8d035ed2`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:37:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:37:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:37:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:25 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2b3981bc62720e6e1f9f8b6fd2d4af6b8dc0d5d1d930cad27b75a30d93221`  
		Last Modified: Tue, 07 Jun 2022 00:39:28 GMT  
		Size: 4.8 MB (4817739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff80362b7a8a66dc0750954a4c03f08846b9241ac54372ec5bae9d12540d468`  
		Last Modified: Tue, 07 Jun 2022 00:39:27 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d453cada745b8af1182eb78a54478ae0375ac8f0b4b908d273b10429bcd7ec81`  
		Last Modified: Tue, 07 Jun 2022 00:39:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f79b6a697fd3011ea990d9d8ef464697221eacc2d053352e61632bcb16d3c3`  
		Last Modified: Tue, 07 Jun 2022 00:39:27 GMT  
		Size: 240.2 KB (240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326546dbbe4e98516ffed1b2576dbaaa1a592e2c5f4e103da5d95ffe6b418ef1`  
		Last Modified: Tue, 07 Jun 2022 00:39:37 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm`

```console
$ docker pull neurodebian@sha256:78c9f3eccfaafb9fb4dd2a9dca8820b44d93473e5c6f0498f2190e9e946a68c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bookworm` - linux; amd64

```console
$ docker pull neurodebian@sha256:068faa6f7448a0d180c996d5535104e837626f54186aeaf014d75dcca8a26d58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64881666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bebcce458d791df05d664cf985b5b3b9b402a6a3d51a53b85df9b114e47e838c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:19:50 GMT
ADD file:05d40d360d088a73d2d9ea8361742b3b0e7f5ac80923374f84acf3d1be6c7798 in / 
# Sat, 28 May 2022 01:19:52 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:36 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:40 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1afe78e67a22dc5c619d5518a1d45e8f5ca31628fa6b7caa3b645c4fba19faaa`  
		Last Modified: Sat, 28 May 2022 01:24:12 GMT  
		Size: 52.9 MB (52947713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d562bd670035564f61d24341f5130b01d36042c36107e0a987fb466eb6d6ffb8`  
		Last Modified: Sat, 28 May 2022 05:39:54 GMT  
		Size: 11.6 MB (11640504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7050b6924f15d3e72dbb1096546f83c63ecdbbca6186c8f851a03625a1f32674`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bda5105d9eff32d11d816fd1398dce31832adc9410be0638a2acea9cbe9b7b`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f537aae945d8347c844b8fb05e793d4a82d4539f9582be5aee2b0eecdc4db8e5`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 291.4 KB (291437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm-non-free`

```console
$ docker pull neurodebian@sha256:3bb5cb32011cd186cd2fe4ef5ab98d32eaee384e75cd3bd68dbe1c92132893e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bookworm-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:ae48c9830c46b712195cfb1f7b88a2decbe44bdc56d140d415df9b1e2b7c2d6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64882033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d04a564923a36175ecb0b612039ac656fe8b127f4e837dc08c9acd6e4141f84d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:19:50 GMT
ADD file:05d40d360d088a73d2d9ea8361742b3b0e7f5ac80923374f84acf3d1be6c7798 in / 
# Sat, 28 May 2022 01:19:52 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:36 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:40 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:44 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:1afe78e67a22dc5c619d5518a1d45e8f5ca31628fa6b7caa3b645c4fba19faaa`  
		Last Modified: Sat, 28 May 2022 01:24:12 GMT  
		Size: 52.9 MB (52947713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d562bd670035564f61d24341f5130b01d36042c36107e0a987fb466eb6d6ffb8`  
		Last Modified: Sat, 28 May 2022 05:39:54 GMT  
		Size: 11.6 MB (11640504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7050b6924f15d3e72dbb1096546f83c63ecdbbca6186c8f851a03625a1f32674`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bda5105d9eff32d11d816fd1398dce31832adc9410be0638a2acea9cbe9b7b`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f537aae945d8347c844b8fb05e793d4a82d4539f9582be5aee2b0eecdc4db8e5`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 291.4 KB (291437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfbc4116d9376d185dae07ff9b45bf648c9f12cd31942524fc08991a21d25a5`  
		Last Modified: Sat, 28 May 2022 05:40:07 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:c594c3ef72db3990d13d53cf2a014328b50460cad2bc9ba20c28d52a7f2bb606
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:f9c473661ee2f6c1b9af6d80cfe37980d51be56b56728e4c85a3b4b74dae0714
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66632946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ff7873e504d0b4ffc2d821b9d777f9dad9f593f3431dd0bde40441e4ed03e2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:12 GMT
ADD file:dd3d4b31d7f1d4062ad0eb2d85dba064cea067b1eb4a8b89a0b593ea90001cdf in / 
# Sat, 28 May 2022 01:20:12 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e756f3fdd6a378aa16205b0f75d178b7532b110e86be7659004fc6a21183226c`  
		Last Modified: Sat, 28 May 2022 01:24:51 GMT  
		Size: 55.0 MB (55009253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042d25d72a7dea1cac3b0025ffda5a744367e349b4b8af91ee511c0987d31e8`  
		Last Modified: Sat, 28 May 2022 05:39:30 GMT  
		Size: 11.3 MB (11310360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f8ddb2c45cc88bdf5de437bff502c544b8c489d28b4928b5f58b8432440f24`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d815e97d100e1c9e458bc54972d5fde92a3239754eb453077fc38dbc42e6b9`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e5783c05be991fe571e19a5fe838b22f8120fab5f86db0a60b24721fcad9da`  
		Last Modified: Sat, 28 May 2022 05:39:29 GMT  
		Size: 311.3 KB (311322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:7f5da94d65103f01e54681100cb3d38bdb2642cd40749f1b7bb39111688e0aa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:e79b980580bba0fb6032a8d7dd07d2dfe9d8f55a1ead5e2d622fcea7bf783e31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66633311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16391b661151b02a3078f451d2e12b290e9d5d8fe88cac6809419c9752790d5b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:12 GMT
ADD file:dd3d4b31d7f1d4062ad0eb2d85dba064cea067b1eb4a8b89a0b593ea90001cdf in / 
# Sat, 28 May 2022 01:20:12 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:25 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:e756f3fdd6a378aa16205b0f75d178b7532b110e86be7659004fc6a21183226c`  
		Last Modified: Sat, 28 May 2022 01:24:51 GMT  
		Size: 55.0 MB (55009253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042d25d72a7dea1cac3b0025ffda5a744367e349b4b8af91ee511c0987d31e8`  
		Last Modified: Sat, 28 May 2022 05:39:30 GMT  
		Size: 11.3 MB (11310360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f8ddb2c45cc88bdf5de437bff502c544b8c489d28b4928b5f58b8432440f24`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d815e97d100e1c9e458bc54972d5fde92a3239754eb453077fc38dbc42e6b9`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e5783c05be991fe571e19a5fe838b22f8120fab5f86db0a60b24721fcad9da`  
		Last Modified: Sat, 28 May 2022 05:39:29 GMT  
		Size: 311.3 KB (311322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07471eb1d1598973692a746f2cc5cac14a11e55b43f93822a12a117ecbb8572a`  
		Last Modified: Sat, 28 May 2022 05:39:41 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:b9cbc75b38dca65aefd999e8c0e591ed965f95db49d8f03688c8eeedb689bb9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:59c8f1bd0b8c2bc34454fdffb814b231fceeac95b2e7f133c3b326fbb08f1651
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61245500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b64a0beed441d3db2a683632858a879fe7ad1df1244094e2cd4cdcde7153b6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:36:58 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:36:59 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:00 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:04 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b408b972c76f457b5928d48a45e6c6669ce35818a0c203b012c6966b8d654289`  
		Last Modified: Sat, 28 May 2022 05:39:10 GMT  
		Size: 10.5 MB (10500296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f476d1ba5bb41283ab8a2ef5d7968db4f7e10aab5242fbb3f8381dab67b636`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a556d3bcd634466f553097ef3d03a9bd26dc13edafe9511d4254a1fc257c45e1`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b5e5f807a99c180c7ceadd62cd0a13b22b4f9edae5661acf56bc40c9e9b169`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 302.8 KB (302771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:34bd541da284138fed75724766e0d5e3cac218103ccab5d712db0e8002858d41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:b6f2c3e37f8532066293ccd087ca1f2511ae131f78439be9a9d3ab8dc26991f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61245865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d9e8dac7e90dcb98355f93be5c3ac21e3621c86c21152b1ecfdc8ea81e94a4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:36:58 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:36:59 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:00 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:04 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:08 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b408b972c76f457b5928d48a45e6c6669ce35818a0c203b012c6966b8d654289`  
		Last Modified: Sat, 28 May 2022 05:39:10 GMT  
		Size: 10.5 MB (10500296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f476d1ba5bb41283ab8a2ef5d7968db4f7e10aab5242fbb3f8381dab67b636`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a556d3bcd634466f553097ef3d03a9bd26dc13edafe9511d4254a1fc257c45e1`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b5e5f807a99c180c7ceadd62cd0a13b22b4f9edae5661acf56bc40c9e9b169`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 302.8 KB (302771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca022902e8dca86c10ed36509f07e5cb9ccafaacbf0687a47d858b5f7e344c66`  
		Last Modified: Sat, 28 May 2022 05:39:19 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal`

```console
$ docker pull neurodebian@sha256:910dff6bf17ef9c6ecdc30982ee18bd4d09fb2c1f740e53348afde41e021eaf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:39f2154d2cdb8d241fe22e1aa8d7646d29503aa842ac35aad54d97266de1598b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db6a99a7f13a251621d206e8da7fe6bab43d65ea0af1fc7a69a8d49754a79959`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:37:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:37:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:37:42 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0d85648c57095c325776ef894c7e76c557caf12f9bcb61f510da5c30f4f660`  
		Last Modified: Tue, 07 Jun 2022 00:39:47 GMT  
		Size: 5.5 MB (5489017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b42d0b055eb8b4dabb68755df18c0921420d071b554c246ac4ec6068416583`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be77e820178f2d7d401e7cb28b70f9a90763d3bd2626132c372fec5ccbacc805`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885284a345938a81195044fcfc0624d73570f0df68988e21abb0a58b52e1d914`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 238.5 KB (238469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal-non-free`

```console
$ docker pull neurodebian@sha256:7ae6f8dff41c0235b6d27fe78cf4eee3d754c98a9c9821f36e77236dc925f552
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:focal-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:108c69cf6392b3d1b949af39953aacd1021687c93fcc3d623c3bd99e152e1dc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a3385e084c1283d64781c31064f68f3d3d259a6048ea0f3ae14b523fc4abcde`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:37:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:37:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:37:42 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:45 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0d85648c57095c325776ef894c7e76c557caf12f9bcb61f510da5c30f4f660`  
		Last Modified: Tue, 07 Jun 2022 00:39:47 GMT  
		Size: 5.5 MB (5489017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b42d0b055eb8b4dabb68755df18c0921420d071b554c246ac4ec6068416583`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be77e820178f2d7d401e7cb28b70f9a90763d3bd2626132c372fec5ccbacc805`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885284a345938a81195044fcfc0624d73570f0df68988e21abb0a58b52e1d914`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 238.5 KB (238469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c25ef9a1e3a54caf76ffdf6eae063350a823350aed154a1ef78ae1b1fd8eea`  
		Last Modified: Tue, 07 Jun 2022 00:39:56 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:impish`

```console
$ docker pull neurodebian@sha256:7aaf8441df1e42705456bbd66f50bacdc3dbebdacc47c7bd4683c5666e25a836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:impish` - linux; amd64

```console
$ docker pull neurodebian@sha256:db1963ee159e0dca0159562742ad532d2a086a988b9354057ed8d77647b5e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34384580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e017fc712553f899766998fdb9db30eee355df9033c23dd72ba12b43aa47eb`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:38:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:38:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:38:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4222215fe5bb0924cc9cbcbbb6d524fc181c91b66bd31430a258a78ebce2c519`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 3.8 MB (3752244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983039d4e1a2415f0f809ddd83bcc60a90fe40cf2e2c3a4f93ded36ac4cab37a`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d378c9cd6485d098e5bcf609a3e34edc5c31a424035a4bd61de01eadbab71c6`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e2ecd075adf7f432e69fbe49ea1b42a7c15c0cf6114789b57ffa534f851834`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 250.0 KB (250036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:impish-non-free`

```console
$ docker pull neurodebian@sha256:5a77977ca5ebaa347ada2a1fde9660136750fe448accb5fa7aab557e62d4dc20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:impish-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:6d8c7ae8926031b53a89c3cbe66d4b0b71033d1c6700ec08d99e5cc48ad46127
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34384837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97acd8721334f31321e82f55bd3390a97582b3c638b7df12fface737d824aa2`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:38:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:38:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:38:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:28 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4222215fe5bb0924cc9cbcbbb6d524fc181c91b66bd31430a258a78ebce2c519`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 3.8 MB (3752244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983039d4e1a2415f0f809ddd83bcc60a90fe40cf2e2c3a4f93ded36ac4cab37a`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d378c9cd6485d098e5bcf609a3e34edc5c31a424035a4bd61de01eadbab71c6`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e2ecd075adf7f432e69fbe49ea1b42a7c15c0cf6114789b57ffa534f851834`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 250.0 KB (250036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d9026add10c208d1645d8621401ea34527cba1f3341e18c57b337fba2b4ab3`  
		Last Modified: Tue, 07 Jun 2022 00:40:15 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:c594c3ef72db3990d13d53cf2a014328b50460cad2bc9ba20c28d52a7f2bb606
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:f9c473661ee2f6c1b9af6d80cfe37980d51be56b56728e4c85a3b4b74dae0714
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66632946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ff7873e504d0b4ffc2d821b9d777f9dad9f593f3431dd0bde40441e4ed03e2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:12 GMT
ADD file:dd3d4b31d7f1d4062ad0eb2d85dba064cea067b1eb4a8b89a0b593ea90001cdf in / 
# Sat, 28 May 2022 01:20:12 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e756f3fdd6a378aa16205b0f75d178b7532b110e86be7659004fc6a21183226c`  
		Last Modified: Sat, 28 May 2022 01:24:51 GMT  
		Size: 55.0 MB (55009253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042d25d72a7dea1cac3b0025ffda5a744367e349b4b8af91ee511c0987d31e8`  
		Last Modified: Sat, 28 May 2022 05:39:30 GMT  
		Size: 11.3 MB (11310360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f8ddb2c45cc88bdf5de437bff502c544b8c489d28b4928b5f58b8432440f24`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d815e97d100e1c9e458bc54972d5fde92a3239754eb453077fc38dbc42e6b9`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e5783c05be991fe571e19a5fe838b22f8120fab5f86db0a60b24721fcad9da`  
		Last Modified: Sat, 28 May 2022 05:39:29 GMT  
		Size: 311.3 KB (311322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:8a939884574b95629b0e008af76e99e33cf54ce237d4ed26c02a8f862095fdc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:d4047f5074c13db64929af6984a864c67c70f6f9caf9cb192c54672ccad9de42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65097820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19a507df560f2fe395d315cc58e338ab078fe6eea8239aee02247b6c115df113`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:21:32 GMT
ADD file:dffa51e87e58558bb4b777e117ecb18500d90a9646513d0d8d9724bb5c949dc5 in / 
# Sat, 28 May 2022 01:21:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7fa02d3fa6e2ab30d6142a096f5321227237c89c02dd890ff9fa745dbf0790d1`  
		Last Modified: Sat, 28 May 2022 01:27:35 GMT  
		Size: 53.2 MB (53161898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e893d63a4ae27cf63fe131c1636a8b660f2c2ec88c1b6f04fc8aebc6c5032e07`  
		Last Modified: Sat, 28 May 2022 05:40:18 GMT  
		Size: 11.6 MB (11642383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f98b8c1b303902f87110931f235a66eaaa10c3b6effa369c4605bfbbd17f17`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779eecbc9c1e457821d1405943bf4e67f06251aeac84234e0c2a43cf5b1c1098`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6c5e124545a21a4d8b1bd0e2d39c824b39280a4195f0186b920b242937c68f`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 291.5 KB (291531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:1c97c80218492f67201905a2ef77914016f4c3f84b0944f2be32fa9d5f2ce771
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:c9946dd4a8acdd0f5ae42a3aa6388845efc231efed63604aae19dafd89e07f09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65098138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f75e10478632a1500885cc4b349960a0a1023b8431dcb21da5343f4a235e8c3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:21:32 GMT
ADD file:dffa51e87e58558bb4b777e117ecb18500d90a9646513d0d8d9724bb5c949dc5 in / 
# Sat, 28 May 2022 01:21:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:38:03 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:7fa02d3fa6e2ab30d6142a096f5321227237c89c02dd890ff9fa745dbf0790d1`  
		Last Modified: Sat, 28 May 2022 01:27:35 GMT  
		Size: 53.2 MB (53161898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e893d63a4ae27cf63fe131c1636a8b660f2c2ec88c1b6f04fc8aebc6c5032e07`  
		Last Modified: Sat, 28 May 2022 05:40:18 GMT  
		Size: 11.6 MB (11642383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f98b8c1b303902f87110931f235a66eaaa10c3b6effa369c4605bfbbd17f17`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779eecbc9c1e457821d1405943bf4e67f06251aeac84234e0c2a43cf5b1c1098`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6c5e124545a21a4d8b1bd0e2d39c824b39280a4195f0186b920b242937c68f`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 291.5 KB (291531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dbd0f31bfda6ecad55ae077dcc7934a72952336e9aa1be2bac9f77fcea7bf2`  
		Last Modified: Sat, 28 May 2022 05:40:27 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100`

```console
$ docker pull neurodebian@sha256:b9cbc75b38dca65aefd999e8c0e591ed965f95db49d8f03688c8eeedb689bb9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd100` - linux; amd64

```console
$ docker pull neurodebian@sha256:59c8f1bd0b8c2bc34454fdffb814b231fceeac95b2e7f133c3b326fbb08f1651
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61245500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b64a0beed441d3db2a683632858a879fe7ad1df1244094e2cd4cdcde7153b6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:36:58 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:36:59 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:00 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:04 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b408b972c76f457b5928d48a45e6c6669ce35818a0c203b012c6966b8d654289`  
		Last Modified: Sat, 28 May 2022 05:39:10 GMT  
		Size: 10.5 MB (10500296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f476d1ba5bb41283ab8a2ef5d7968db4f7e10aab5242fbb3f8381dab67b636`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a556d3bcd634466f553097ef3d03a9bd26dc13edafe9511d4254a1fc257c45e1`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b5e5f807a99c180c7ceadd62cd0a13b22b4f9edae5661acf56bc40c9e9b169`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 302.8 KB (302771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:34bd541da284138fed75724766e0d5e3cac218103ccab5d712db0e8002858d41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:b6f2c3e37f8532066293ccd087ca1f2511ae131f78439be9a9d3ab8dc26991f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61245865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d9e8dac7e90dcb98355f93be5c3ac21e3621c86c21152b1ecfdc8ea81e94a4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:36:58 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:36:59 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:00 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:04 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:08 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b408b972c76f457b5928d48a45e6c6669ce35818a0c203b012c6966b8d654289`  
		Last Modified: Sat, 28 May 2022 05:39:10 GMT  
		Size: 10.5 MB (10500296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f476d1ba5bb41283ab8a2ef5d7968db4f7e10aab5242fbb3f8381dab67b636`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a556d3bcd634466f553097ef3d03a9bd26dc13edafe9511d4254a1fc257c45e1`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b5e5f807a99c180c7ceadd62cd0a13b22b4f9edae5661acf56bc40c9e9b169`  
		Last Modified: Sat, 28 May 2022 05:39:09 GMT  
		Size: 302.8 KB (302771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca022902e8dca86c10ed36509f07e5cb9ccafaacbf0687a47d858b5f7e344c66`  
		Last Modified: Sat, 28 May 2022 05:39:19 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110`

```console
$ docker pull neurodebian@sha256:c594c3ef72db3990d13d53cf2a014328b50460cad2bc9ba20c28d52a7f2bb606
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd110` - linux; amd64

```console
$ docker pull neurodebian@sha256:f9c473661ee2f6c1b9af6d80cfe37980d51be56b56728e4c85a3b4b74dae0714
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66632946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ff7873e504d0b4ffc2d821b9d777f9dad9f593f3431dd0bde40441e4ed03e2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:12 GMT
ADD file:dd3d4b31d7f1d4062ad0eb2d85dba064cea067b1eb4a8b89a0b593ea90001cdf in / 
# Sat, 28 May 2022 01:20:12 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e756f3fdd6a378aa16205b0f75d178b7532b110e86be7659004fc6a21183226c`  
		Last Modified: Sat, 28 May 2022 01:24:51 GMT  
		Size: 55.0 MB (55009253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042d25d72a7dea1cac3b0025ffda5a744367e349b4b8af91ee511c0987d31e8`  
		Last Modified: Sat, 28 May 2022 05:39:30 GMT  
		Size: 11.3 MB (11310360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f8ddb2c45cc88bdf5de437bff502c544b8c489d28b4928b5f58b8432440f24`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d815e97d100e1c9e458bc54972d5fde92a3239754eb453077fc38dbc42e6b9`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e5783c05be991fe571e19a5fe838b22f8120fab5f86db0a60b24721fcad9da`  
		Last Modified: Sat, 28 May 2022 05:39:29 GMT  
		Size: 311.3 KB (311322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:7f5da94d65103f01e54681100cb3d38bdb2642cd40749f1b7bb39111688e0aa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:e79b980580bba0fb6032a8d7dd07d2dfe9d8f55a1ead5e2d622fcea7bf783e31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66633311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16391b661151b02a3078f451d2e12b290e9d5d8fe88cac6809419c9752790d5b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:12 GMT
ADD file:dd3d4b31d7f1d4062ad0eb2d85dba064cea067b1eb4a8b89a0b593ea90001cdf in / 
# Sat, 28 May 2022 01:20:12 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:25 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:e756f3fdd6a378aa16205b0f75d178b7532b110e86be7659004fc6a21183226c`  
		Last Modified: Sat, 28 May 2022 01:24:51 GMT  
		Size: 55.0 MB (55009253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042d25d72a7dea1cac3b0025ffda5a744367e349b4b8af91ee511c0987d31e8`  
		Last Modified: Sat, 28 May 2022 05:39:30 GMT  
		Size: 11.3 MB (11310360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f8ddb2c45cc88bdf5de437bff502c544b8c489d28b4928b5f58b8432440f24`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d815e97d100e1c9e458bc54972d5fde92a3239754eb453077fc38dbc42e6b9`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e5783c05be991fe571e19a5fe838b22f8120fab5f86db0a60b24721fcad9da`  
		Last Modified: Sat, 28 May 2022 05:39:29 GMT  
		Size: 311.3 KB (311322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07471eb1d1598973692a746f2cc5cac14a11e55b43f93822a12a117ecbb8572a`  
		Last Modified: Sat, 28 May 2022 05:39:41 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120`

```console
$ docker pull neurodebian@sha256:78c9f3eccfaafb9fb4dd2a9dca8820b44d93473e5c6f0498f2190e9e946a68c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd120` - linux; amd64

```console
$ docker pull neurodebian@sha256:068faa6f7448a0d180c996d5535104e837626f54186aeaf014d75dcca8a26d58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64881666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bebcce458d791df05d664cf985b5b3b9b402a6a3d51a53b85df9b114e47e838c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:19:50 GMT
ADD file:05d40d360d088a73d2d9ea8361742b3b0e7f5ac80923374f84acf3d1be6c7798 in / 
# Sat, 28 May 2022 01:19:52 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:36 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:40 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1afe78e67a22dc5c619d5518a1d45e8f5ca31628fa6b7caa3b645c4fba19faaa`  
		Last Modified: Sat, 28 May 2022 01:24:12 GMT  
		Size: 52.9 MB (52947713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d562bd670035564f61d24341f5130b01d36042c36107e0a987fb466eb6d6ffb8`  
		Last Modified: Sat, 28 May 2022 05:39:54 GMT  
		Size: 11.6 MB (11640504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7050b6924f15d3e72dbb1096546f83c63ecdbbca6186c8f851a03625a1f32674`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bda5105d9eff32d11d816fd1398dce31832adc9410be0638a2acea9cbe9b7b`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f537aae945d8347c844b8fb05e793d4a82d4539f9582be5aee2b0eecdc4db8e5`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 291.4 KB (291437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:3bb5cb32011cd186cd2fe4ef5ab98d32eaee384e75cd3bd68dbe1c92132893e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:ae48c9830c46b712195cfb1f7b88a2decbe44bdc56d140d415df9b1e2b7c2d6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64882033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d04a564923a36175ecb0b612039ac656fe8b127f4e837dc08c9acd6e4141f84d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:19:50 GMT
ADD file:05d40d360d088a73d2d9ea8361742b3b0e7f5ac80923374f84acf3d1be6c7798 in / 
# Sat, 28 May 2022 01:19:52 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:36 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:40 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:44 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:1afe78e67a22dc5c619d5518a1d45e8f5ca31628fa6b7caa3b645c4fba19faaa`  
		Last Modified: Sat, 28 May 2022 01:24:12 GMT  
		Size: 52.9 MB (52947713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d562bd670035564f61d24341f5130b01d36042c36107e0a987fb466eb6d6ffb8`  
		Last Modified: Sat, 28 May 2022 05:39:54 GMT  
		Size: 11.6 MB (11640504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7050b6924f15d3e72dbb1096546f83c63ecdbbca6186c8f851a03625a1f32674`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bda5105d9eff32d11d816fd1398dce31832adc9410be0638a2acea9cbe9b7b`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f537aae945d8347c844b8fb05e793d4a82d4539f9582be5aee2b0eecdc4db8e5`  
		Last Modified: Sat, 28 May 2022 05:39:53 GMT  
		Size: 291.4 KB (291437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfbc4116d9376d185dae07ff9b45bf648c9f12cd31942524fc08991a21d25a5`  
		Last Modified: Sat, 28 May 2022 05:40:07 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd16.04`

```console
$ docker pull neurodebian@sha256:4f8f3b02888f61824d206a937db34a20819de9cf11a2a0161dcfa463c4cba1fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd16.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:d80e83bfcc000dd04b02c778a1297c7ad2540cb555ab96c90ec154c6a4f0f495
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60902017c278b0db41b17f8f1de27469127d1ea4898b2469f52647585af6120`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:57:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Mar 2022 17:27:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 16 Mar 2022 17:27:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 16 Mar 2022 17:27:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84732b274efc4bdfc5e30a12f05cbd1a9936e3ed5e8952879d6ee935df35eb79`  
		Last Modified: Tue, 31 Aug 2021 04:00:24 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3505bfdde8eb1415423d95064ff6b92c835526022feb1d95009ab5ec04c115`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3fae1c80c2541f9a1f6a2df3ea6faa8f5c9797dda86103383518675981d44`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a78747ad8c43a648a10d04a1c586defca6040cc6c5a4acf404d3962d361631a`  
		Last Modified: Wed, 16 Mar 2022 17:35:35 GMT  
		Size: 227.0 KB (226984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd16.04-non-free`

```console
$ docker pull neurodebian@sha256:79afd2bee6d4c71c226efc18ed02df20d4b960303d3726749e5316d6e833137b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd16.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:2614aec9e563f0b111961f993de935a0fbb9620cdb11473ac31ec813dac0323e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4763f90a405bf63daed0435933c43c39b39f71793a896d5ed656d45e8fb9242`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:57:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Mar 2022 17:27:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 16 Mar 2022 17:27:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 16 Mar 2022 17:27:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Mar 2022 17:27:29 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84732b274efc4bdfc5e30a12f05cbd1a9936e3ed5e8952879d6ee935df35eb79`  
		Last Modified: Tue, 31 Aug 2021 04:00:24 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3505bfdde8eb1415423d95064ff6b92c835526022feb1d95009ab5ec04c115`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3fae1c80c2541f9a1f6a2df3ea6faa8f5c9797dda86103383518675981d44`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a78747ad8c43a648a10d04a1c586defca6040cc6c5a4acf404d3962d361631a`  
		Last Modified: Wed, 16 Mar 2022 17:35:35 GMT  
		Size: 227.0 KB (226984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374df1832948bd22b70477d80f3e38c6fb69de53d87a19787be363131e99a16f`  
		Last Modified: Wed, 16 Mar 2022 17:35:44 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04`

```console
$ docker pull neurodebian@sha256:24dbb94d281291cb1e04b6108e5eaca921dfee07b976021bf1dccd7d516833b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd18.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:375123cc33c1c024fb8429f011c99b58c87203c5a4a936adfaa84064dee99f3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31771462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3bbfb1b8f311ec84d7ab789e1111bcaf2f73b4ff6fb1611454c72a12352a8a4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:37:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:37:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:37:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2b3981bc62720e6e1f9f8b6fd2d4af6b8dc0d5d1d930cad27b75a30d93221`  
		Last Modified: Tue, 07 Jun 2022 00:39:28 GMT  
		Size: 4.8 MB (4817739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff80362b7a8a66dc0750954a4c03f08846b9241ac54372ec5bae9d12540d468`  
		Last Modified: Tue, 07 Jun 2022 00:39:27 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d453cada745b8af1182eb78a54478ae0375ac8f0b4b908d273b10429bcd7ec81`  
		Last Modified: Tue, 07 Jun 2022 00:39:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f79b6a697fd3011ea990d9d8ef464697221eacc2d053352e61632bcb16d3c3`  
		Last Modified: Tue, 07 Jun 2022 00:39:27 GMT  
		Size: 240.2 KB (240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04-non-free`

```console
$ docker pull neurodebian@sha256:d9f97ebb267aa7ecef9b61d57a119f4c1938d73201aa1a0915b356ac6c74858d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd18.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:52db60494f9b1f9ed71c583e724777aea45be1f56982bbdbb06faae6efbb384e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31771718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2d6fea5ab69bb8a2c661a8b8ccb7226fbd7c8b58f1e12a5cff9753a8d035ed2`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:37:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:37:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:37:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:25 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2b3981bc62720e6e1f9f8b6fd2d4af6b8dc0d5d1d930cad27b75a30d93221`  
		Last Modified: Tue, 07 Jun 2022 00:39:28 GMT  
		Size: 4.8 MB (4817739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff80362b7a8a66dc0750954a4c03f08846b9241ac54372ec5bae9d12540d468`  
		Last Modified: Tue, 07 Jun 2022 00:39:27 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d453cada745b8af1182eb78a54478ae0375ac8f0b4b908d273b10429bcd7ec81`  
		Last Modified: Tue, 07 Jun 2022 00:39:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f79b6a697fd3011ea990d9d8ef464697221eacc2d053352e61632bcb16d3c3`  
		Last Modified: Tue, 07 Jun 2022 00:39:27 GMT  
		Size: 240.2 KB (240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326546dbbe4e98516ffed1b2576dbaaa1a592e2c5f4e103da5d95ffe6b418ef1`  
		Last Modified: Tue, 07 Jun 2022 00:39:37 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04`

```console
$ docker pull neurodebian@sha256:910dff6bf17ef9c6ecdc30982ee18bd4d09fb2c1f740e53348afde41e021eaf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd20.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:39f2154d2cdb8d241fe22e1aa8d7646d29503aa842ac35aad54d97266de1598b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db6a99a7f13a251621d206e8da7fe6bab43d65ea0af1fc7a69a8d49754a79959`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:37:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:37:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:37:42 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0d85648c57095c325776ef894c7e76c557caf12f9bcb61f510da5c30f4f660`  
		Last Modified: Tue, 07 Jun 2022 00:39:47 GMT  
		Size: 5.5 MB (5489017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b42d0b055eb8b4dabb68755df18c0921420d071b554c246ac4ec6068416583`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be77e820178f2d7d401e7cb28b70f9a90763d3bd2626132c372fec5ccbacc805`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885284a345938a81195044fcfc0624d73570f0df68988e21abb0a58b52e1d914`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 238.5 KB (238469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04-non-free`

```console
$ docker pull neurodebian@sha256:7ae6f8dff41c0235b6d27fe78cf4eee3d754c98a9c9821f36e77236dc925f552
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd20.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:108c69cf6392b3d1b949af39953aacd1021687c93fcc3d623c3bd99e152e1dc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a3385e084c1283d64781c31064f68f3d3d259a6048ea0f3ae14b523fc4abcde`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:37:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:37:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:37:42 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:45 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0d85648c57095c325776ef894c7e76c557caf12f9bcb61f510da5c30f4f660`  
		Last Modified: Tue, 07 Jun 2022 00:39:47 GMT  
		Size: 5.5 MB (5489017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b42d0b055eb8b4dabb68755df18c0921420d071b554c246ac4ec6068416583`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be77e820178f2d7d401e7cb28b70f9a90763d3bd2626132c372fec5ccbacc805`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885284a345938a81195044fcfc0624d73570f0df68988e21abb0a58b52e1d914`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 238.5 KB (238469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c25ef9a1e3a54caf76ffdf6eae063350a823350aed154a1ef78ae1b1fd8eea`  
		Last Modified: Tue, 07 Jun 2022 00:39:56 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd21.10`

```console
$ docker pull neurodebian@sha256:7aaf8441df1e42705456bbd66f50bacdc3dbebdacc47c7bd4683c5666e25a836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd21.10` - linux; amd64

```console
$ docker pull neurodebian@sha256:db1963ee159e0dca0159562742ad532d2a086a988b9354057ed8d77647b5e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34384580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e017fc712553f899766998fdb9db30eee355df9033c23dd72ba12b43aa47eb`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:38:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:38:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:38:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4222215fe5bb0924cc9cbcbbb6d524fc181c91b66bd31430a258a78ebce2c519`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 3.8 MB (3752244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983039d4e1a2415f0f809ddd83bcc60a90fe40cf2e2c3a4f93ded36ac4cab37a`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d378c9cd6485d098e5bcf609a3e34edc5c31a424035a4bd61de01eadbab71c6`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e2ecd075adf7f432e69fbe49ea1b42a7c15c0cf6114789b57ffa534f851834`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 250.0 KB (250036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd21.10-non-free`

```console
$ docker pull neurodebian@sha256:5a77977ca5ebaa347ada2a1fde9660136750fe448accb5fa7aab557e62d4dc20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd21.10-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:6d8c7ae8926031b53a89c3cbe66d4b0b71033d1c6700ec08d99e5cc48ad46127
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34384837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97acd8721334f31321e82f55bd3390a97582b3c638b7df12fface737d824aa2`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:38:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:38:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:38:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:28 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4222215fe5bb0924cc9cbcbbb6d524fc181c91b66bd31430a258a78ebce2c519`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 3.8 MB (3752244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983039d4e1a2415f0f809ddd83bcc60a90fe40cf2e2c3a4f93ded36ac4cab37a`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d378c9cd6485d098e5bcf609a3e34edc5c31a424035a4bd61de01eadbab71c6`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e2ecd075adf7f432e69fbe49ea1b42a7c15c0cf6114789b57ffa534f851834`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 250.0 KB (250036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d9026add10c208d1645d8621401ea34527cba1f3341e18c57b337fba2b4ab3`  
		Last Modified: Tue, 07 Jun 2022 00:40:15 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd90`

```console
$ docker pull neurodebian@sha256:c914de67f522ff143c351014549fbc7a99eaedfd3e55e8e389571c6829b81539
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd90` - linux; amd64

```console
$ docker pull neurodebian@sha256:22465c84b107281c447a1083a4f1f3f0f944be234b9f17b7e86cab22f22319fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52298309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff5f76641a5390ddc675f50f2fe9b530869b689be5a22f5222e56e9ea1924d8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:36:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:36:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:36:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:36:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53032c7bddb3b2e8c2de1e25d78411be689bf7effc71a975583142ac4583497`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 6.6 MB (6572860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0f40fc54db07d6cead19c0c27fabd467d3ef85bb483adaf55c6a5f9fa9a84`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 3.2 KB (3156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc6a032a7f850c01faab3c678d84daa90794e05c89876550c693d57079f289`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8f2d589de5a69876d0301d1115c435f1ff204ddf9e7da2dca92e08ef77c327`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 292.3 KB (292319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd90-non-free`

```console
$ docker pull neurodebian@sha256:da2038eb5562e027f46c8338c6f2def20f52ff060897f08ac2f667dd79d31923
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd90-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:51f10fdd6d8a1a7fb99defc9ddb11e736171bab179d11551de8a98c06c728eec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52298676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c305eab94692f4f6969be81c2a09ea43160496e09a122931e8bc8e239e6ef3d9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:36:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:36:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:36:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:36:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:36:50 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53032c7bddb3b2e8c2de1e25d78411be689bf7effc71a975583142ac4583497`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 6.6 MB (6572860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0f40fc54db07d6cead19c0c27fabd467d3ef85bb483adaf55c6a5f9fa9a84`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 3.2 KB (3156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc6a032a7f850c01faab3c678d84daa90794e05c89876550c693d57079f289`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8f2d589de5a69876d0301d1115c435f1ff204ddf9e7da2dca92e08ef77c327`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 292.3 KB (292319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601b728a30ef3015c4146edae6d99c749c872db9e246147316784e3a5f404209`  
		Last Modified: Sat, 28 May 2022 05:39:00 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:non-free`

```console
$ docker pull neurodebian@sha256:7f5da94d65103f01e54681100cb3d38bdb2642cd40749f1b7bb39111688e0aa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:e79b980580bba0fb6032a8d7dd07d2dfe9d8f55a1ead5e2d622fcea7bf783e31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66633311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16391b661151b02a3078f451d2e12b290e9d5d8fe88cac6809419c9752790d5b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:12 GMT
ADD file:dd3d4b31d7f1d4062ad0eb2d85dba064cea067b1eb4a8b89a0b593ea90001cdf in / 
# Sat, 28 May 2022 01:20:12 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:25 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:e756f3fdd6a378aa16205b0f75d178b7532b110e86be7659004fc6a21183226c`  
		Last Modified: Sat, 28 May 2022 01:24:51 GMT  
		Size: 55.0 MB (55009253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042d25d72a7dea1cac3b0025ffda5a744367e349b4b8af91ee511c0987d31e8`  
		Last Modified: Sat, 28 May 2022 05:39:30 GMT  
		Size: 11.3 MB (11310360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f8ddb2c45cc88bdf5de437bff502c544b8c489d28b4928b5f58b8432440f24`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d815e97d100e1c9e458bc54972d5fde92a3239754eb453077fc38dbc42e6b9`  
		Last Modified: Sat, 28 May 2022 05:39:28 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e5783c05be991fe571e19a5fe838b22f8120fab5f86db0a60b24721fcad9da`  
		Last Modified: Sat, 28 May 2022 05:39:29 GMT  
		Size: 311.3 KB (311322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07471eb1d1598973692a746f2cc5cac14a11e55b43f93822a12a117ecbb8572a`  
		Last Modified: Sat, 28 May 2022 05:39:41 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:8a939884574b95629b0e008af76e99e33cf54ce237d4ed26c02a8f862095fdc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:d4047f5074c13db64929af6984a864c67c70f6f9caf9cb192c54672ccad9de42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65097820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19a507df560f2fe395d315cc58e338ab078fe6eea8239aee02247b6c115df113`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:21:32 GMT
ADD file:dffa51e87e58558bb4b777e117ecb18500d90a9646513d0d8d9724bb5c949dc5 in / 
# Sat, 28 May 2022 01:21:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7fa02d3fa6e2ab30d6142a096f5321227237c89c02dd890ff9fa745dbf0790d1`  
		Last Modified: Sat, 28 May 2022 01:27:35 GMT  
		Size: 53.2 MB (53161898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e893d63a4ae27cf63fe131c1636a8b660f2c2ec88c1b6f04fc8aebc6c5032e07`  
		Last Modified: Sat, 28 May 2022 05:40:18 GMT  
		Size: 11.6 MB (11642383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f98b8c1b303902f87110931f235a66eaaa10c3b6effa369c4605bfbbd17f17`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779eecbc9c1e457821d1405943bf4e67f06251aeac84234e0c2a43cf5b1c1098`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6c5e124545a21a4d8b1bd0e2d39c824b39280a4195f0186b920b242937c68f`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 291.5 KB (291531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:1c97c80218492f67201905a2ef77914016f4c3f84b0944f2be32fa9d5f2ce771
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:c9946dd4a8acdd0f5ae42a3aa6388845efc231efed63604aae19dafd89e07f09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65098138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f75e10478632a1500885cc4b349960a0a1023b8431dcb21da5343f4a235e8c3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:21:32 GMT
ADD file:dffa51e87e58558bb4b777e117ecb18500d90a9646513d0d8d9724bb5c949dc5 in / 
# Sat, 28 May 2022 01:21:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:37:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:37:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:37:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:37:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:38:03 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:7fa02d3fa6e2ab30d6142a096f5321227237c89c02dd890ff9fa745dbf0790d1`  
		Last Modified: Sat, 28 May 2022 01:27:35 GMT  
		Size: 53.2 MB (53161898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e893d63a4ae27cf63fe131c1636a8b660f2c2ec88c1b6f04fc8aebc6c5032e07`  
		Last Modified: Sat, 28 May 2022 05:40:18 GMT  
		Size: 11.6 MB (11642383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f98b8c1b303902f87110931f235a66eaaa10c3b6effa369c4605bfbbd17f17`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779eecbc9c1e457821d1405943bf4e67f06251aeac84234e0c2a43cf5b1c1098`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6c5e124545a21a4d8b1bd0e2d39c824b39280a4195f0186b920b242937c68f`  
		Last Modified: Sat, 28 May 2022 05:40:17 GMT  
		Size: 291.5 KB (291531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dbd0f31bfda6ecad55ae077dcc7934a72952336e9aa1be2bac9f77fcea7bf2`  
		Last Modified: Sat, 28 May 2022 05:40:27 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:stretch`

```console
$ docker pull neurodebian@sha256:c914de67f522ff143c351014549fbc7a99eaedfd3e55e8e389571c6829b81539
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:stretch` - linux; amd64

```console
$ docker pull neurodebian@sha256:22465c84b107281c447a1083a4f1f3f0f944be234b9f17b7e86cab22f22319fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52298309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff5f76641a5390ddc675f50f2fe9b530869b689be5a22f5222e56e9ea1924d8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:36:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:36:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:36:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:36:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53032c7bddb3b2e8c2de1e25d78411be689bf7effc71a975583142ac4583497`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 6.6 MB (6572860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0f40fc54db07d6cead19c0c27fabd467d3ef85bb483adaf55c6a5f9fa9a84`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 3.2 KB (3156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc6a032a7f850c01faab3c678d84daa90794e05c89876550c693d57079f289`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8f2d589de5a69876d0301d1115c435f1ff204ddf9e7da2dca92e08ef77c327`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 292.3 KB (292319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:stretch-non-free`

```console
$ docker pull neurodebian@sha256:da2038eb5562e027f46c8338c6f2def20f52ff060897f08ac2f667dd79d31923
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:stretch-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:51f10fdd6d8a1a7fb99defc9ddb11e736171bab179d11551de8a98c06c728eec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52298676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c305eab94692f4f6969be81c2a09ea43160496e09a122931e8bc8e239e6ef3d9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:36:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:36:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 May 2022 05:36:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 May 2022 05:36:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:36:50 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53032c7bddb3b2e8c2de1e25d78411be689bf7effc71a975583142ac4583497`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 6.6 MB (6572860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0f40fc54db07d6cead19c0c27fabd467d3ef85bb483adaf55c6a5f9fa9a84`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 3.2 KB (3156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc6a032a7f850c01faab3c678d84daa90794e05c89876550c693d57079f289`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8f2d589de5a69876d0301d1115c435f1ff204ddf9e7da2dca92e08ef77c327`  
		Last Modified: Sat, 28 May 2022 05:38:50 GMT  
		Size: 292.3 KB (292319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601b728a30ef3015c4146edae6d99c749c872db9e246147316784e3a5f404209`  
		Last Modified: Sat, 28 May 2022 05:39:00 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:xenial`

```console
$ docker pull neurodebian@sha256:4f8f3b02888f61824d206a937db34a20819de9cf11a2a0161dcfa463c4cba1fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:xenial` - linux; amd64

```console
$ docker pull neurodebian@sha256:d80e83bfcc000dd04b02c778a1297c7ad2540cb555ab96c90ec154c6a4f0f495
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60902017c278b0db41b17f8f1de27469127d1ea4898b2469f52647585af6120`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:57:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Mar 2022 17:27:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 16 Mar 2022 17:27:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 16 Mar 2022 17:27:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84732b274efc4bdfc5e30a12f05cbd1a9936e3ed5e8952879d6ee935df35eb79`  
		Last Modified: Tue, 31 Aug 2021 04:00:24 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3505bfdde8eb1415423d95064ff6b92c835526022feb1d95009ab5ec04c115`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3fae1c80c2541f9a1f6a2df3ea6faa8f5c9797dda86103383518675981d44`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a78747ad8c43a648a10d04a1c586defca6040cc6c5a4acf404d3962d361631a`  
		Last Modified: Wed, 16 Mar 2022 17:35:35 GMT  
		Size: 227.0 KB (226984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:xenial-non-free`

```console
$ docker pull neurodebian@sha256:79afd2bee6d4c71c226efc18ed02df20d4b960303d3726749e5316d6e833137b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:xenial-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:2614aec9e563f0b111961f993de935a0fbb9620cdb11473ac31ec813dac0323e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4763f90a405bf63daed0435933c43c39b39f71793a896d5ed656d45e8fb9242`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:57:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Mar 2022 17:27:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 16 Mar 2022 17:27:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 16 Mar 2022 17:27:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Mar 2022 17:27:29 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84732b274efc4bdfc5e30a12f05cbd1a9936e3ed5e8952879d6ee935df35eb79`  
		Last Modified: Tue, 31 Aug 2021 04:00:24 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3505bfdde8eb1415423d95064ff6b92c835526022feb1d95009ab5ec04c115`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3fae1c80c2541f9a1f6a2df3ea6faa8f5c9797dda86103383518675981d44`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a78747ad8c43a648a10d04a1c586defca6040cc6c5a4acf404d3962d361631a`  
		Last Modified: Wed, 16 Mar 2022 17:35:35 GMT  
		Size: 227.0 KB (226984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374df1832948bd22b70477d80f3e38c6fb69de53d87a19787be363131e99a16f`  
		Last Modified: Wed, 16 Mar 2022 17:35:44 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
