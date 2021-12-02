## `debian:stretch-backports`

```console
$ docker pull debian@sha256:dc6397fc28bd2cdc28bb4b12a38ee800c4b544734fad9be04a262d3b05806a4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:912707655edc34a996abf23b02c6cf8f1b0d3dd01a74aef2204536649507a0b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45381620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4cb5795da7d198a15ff0abd4faf52f45d19bf660f22a799b3fad07d51c7cce`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:50:23 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b8f63add2d388d573c5011be32144ff0513f6164b6453b18d4933a6912a6c3`  
		Last Modified: Thu, 02 Dec 2021 02:57:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:ece7cf4b91070ba3b04693fc7bbfd107ee099bd1718e72c00f2a14bc62d001a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44091928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:359c68ae3547dfa04efad63fe174b02e6a29c2fe0ac289f3c83f1d91cfc65199`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:57:10 GMT
ADD file:a2c8513298faf10e5f3b6a070d46acca10a79d9dd50302c55604df9fecb26b2a in / 
# Thu, 02 Dec 2021 02:57:11 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:57:32 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8bd29eaaacb1755f329ce7db7d99eb138c06aad3ab1bb6e8c3b0017596eb1f69`  
		Last Modified: Thu, 02 Dec 2021 03:15:21 GMT  
		Size: 44.1 MB (44091702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b03fae5da188a9bf2a6e253f5cc7d306d61f68758d531978c965b8438500fa`  
		Last Modified: Thu, 02 Dec 2021 03:15:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:e0ddf32aad03141f45feac62807d0f9360eaaeb7aa74a09a9eff57db77b03fdd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42116980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a01f3136c31a5424c78359239e05e16144076238965f03272f867cda103496`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:10:39 GMT
ADD file:1f947e5a3f8b1da292340501298edf2b879183aea9e90531f21c2b22500e79ad in / 
# Thu, 02 Dec 2021 09:10:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:10:55 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fdee104a33d14b2fdafeeaca15f0252d32280549d3cdc971244796c6e69ad0d3`  
		Last Modified: Thu, 02 Dec 2021 09:27:53 GMT  
		Size: 42.1 MB (42116754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42e8133d120da8f5bcebc8e97cc8c092a59c80be12154a677485b5774c0ace`  
		Last Modified: Thu, 02 Dec 2021 09:28:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:d1380ae0b7794d8be981f098e4210301b44857857a0b168465ddfa536ad2a24d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43173907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759d446565921abeb43b25e7193d85f562a7965067c5eaeb2e6bd0b1333df646`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:10:09 GMT
ADD file:7be59c7e3b187d010c0e8625e45324f421a21518258e6bd35bab6e0e86c9494c in / 
# Thu, 02 Dec 2021 08:10:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:10:16 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6965f119641a6f16b55da01b7c12884960366228a181268b0bf7d0b7d50b2336`  
		Last Modified: Thu, 02 Dec 2021 08:44:30 GMT  
		Size: 43.2 MB (43173684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d9c57bb5f44e023ef68089669db23c0b71c8749174eec5e5d6f0837e5b8e66`  
		Last Modified: Thu, 02 Dec 2021 08:44:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:a1c3d61a8000e88b8b4d2cc5c5c32c0b78b2fdc849099ae2b8c85dbc6458b792
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46098115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb2b23f17367cf644daa8e2392a4ff6535b9974542ad4487a4eefc187378030a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:42:27 GMT
ADD file:7211d8cf4427f9effab1662b9a54e89548974bde8e4162ccd44fddbc57024912 in / 
# Thu, 02 Dec 2021 02:42:27 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:42:34 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8450ec7364298e2205fbbb540c3ebcbfe46324826539d90ea2e28eeec0bec114`  
		Last Modified: Thu, 02 Dec 2021 02:52:39 GMT  
		Size: 46.1 MB (46097889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4360cabbf8d8fb2928f24bf7d65bb27307718422d45bf291e75f8cfaed96d2af`  
		Last Modified: Thu, 02 Dec 2021 02:52:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
