<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `sapmachine`

-	[`sapmachine:11`](#sapmachine11)
-	[`sapmachine:11.0.12`](#sapmachine11012)
-	[`sapmachine:17`](#sapmachine17)
-	[`sapmachine:latest`](#sapmachinelatest)
-	[`sapmachine:lts`](#sapmachinelts)

## `sapmachine:11`

```console
$ docker pull sapmachine@sha256:8f75bfdab450ad0d6d0648168278e7dba212a4279a2a8853fb2f893c85b4691c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:11` - linux; amd64

```console
$ docker pull sapmachine@sha256:e1b69706945d30cdc5db6a3e957405a3d5cb926461ca5509b368237592c19640
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235086424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668c6dd9864c680a07a1277984a16ec7f67bdef2bd39dc27970d73c32e6ac1ce`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 05:09:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:10:54 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.12     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:10:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Tue, 31 Aug 2021 05:10:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6749e8b9c88959d91457b9b57bd8d08701cf0f82a7b72d535eab42ee6b319730`  
		Last Modified: Tue, 31 Aug 2021 05:11:13 GMT  
		Size: 8.3 MB (8324712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac7c23689bbbf0c05c6b22648b3efdb001ac588a23ab0ebda214e5317c3a851`  
		Last Modified: Tue, 31 Aug 2021 05:11:54 GMT  
		Size: 198.2 MB (198191638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:11.0.12`

```console
$ docker pull sapmachine@sha256:8f75bfdab450ad0d6d0648168278e7dba212a4279a2a8853fb2f893c85b4691c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:11.0.12` - linux; amd64

```console
$ docker pull sapmachine@sha256:e1b69706945d30cdc5db6a3e957405a3d5cb926461ca5509b368237592c19640
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235086424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668c6dd9864c680a07a1277984a16ec7f67bdef2bd39dc27970d73c32e6ac1ce`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 05:09:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:10:54 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.12     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:10:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Tue, 31 Aug 2021 05:10:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6749e8b9c88959d91457b9b57bd8d08701cf0f82a7b72d535eab42ee6b319730`  
		Last Modified: Tue, 31 Aug 2021 05:11:13 GMT  
		Size: 8.3 MB (8324712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac7c23689bbbf0c05c6b22648b3efdb001ac588a23ab0ebda214e5317c3a851`  
		Last Modified: Tue, 31 Aug 2021 05:11:54 GMT  
		Size: 198.2 MB (198191638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:17`

```console
$ docker pull sapmachine@sha256:52cdbdab16a320526a9d18628ab175d3633644c62a77a11b1e3f680052831882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:17` - linux; amd64

```console
$ docker pull sapmachine@sha256:8202cf21f9460e96d8135e32ad8f6a6844b6936cd9d4cb3938d19e6bd81d2604
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234482194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc16856577406f0955caa4f7621f0403e0d8070b91006a6ba3fe0215f5d19f8`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 05:09:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Sep 2021 21:40:12 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Sep 2021 21:40:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Fri, 17 Sep 2021 21:40:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6749e8b9c88959d91457b9b57bd8d08701cf0f82a7b72d535eab42ee6b319730`  
		Last Modified: Tue, 31 Aug 2021 05:11:13 GMT  
		Size: 8.3 MB (8324712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba8feeb93aca0fa4ef299529124f97304595c44a5788f3d37068e45f279e719`  
		Last Modified: Fri, 17 Sep 2021 21:40:49 GMT  
		Size: 197.6 MB (197587408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:52cdbdab16a320526a9d18628ab175d3633644c62a77a11b1e3f680052831882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:8202cf21f9460e96d8135e32ad8f6a6844b6936cd9d4cb3938d19e6bd81d2604
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234482194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc16856577406f0955caa4f7621f0403e0d8070b91006a6ba3fe0215f5d19f8`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 05:09:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Sep 2021 21:40:12 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Sep 2021 21:40:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Fri, 17 Sep 2021 21:40:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6749e8b9c88959d91457b9b57bd8d08701cf0f82a7b72d535eab42ee6b319730`  
		Last Modified: Tue, 31 Aug 2021 05:11:13 GMT  
		Size: 8.3 MB (8324712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba8feeb93aca0fa4ef299529124f97304595c44a5788f3d37068e45f279e719`  
		Last Modified: Fri, 17 Sep 2021 21:40:49 GMT  
		Size: 197.6 MB (197587408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:8f75bfdab450ad0d6d0648168278e7dba212a4279a2a8853fb2f893c85b4691c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:e1b69706945d30cdc5db6a3e957405a3d5cb926461ca5509b368237592c19640
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235086424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668c6dd9864c680a07a1277984a16ec7f67bdef2bd39dc27970d73c32e6ac1ce`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 05:09:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:10:54 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.12     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:10:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Tue, 31 Aug 2021 05:10:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6749e8b9c88959d91457b9b57bd8d08701cf0f82a7b72d535eab42ee6b319730`  
		Last Modified: Tue, 31 Aug 2021 05:11:13 GMT  
		Size: 8.3 MB (8324712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac7c23689bbbf0c05c6b22648b3efdb001ac588a23ab0ebda214e5317c3a851`  
		Last Modified: Tue, 31 Aug 2021 05:11:54 GMT  
		Size: 198.2 MB (198191638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
