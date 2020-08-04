## `debian:stretch-backports`

```console
$ docker pull debian@sha256:110d18f90255e39a6eac2c3a17b4bbd137fb5a43499bb523f9da20a46fb0c9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:03ee996b9719ea682a12b5385c3a93c103a9c93d41cdd44ed65fbb19131b8b11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45369896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52a14ebc3ae213213285ef6527255bf8a067758959c810d1fe60b05636f041e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:06:48 GMT
ADD file:f98fe3d719ea765cb59da025d506d0bbd6db7a842b6b63c58c8d4d65b51bdb1f in / 
# Wed, 22 Jul 2020 02:06:48 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:06:54 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7e6d8ed603557d9bf077a9ace4ee506501970a4938b9a704f040ad15f22bd4e8`  
		Last Modified: Wed, 22 Jul 2020 02:12:13 GMT  
		Size: 45.4 MB (45369674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6954bf97a51499d1fb263895c04fec70a7aeab331825e2306b94eeedf7af4e3`  
		Last Modified: Wed, 22 Jul 2020 02:12:18 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:e3decd61012b7c7e4f9158ef96cff7a029f09b2472c392794ceed93d6a91c0b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44081446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecfa578e927bc15ed6fadd3e88711103ae438cb9cef42b1e27de4f13ea0efaf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:23:56 GMT
ADD file:c82979276574ae052b356c92955110dfb283d33659ea097871176d1a62ed98ff in / 
# Tue, 04 Aug 2020 03:24:04 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:24:45 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8653f8cd9e4c7c5ecd1cd925507522d43ec49dea7127050e56d71d3447f39292`  
		Last Modified: Tue, 04 Aug 2020 03:38:23 GMT  
		Size: 44.1 MB (44081220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2689e285e5451089092bd3fa4d0e551872d5e73e944ee6bd67d3517727611fff`  
		Last Modified: Tue, 04 Aug 2020 03:38:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:862bd09b3d2ab23b347463a174e5be437a7614b6f77d8d40e7591998196b6de0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42111607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92cf524d667492d23aa8823a53b921dd1fb1a215e87fa8e2ffaf4830959517f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:04 GMT
ADD file:0ba6f3203fb10e66124d03088d234e92fc908c572ec7eed268e866623a383a7d in / 
# Tue, 04 Aug 2020 05:01:07 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:01:16 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:323178d00ec2c5eb5ffb9cb696a52eaf8683dcf2eb605c742da2953556f06e37`  
		Last Modified: Tue, 04 Aug 2020 05:08:40 GMT  
		Size: 42.1 MB (42111382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6f1c8ddbe824bb2a9ce7f0ad328d89038d5b288e289e94de3137f65e458387`  
		Last Modified: Tue, 04 Aug 2020 05:08:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6ec1d3f27e4e583894448c96bcc55cbfe80accf013ea263a88ed97c7619466b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43169630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f501116ecd90063591421ddd06a837e4eb32891e909939a383f1c25e3ffe4993`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:43:42 GMT
ADD file:9c5c9df9952cb51291333837bdb462bbdf9f157e91e616f1e3fb8d2fcb1a1983 in / 
# Wed, 22 Jul 2020 00:43:45 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:43:54 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ad4de4f68e9c2c0f5e5e62d379d936bb88ce467505ed002fb1e10c434fefe90c`  
		Last Modified: Wed, 22 Jul 2020 00:49:52 GMT  
		Size: 43.2 MB (43169407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4167ee6e6df70cf9862116173bbe4240fa5fdfaa129a95bb5d758f8ad1e78d06`  
		Last Modified: Wed, 22 Jul 2020 00:50:04 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:cdc642b99bbc33cb48875fedc3f468d9aca417356721bcc8c508911e72e4af8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46087001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b446a1d9ca14dd448941b68bc2ebff0a75dafc2bea9a647e8d59c0d33747c50b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:39:59 GMT
ADD file:af30f23f89d9bbdd6ad60199f3d978a5e426835c6138e0c76a3453680945a121 in / 
# Tue, 04 Aug 2020 03:39:59 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:40:04 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:36eaaca1a8d1677d2d2aa93f595d838e71ccbe4254f548ff566f97e8d555df1c`  
		Last Modified: Tue, 04 Aug 2020 03:45:28 GMT  
		Size: 46.1 MB (46086777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4d2c2badd53cd2fe3de49bcd7e2c043577b8b1da44ed66eab8b6439e70ae29`  
		Last Modified: Tue, 04 Aug 2020 03:45:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
