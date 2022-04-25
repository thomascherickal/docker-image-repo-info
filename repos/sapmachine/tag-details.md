<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `sapmachine`

-	[`sapmachine:11`](#sapmachine11)
-	[`sapmachine:11.0.15`](#sapmachine11015)
-	[`sapmachine:17`](#sapmachine17)
-	[`sapmachine:17.0.3`](#sapmachine1703)
-	[`sapmachine:18`](#sapmachine18)
-	[`sapmachine:18.0.1`](#sapmachine1801)
-	[`sapmachine:latest`](#sapmachinelatest)
-	[`sapmachine:lts`](#sapmachinelts)

## `sapmachine:11`

```console
$ docker pull sapmachine@sha256:322e280276e6fe9894ca0f54065e44cc23922ef94a7a2d9a12eee48713443288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:11` - linux; amd64

```console
$ docker pull sapmachine@sha256:88bccd02a278861ff0459d1a834f5dd68ab063f0f9adea50026993e12b63801c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234595123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41c9ee003bc685535120d63b339d2cf51a9aa8fcb09990e6ba8b1e780111edb`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:56:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:56:48 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.14.1     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:56:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Fri, 22 Apr 2022 03:56:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff95dd8c1098ae71dc81b04acfd2d3daf018131b8193361347566dac0fe084d`  
		Last Modified: Fri, 22 Apr 2022 03:58:18 GMT  
		Size: 8.3 MB (8317757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8131bb11c982e87bef4f98706e0137f0fc623acfeac513228dcbbe2b391f67d`  
		Last Modified: Fri, 22 Apr 2022 03:58:32 GMT  
		Size: 197.7 MB (197711368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:11.0.15`

```console
$ docker pull sapmachine@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `sapmachine:17`

```console
$ docker pull sapmachine@sha256:c5fd3687e68b521238e3fdf8a58cba3c0c4c5b25861a27da33a811852ddf6581
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:17` - linux; amd64

```console
$ docker pull sapmachine@sha256:eb7659ab20223f149f5f7df29ca8d570b326804aca40ebc3cf0e6f57139930eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234531401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7290c4fedecdd8d519986ae0b14d2c10a813c7d9afd05e31e5c3b0a7670e0a65`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:56:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:00 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Fri, 22 Apr 2022 03:58:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff95dd8c1098ae71dc81b04acfd2d3daf018131b8193361347566dac0fe084d`  
		Last Modified: Fri, 22 Apr 2022 03:58:18 GMT  
		Size: 8.3 MB (8317757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7540cfea05a9f68d05978eb8265628437464b58e87584361960143dc99b633`  
		Last Modified: Fri, 22 Apr 2022 03:59:22 GMT  
		Size: 197.6 MB (197647646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:17.0.3`

```console
$ docker pull sapmachine@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `sapmachine:18`

```console
$ docker pull sapmachine@sha256:a9e6f4c0f19f78bae4dbbe812e47b53aeb1bba52f40243dc065eb3d0a21180c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:18` - linux; amd64

```console
$ docker pull sapmachine@sha256:bc8c48e8467d26039ec71be83c872071d6a37ead470e2905febc6c60aa495074
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294323b5ac41eaae62841658681b197f1efbd6c4a2e21191511b2a9aa1a8477c`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:56:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:57:28 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-18-jdk=18     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:57:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-18
# Fri, 22 Apr 2022 03:57:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb3497eded1e3eecf8f2698c510b36e1d91b42337d37bd2dc6e64189ae252b6`  
		Last Modified: Fri, 22 Apr 2022 03:58:43 GMT  
		Size: 7.9 MB (7925521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645b9cce910a26164717a8f068f96c514f692f6b63acb51fd49371a87f3b6922`  
		Last Modified: Fri, 22 Apr 2022 03:58:57 GMT  
		Size: 198.7 MB (198678485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:18.0.1`

```console
$ docker pull sapmachine@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:a9e6f4c0f19f78bae4dbbe812e47b53aeb1bba52f40243dc065eb3d0a21180c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:bc8c48e8467d26039ec71be83c872071d6a37ead470e2905febc6c60aa495074
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294323b5ac41eaae62841658681b197f1efbd6c4a2e21191511b2a9aa1a8477c`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:56:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:57:28 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-18-jdk=18     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:57:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-18
# Fri, 22 Apr 2022 03:57:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb3497eded1e3eecf8f2698c510b36e1d91b42337d37bd2dc6e64189ae252b6`  
		Last Modified: Fri, 22 Apr 2022 03:58:43 GMT  
		Size: 7.9 MB (7925521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645b9cce910a26164717a8f068f96c514f692f6b63acb51fd49371a87f3b6922`  
		Last Modified: Fri, 22 Apr 2022 03:58:57 GMT  
		Size: 198.7 MB (198678485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:c5fd3687e68b521238e3fdf8a58cba3c0c4c5b25861a27da33a811852ddf6581
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:eb7659ab20223f149f5f7df29ca8d570b326804aca40ebc3cf0e6f57139930eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234531401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7290c4fedecdd8d519986ae0b14d2c10a813c7d9afd05e31e5c3b0a7670e0a65`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:56:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:00 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Fri, 22 Apr 2022 03:58:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff95dd8c1098ae71dc81b04acfd2d3daf018131b8193361347566dac0fe084d`  
		Last Modified: Fri, 22 Apr 2022 03:58:18 GMT  
		Size: 8.3 MB (8317757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7540cfea05a9f68d05978eb8265628437464b58e87584361960143dc99b633`  
		Last Modified: Fri, 22 Apr 2022 03:59:22 GMT  
		Size: 197.6 MB (197647646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
