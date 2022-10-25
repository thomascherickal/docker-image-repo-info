## `debian:testing-backports`

```console
$ docker pull debian@sha256:c3ed851e441808019f25de691be0cf4fce152e5761856a72832a734f2270036b
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
$ docker pull debian@sha256:6a970621b872d3f4a145618bb6ee8148fad3562fb1932c877a564aa20bd11f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51261981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c1469fbfb53fc9d150b77ba9471f706c265e1029fb957545e605517a39cb1bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:45:19 GMT
ADD file:7b3c3912d73330bfbb6eb18f8cba6491e0c4b2be59bc6b846a4a0cde39b1ad27 in / 
# Tue, 25 Oct 2022 01:45:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:45:22 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ebbe46658ae1eddd748e3222cbc9dd7109f9fd7f279a4b2f9d6a32d0a58b4c16`  
		Last Modified: Tue, 25 Oct 2022 01:50:50 GMT  
		Size: 51.3 MB (51261759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5900a9fa43b590cadc60d1cdb3d921ad1e9b82a29f91b032ac710e43a116bf61`  
		Last Modified: Tue, 25 Oct 2022 01:51:01 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:1778ca32183d5881d8aa0f1b14f22bf6e3bd9d8d49702e440f2a30c73227bee8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50178619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a401b1447f848a332c76f02a19047c6f07702e0775dd5e0061f98ff630b19a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:48 GMT
ADD file:1e3e886911bc454265fc5b72f45b62c2a9994f7d6cfdac259818f33bccf61376 in / 
# Tue, 25 Oct 2022 03:07:48 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:07:54 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9efe593dedf724c710365cbc5d88f301354b892e3302dfae20a8ba15a34cd967`  
		Last Modified: Tue, 25 Oct 2022 03:13:46 GMT  
		Size: 50.2 MB (50178398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae95d97b9f5f6710a27edd7749b65f3450ab8a45b4a197861f9ebbdb53d2b27a`  
		Last Modified: Tue, 25 Oct 2022 03:13:59 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:1b0886b03411d3adc54c81e4aad6180b4e4c48d325cbe682a473db12de9b8101
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47997697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a80d27f16f124dcfb594f69e2107ce6902e26558f3f9b90edffd9fc49b02438`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:16:26 GMT
ADD file:235cdd454d0a7a1ea304c9a65b0ec59ccb6dab2f75a7fd35928604d4ec1d10b0 in / 
# Tue, 25 Oct 2022 03:16:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:16:34 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d3df850c9646ef510d7e6c53aeb7bc9e01b669a7052a73eddad2a14122637a69`  
		Last Modified: Tue, 25 Oct 2022 03:24:44 GMT  
		Size: 48.0 MB (47997475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbd30313d7b4c3925c94478eab03e8b4a32857082598ffe2ff033c9e5880f64`  
		Last Modified: Tue, 25 Oct 2022 03:24:56 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:5353c8db079d868d6c96b2f932e94ec1f438924ca13cec37c51e649e295e3f42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52980621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bf2a79b62dfc1042874a53f23fd6aa0dc233299d1bf91c44cd4d29ab4024271`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:46:34 GMT
ADD file:d8a562b059284e25b26f8bb851509a38bf96a6ca745d5f220f0c50c5a2791d8b in / 
# Tue, 04 Oct 2022 23:46:35 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:46:41 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:76f19dcc19c7ebaa09b68b24e05232d803279cd70b2bfaf1b9b883b76e3a5147`  
		Last Modified: Tue, 04 Oct 2022 23:53:31 GMT  
		Size: 53.0 MB (52980396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd605a54635e20f4be7cf40fa4e1797422e1125243d99991e456e9f2d39e0773`  
		Last Modified: Tue, 04 Oct 2022 23:53:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:d3b32bda9c133d55cd448dbbb613d04481342a9858a38d5af729b44d83ba025b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52224997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ecfae015780c931559bc1e81505f5c3b0b5656b27a0ed1f48839f40e3b9a33a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:24:25 GMT
ADD file:ef956fbaabcf0c2b4f6d6b214e986b76cfcf0e05720e163fd7c000c2aaafcfbe in / 
# Tue, 25 Oct 2022 02:24:25 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:24:31 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:550818b5edd6670d29cb073384731cb9a2aafc2c09d120872aaa6860e67140e0`  
		Last Modified: Tue, 25 Oct 2022 02:31:36 GMT  
		Size: 52.2 MB (52224775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51aeb1cbf270a29df7f74ef696404d91b2865e7e46e09d2f052061b98cfd24e`  
		Last Modified: Tue, 25 Oct 2022 02:31:47 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3ae2b45d3dff79ed6a64eb192df8ba79cc7550738630ca6941ccf89f7c1a9104
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52967232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32cb1055829163e06706f6b57c6d3b1d9101f2ac06d7ff9b7f65eba069f1b4c8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:18 GMT
ADD file:4ff9efc8f665301da37db96a22470e284e0d7d47891026e9194a2c7709508b8b in / 
# Wed, 05 Oct 2022 00:13:22 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:13:34 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1454aae498a3aa762b432635fb671c490406bf5e6ec9ca85aac661eab19b190c`  
		Last Modified: Wed, 05 Oct 2022 00:21:50 GMT  
		Size: 53.0 MB (52967007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78aa87929f162f1fa06c0dd2992068d599de529c3636920fa06651e4215a8bb`  
		Last Modified: Wed, 05 Oct 2022 00:22:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:7ee3fe003c021425348daeccf242502c1e9ca531a1b7599664a2823946e56121
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.3 MB (55338954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f07a04ffb30db62f97b9948132c41c34cde8bcbe0858c8537ab3a77f4dcaf889`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:15:17 GMT
ADD file:eb3294b440b1de7e5e420328a146136657392ed0568fcc54a574e171e31558a1 in / 
# Tue, 25 Oct 2022 03:15:20 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:15:25 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e78937113e3c6d6902831ab5c7cb1ac7b54dd956b0a882adb2b81160f0cd0833`  
		Last Modified: Tue, 25 Oct 2022 03:21:41 GMT  
		Size: 55.3 MB (55338729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4b811f6057e845be5e7ea7cc69391617926f6d6ba7e24914e26685e9cc4851`  
		Last Modified: Tue, 25 Oct 2022 03:21:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:5fd4c1b9f6e6d984c924a1d50e7b4cdf6d02e618ec7062c857385dc1651635f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49578696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6accc7312c47a1a17e6f0584601ac09ad6965a90a2cb7a6c35a4f245bd59992`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:15:47 GMT
ADD file:9093ef5b03ab758cca4be205f4332f6e9ef617d8bed9b952af0073c9eff5ff4f in / 
# Tue, 25 Oct 2022 01:15:50 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:15:56 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:61dde8995e51d73ce3f12dd6592eb9f349f7c17628780fae6f2693134ed30c40`  
		Last Modified: Tue, 25 Oct 2022 01:20:12 GMT  
		Size: 49.6 MB (49578473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d20602ff47fd95f7ec3768dc16ca9e4df59cd2e0876844a3e1a7fe7513ae5`  
		Last Modified: Tue, 25 Oct 2022 01:20:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
