## `debian:testing-backports`

```console
$ docker pull debian@sha256:2629e4daf047174f9293b20e9fa39c93ef5fb51ca88e6b5b4773dacd65190498
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
$ docker pull debian@sha256:78249bcc0fc70bd23219f9fe646518b6ef82c46dc41c6188e363ec9e46b4d8be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49514990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b059eebcf4c1b841d444fe4853a312f5011e7bbf95db06eea49fd560cb0a729`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:23:06 GMT
ADD file:76da3f2b01205bf031c5a2baa5619f5692978dddb951a74e40bb95b7153a58b3 in / 
# Thu, 07 Sep 2023 00:23:07 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:23:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e20a7cf08f98f931d334586c1398ad4809e12fa399f21f419a18fabc331e71b0`  
		Last Modified: Thu, 07 Sep 2023 00:29:42 GMT  
		Size: 49.5 MB (49514768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171c807390c9713d23a025de193935c88a997a7f0e8603ea06e69637de2beb0d`  
		Last Modified: Thu, 07 Sep 2023 00:29:52 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:00387a5c6b4d2f48527b8c8eed9c8ff3101f3fc50031ba53ba83f95c74c2c47a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47224258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81fed9fa7c6259c5d969add6a25214da5ce53958c8bd2f7daaf7aac414e002ef`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:49:39 GMT
ADD file:5b68c73b000630382e868620028a8146b89b70627b52744f5666dd7ac6445ed4 in / 
# Thu, 07 Sep 2023 00:49:40 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:49:43 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e2baa0d5df35e4031e8724d992e5f535848ac70b14df7b835eadbe05559f1e75`  
		Last Modified: Thu, 07 Sep 2023 00:54:24 GMT  
		Size: 47.2 MB (47224036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165056abfd1bc27dc18a6a12ac7ac61f482336956cc3e09562c2d7ac9b86720f`  
		Last Modified: Thu, 07 Sep 2023 00:54:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:329ca0c05c03a245f1ebac8695dd872af59b49f5f9b78921e13214f67ff8e9ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45010707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa6ffea3ddd747a56e6075db34cf614e74177784f134266b8fee23daf0d7d04`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:00:05 GMT
ADD file:897785df1f98741acdef541f7edc68c57cf0e3eb1698a87bd0537f8f0c654609 in / 
# Thu, 07 Sep 2023 01:00:06 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:00:09 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:de3c771b38223a129831a1a42a2e847e03db1ddec7563ae811b86bfd1c2f43b6`  
		Last Modified: Thu, 07 Sep 2023 01:06:20 GMT  
		Size: 45.0 MB (45010485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae7d463cc58a4fa1f7b931ede15a093d697e3f4032aece6f89327b06dae6b03`  
		Last Modified: Thu, 07 Sep 2023 01:06:29 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:9598abf362ebdfecd26adbe730a32f328823732206c4bbf3edd12d0973180cc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49445557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3abdcf51afa282c392d6ea615670d7fc925fd82d588cbf8bbc456506fb96fa2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:08 GMT
ADD file:69f87b30025e86f5acfb8429da721cfe92ff7a1c139df827231caa96a982a89a in / 
# Thu, 07 Sep 2023 00:41:09 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:41:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cbef94b03c52659992feffae251a9a4af30679b4e560f2f8fa84e26f3ce8140c`  
		Last Modified: Thu, 07 Sep 2023 00:46:33 GMT  
		Size: 49.4 MB (49445334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ddb18ba5259f87d88d4eb7e820e1665531edab0d313856d69867c23ebbdda1`  
		Last Modified: Thu, 07 Sep 2023 00:46:42 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:ef864ec1de996b6f9321b4b9e72d4ca9d14d26ce9511b3b7e06b4e199e812f31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50534753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13dde60631e8e192091d54be0e870b716d6eb4cbaaa03733254d0ec449eb18ac`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:22 GMT
ADD file:f44129ff1b4d8fbddb60f8ebcbc4c63bed1adc3894e52e8bc9bce31e1d82928b in / 
# Thu, 07 Sep 2023 00:41:23 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:41:26 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ea53a78b4b944bc37f70197e4395139b6adb07971f3842a419cabc2f23c82377`  
		Last Modified: Thu, 07 Sep 2023 00:48:20 GMT  
		Size: 50.5 MB (50534533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33697a5da812002bdc5d5adfbc6d81af4a01d0f41da18dd0a69d21b58bb07ef7`  
		Last Modified: Thu, 07 Sep 2023 00:48:29 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:d7f9d0c193b1243296933d77e46368c351f748ac9f25bdf6004837362feab1d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49357714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9446609c53bc9ac46867b5b2fc2d4ad8126a269f7d25c60226bf806f8f8aeaff`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:14:39 GMT
ADD file:c6067d8729951df2c664bbd3ecc7487e82dae7e0d0b3868624030b3c5f73fb01 in / 
# Thu, 07 Sep 2023 01:14:45 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:14:57 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f2b2f343fec7d418a01e7f9a18923cec3fd789ce3a8f4f2e038ab44322805015`  
		Last Modified: Thu, 07 Sep 2023 01:25:59 GMT  
		Size: 49.4 MB (49357489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1616c4fbbe4d180cf5e90580dd36efd3cea4840e29e85e2b27da63f3beb488`  
		Last Modified: Thu, 07 Sep 2023 01:26:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:e8f125538ff43b4de7b91d687865279e76824d9940b600af435f768abeae1963
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53456239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d39562874b85d2a07c5ce80cbb507fd4a407c964594d73d6a0ecc9557f9d2ce6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:13 GMT
ADD file:69350b5a5e94c4a556e56f265533a04f8035ebc4bd834bec57b98a246ee547a6 in / 
# Thu, 07 Sep 2023 00:20:18 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:20:25 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7c3a2b005dd31b7bb84d8511ccf37b021f6db4066b3d2136dbdc778ea24e8eac`  
		Last Modified: Thu, 07 Sep 2023 00:27:03 GMT  
		Size: 53.5 MB (53456014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920e70ede045e655cd02d6cfdbb984e2f1c4895f84cb4329cf7f50885abbdc1c`  
		Last Modified: Thu, 07 Sep 2023 00:27:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:82cc9e895cc237b0451d7862badf4992d13a8415673f32fe4f76429972e86de5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48574006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d62c03925f6443a52db33356b94e48c4a0a70bf4c21a1d4ff2361345e2c825`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:46:52 GMT
ADD file:abcf51b81cd6f9cfc93b9963d223d2066f6e087d383af2edcf8f9a577dc23efd in / 
# Thu, 07 Sep 2023 00:46:56 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:47:03 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ee1a4ae1256a1fd777550db8f08b55a9e6e2b2d07e77c364c53343f9f594e95e`  
		Last Modified: Thu, 07 Sep 2023 00:51:44 GMT  
		Size: 48.6 MB (48573786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f758147df3f60775dd12108aace8c6bc463e7b3ca350fd7f3d413dd3041203e3`  
		Last Modified: Thu, 07 Sep 2023 00:51:55 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
