## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:07acca196700023d9a3df68b06e48b47841273080ddd26e3f29e18d7ec41c328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:f83f7ae0e60c46fdee615b51787f40696dcacb14ca5997ae95881942616ca0e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45379897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e141a226973527e94291dea4c007b2dfdd721849504eec32b7c59086b7b5cf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:22 GMT
ADD file:fcbde341692fd5ac6db8f6554cd89ab8fe21895260d60e38afb0d9142efc3472 in / 
# Tue, 28 Sep 2021 01:23:23 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:23:27 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0aa0e512c4e85920af94ae0e640cb6d021269c4539e85acdc851d2661fa290a3`  
		Last Modified: Tue, 28 Sep 2021 01:30:05 GMT  
		Size: 45.4 MB (45379669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9939c6e7518f126cfe380a5831cacc4c6aaf24ab33d0f55543f94c2a50a09c8f`  
		Last Modified: Tue, 28 Sep 2021 01:30:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:59a76b9e89a57a5501247b8282a9820f756ca551600fd9594212de04ef23d86b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44092158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648cbe3ce363595d49c2ef3a90cd6f944a2911d7ecca1b8120cf55af9b410351`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:52:12 GMT
ADD file:ed807aa927e2c5198c9c83b347c43cce4845e8a34aad170055111c06026df75f in / 
# Tue, 28 Sep 2021 01:52:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:52:27 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:be7e9924def62c224fa6d66bfb326fefd41aa4e7c23dc34e14be6897c6aa1421`  
		Last Modified: Tue, 28 Sep 2021 02:08:51 GMT  
		Size: 44.1 MB (44091930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439db44cb40326b1cbf043377fa189fc0fefce38a941f5019e87ba1143f5c9d1`  
		Last Modified: Tue, 28 Sep 2021 02:09:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:3e80a372ff7dea91ffec109a540b7cf338210c1ec98572fa0b5aacc213700a9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42119627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5366dea5d730a6345706b1a2229dc3019154b495297b28f2ce1fc6cb1812b27`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:04:43 GMT
ADD file:cf7d38d2923bab1c84afc083d81241caa464a84caef47a9643c0f14a6c9ac627 in / 
# Thu, 30 Sep 2021 18:04:44 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 18:04:56 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:791eee32c1e22ba9dee78da6f5a2dc709c7a4c1472330db90cb7c3acbbbe2824`  
		Last Modified: Thu, 30 Sep 2021 18:21:36 GMT  
		Size: 42.1 MB (42119399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21da7d1597d13f68694561c3b4a117a649edfe8af79e8c9fce5a835c568b983`  
		Last Modified: Thu, 30 Sep 2021 18:21:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:8a6e08e33e82d8e6777db3e7a796dec770ef5d8decb7d8f6242f65edb80bdc6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43177105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b3e1db8bed1bee46f899a94859cf4e1c72818db4f97c209198bfed083c4a5d0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:25 GMT
ADD file:cbde3caed866b5349b77a93d9204d80a59481520908c71a158b419d01eb815f3 in / 
# Tue, 28 Sep 2021 01:41:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:41:31 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ad8e8d672b1bc4b27cb72d3e50bc21f58f793c9296db796a07bfdb4c1252afdb`  
		Last Modified: Tue, 28 Sep 2021 01:49:45 GMT  
		Size: 43.2 MB (43176880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91e5956907c8d8fb7bd96101bf49308dea484c3a86f71d14ca5a585e55383a8`  
		Last Modified: Tue, 28 Sep 2021 01:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:93e498da1adb30b8e85a61d4a2c141a0679e3248f3c8e7b29afaae9ae520ecc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46097299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac80140beee433ad3e7726d5eecfbf89e91341a25ea441b27b09b7b5eac2eaaa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:06 GMT
ADD file:c4032a14e7d48732f044e7e8b08df458955c11dc14cc5a681f2a69845f94f637 in / 
# Tue, 28 Sep 2021 01:41:07 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:41:14 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d6c5ec7f7724559a7bdb28746c7db50b757d3865ea977b871b843ddc779a9913`  
		Last Modified: Tue, 28 Sep 2021 01:50:33 GMT  
		Size: 46.1 MB (46097074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfa194160263f1475588e2e555e08d368b70b0ed9bcd571729a63ec8f520e78`  
		Last Modified: Tue, 28 Sep 2021 01:50:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
