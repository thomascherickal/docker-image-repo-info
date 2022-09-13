## `debian:testing-backports`

```console
$ docker pull debian@sha256:7a983cf2fc60d14329f5903ad64a444e7d7317b7bad73f859e8a46bd3b735182
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:a8a2693471bcb4a925dd51a5928d97100ef656057e76432fd97c8361f8d7d678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52983807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bac03a2da30bd3a7c55822486a10692ea269b259704da8bb09f2cfb8f7e7d30`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:57:53 GMT
ADD file:eab284d675ebe571774a405e2773ad309e7992babbcee7da7353360819720c79 in / 
# Tue, 13 Sep 2022 00:57:53 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:57:57 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d81669dcf8a7f2d2d267e74db5db6aea7ca548ce5117280e5e7e6c5abeb0b222`  
		Last Modified: Tue, 13 Sep 2022 01:03:18 GMT  
		Size: 53.0 MB (52983583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764c8e3fa1332ea3bbf84a38f2f810d7008e333d5ca19f6731caaa02e623e14a`  
		Last Modified: Tue, 13 Sep 2022 01:03:27 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:673acecf7fd9ee70432da3d1a97d4e5d5bdd248cd4c411e19b04e2121426a0f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52122767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3e2f643a20f57871cc36323e15936b7fec936ed8e5e01342f3457f07cc11cc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:55:28 GMT
ADD file:8a5271643c4e7a06124d169d69237ff785175fa358687fe70569fbdb6019b4d6 in / 
# Tue, 13 Sep 2022 00:55:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:55:36 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:81baa9e2df41ce6d109b1642aa8ac546cb2767115f02971dae2b8b49647e82d5`  
		Last Modified: Tue, 13 Sep 2022 01:03:33 GMT  
		Size: 52.1 MB (52122545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe87e8cdbbf80a1c29de79f722c073671d0c9ccb7cb15b3d7551311eaa71d63d`  
		Last Modified: Tue, 13 Sep 2022 01:03:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:5e8ae8ef450d8760d94d4bb97f4649fe79ebed6eb5680c83b7d1c65131068047
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49555336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30de06ac825bcda6eb595a6acc050957e57b394ca449c08dbcbdb4eec4d95259`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:45:36 GMT
ADD file:3a189fabd18a25649202e19fada53edc913c92c596b1234c0936cc621226692e in / 
# Tue, 23 Aug 2022 01:45:37 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:45:42 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7e1855cae120824d8b8b204aac8c76fd1d169615db57ced1ccd3cf0ca1e6368f`  
		Last Modified: Tue, 23 Aug 2022 01:53:32 GMT  
		Size: 49.6 MB (49555114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a352c50971ca235c107977bdd43496a7770bc4e3690a32031688d878d16bba5e`  
		Last Modified: Tue, 23 Aug 2022 01:53:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:160d736f2ef7e330b8078c43e0036e4a203c319013afbc317cd03542d5dd48d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53117767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e067891fe7465a1ea278d099a68ef8ce0b9a5cb27174a37c72a7a868be6b66fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:54:16 GMT
ADD file:5feea900f1cb717b9ea13acbf6f2d7be123e4b83e550e0121c44dcffeeca226e in / 
# Tue, 23 Aug 2022 01:54:17 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:54:23 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2d7e20893a70b321d1c8a4b612d35a510efd826cfb1d665534f9dd1cd15eb956`  
		Last Modified: Tue, 23 Aug 2022 02:01:03 GMT  
		Size: 53.1 MB (53117542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0dec2ba65d5fc88472d7857f5d7c1fb8aecaae8d2e2451c51afa7b10008238d`  
		Last Modified: Tue, 23 Aug 2022 02:01:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:e47ffefe9d77f96dc1368d77eb1c30deea4eb35906ca103e2af9dd733383d447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54097252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13dce6c9081c8b1e766c46f2fafe5d145f6d1d5d29bdaf40eadfa04bf4fa95c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:04:28 GMT
ADD file:364ffb1c2691887de798917d234954fb0eb7c72137489822bd12bd6194cfdec1 in / 
# Tue, 23 Aug 2022 01:04:29 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:04:35 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:06240d8d46075ea69ca3a286305ca352bcd6ccf14658ebad53126670dbd52354`  
		Last Modified: Tue, 23 Aug 2022 01:11:41 GMT  
		Size: 54.1 MB (54097027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d33488b435129476641a474c0ff40d216bc3ed0cc765db6615bc700be026931`  
		Last Modified: Tue, 23 Aug 2022 01:11:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:00a0b943ca8239fa64cf723d4582429321a5972222072cbe7405fa03d2c14cc6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53119599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3e037922a85e4a5eacf097d342491014b01d0d0920e6160ea6e286179cd7e93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:14:12 GMT
ADD file:f3e9e580221d3e94f0fb61e58fcbf318bc042add830bcdd71dd0983d138c3b0a in / 
# Tue, 23 Aug 2022 00:14:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:14:31 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d67983489079eeb3b8ecef40d659bc0761c151e192dc6a219e80b494d3ef1685`  
		Last Modified: Tue, 23 Aug 2022 00:22:47 GMT  
		Size: 53.1 MB (53119374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54e598f2f73878c653030f8a3e0d9ad2e90e0e2b6ac805e5f30e37094a4c9fc`  
		Last Modified: Tue, 23 Aug 2022 00:22:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:51c5ee4b9c7bf2e3ac8a739eb211125de1f22e01272ec1fad62572e7d82bab26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57290098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0a218f72898ab59522e72852fce60592021339abc05f8c2a4cc80bb543fdba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:26:21 GMT
ADD file:35daf34d4b9f7c9f63a3058d75300b029515bed52adbc8b7a87a5c09a93019fe in / 
# Tue, 23 Aug 2022 01:26:24 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:26:30 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0fcef4ef26ce0a4602ae0238ad72b59e19d865c22413f6b751fbedb72875c424`  
		Last Modified: Tue, 23 Aug 2022 01:32:45 GMT  
		Size: 57.3 MB (57289874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e71cff04e78161bf3d173a360cb86ebe0758b75c0268fbbfff029a9583420a`  
		Last Modified: Tue, 23 Aug 2022 01:32:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:3b341ce3791311654c0a2ebd7a58942b5d941bda7871d7b6967faa100833e760
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51793976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea9e4072be11a39a2b0f77386261842200bc48f92780b3e7e7f299d1975c850`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:49:12 GMT
ADD file:66f44d68f978fe3b9abd2ff209f09412b83ce5518ee28f77b480bea6ca41fd47 in / 
# Tue, 13 Sep 2022 00:49:15 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:49:22 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:72862deaf676befb9cc285a47088524f14e8d520d3f66531de063d495dd63aa3`  
		Last Modified: Tue, 13 Sep 2022 00:53:48 GMT  
		Size: 51.8 MB (51793754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9531bdc635a5ed6091b2356b0c90d77a2fe92dd1476c9b313803b3bfdb0416b5`  
		Last Modified: Tue, 13 Sep 2022 00:53:56 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
