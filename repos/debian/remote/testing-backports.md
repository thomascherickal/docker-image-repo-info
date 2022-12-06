## `debian:testing-backports`

```console
$ docker pull debian@sha256:866d5af1e3a2031887b43662b0068a30bf9fc9fc2a17e525671f994e2d190674
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
$ docker pull debian@sha256:b0626911341af673cd48c323315568ce54c9a07b56052110ee2d8cb0ff99c4f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50260677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e31ec8e2cbe77d1ecaff494af9cce303fe8e6b01816c7ad109fbf6625e74792f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:22:37 GMT
ADD file:ddf2bf5e38ad0d3b2eb29a4cdde4958105c600905abfa6f75edff8c283ee4845 in / 
# Tue, 06 Dec 2022 01:22:37 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:22:40 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d53f8c84bd3a16946373258506e00b7e6d1d9f8087dfe492e8df85096ee760b8`  
		Last Modified: Tue, 06 Dec 2022 01:27:41 GMT  
		Size: 50.3 MB (50260456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c8213a9a8c0d01ee6dfc74a3440bd569a83e74156b5acd08be9d83fde33264`  
		Last Modified: Tue, 06 Dec 2022 01:27:49 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:e5c44ca5cb107b4b3708df421e3b9e4900ae27d7ef4196a75fd8d75107f5eeb0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49227559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f8dc2deedbdc7a8b1c52a01a79ba2c38dcc15762ef51d2d16d308bb1b63ca43`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:50:34 GMT
ADD file:5c5abb51f9c145fc0c02fadf24217a98412dac57fb4ada902b98a1b13269d327 in / 
# Tue, 06 Dec 2022 01:50:35 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:50:42 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:443ce2c1c11b7f9d06683961973d66426be4193cb5a87ce723c3b032aa2463ba`  
		Last Modified: Tue, 06 Dec 2022 01:56:17 GMT  
		Size: 49.2 MB (49227335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0333d45f3cb8da5794afc560c5fb31243ba1a7ef937d094ec1704852a9e803e7`  
		Last Modified: Tue, 06 Dec 2022 01:56:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:f285adce145942231ff459610842f5df620f898e1d285ba6f16c340a6c9f42b1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47047258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47b4fd95c1a469301013347c99a47186c8c5d8b92623535298ad638e36fe51c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:01:18 GMT
ADD file:63250ad0a664c24007c6acd3342b5991116f41d46a00b8bf6934ea1d884cff35 in / 
# Tue, 06 Dec 2022 01:01:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:01:25 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c0308e1b3f3cca232bda5f7d74eb8bc123982e374bd8d8dabe10a8a762254765`  
		Last Modified: Tue, 06 Dec 2022 01:09:11 GMT  
		Size: 47.0 MB (47047036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f781b553b918d921e344b69f4a71c2cd7bfad90596f6069db09a97dd073d4489`  
		Last Modified: Tue, 06 Dec 2022 01:09:22 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6f7989420c91ad566d704fe52786b3492f632eec0921ec85db83c4c6280a55ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50307953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4381934050e2de1ddfbf012d83815e3b1dc4e09b7207782f8ffe28ecc826a036`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:41:30 GMT
ADD file:11bd3a64e9c2bd767695d492043ab5c0f9d2e1ad8060a75c42c3112ce2209ad4 in / 
# Tue, 06 Dec 2022 01:41:30 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:41:33 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:48a13e60e721652f48449ee235d2b585637c9f1a9af5d86f4ae5c9a04d7b9869`  
		Last Modified: Tue, 06 Dec 2022 01:46:17 GMT  
		Size: 50.3 MB (50307728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f0c4c8c272f14311f2b0c6f822291ae28b25c29dbcea5479d37dfc0e4b6462`  
		Last Modified: Tue, 06 Dec 2022 01:46:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:fe09972e1c5be24fb442498840e08aca952c829527f6afae380c89645a7a645a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51301787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61a448a5546030c7cf1d58ca8e660fc5f103b2ca9cf90f1ae515e3fabcb59de1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:41:55 GMT
ADD file:746f29956fe3ee5ee0862558029a5ffd38b9557c764ddf9587138c30ce2c7f49 in / 
# Tue, 06 Dec 2022 01:41:56 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:42:01 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bdecf1147c64128a9d335f70eaa3d8b12e3b7942bcf3033f1aa4ee830a3ac797`  
		Last Modified: Tue, 06 Dec 2022 01:48:40 GMT  
		Size: 51.3 MB (51301563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34af39ac37f03804edeb19cd824894881be851c37df5bba673154c60beaae19`  
		Last Modified: Tue, 06 Dec 2022 01:48:50 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:64c3fc0d1e5471d982ee81352c828eb5726ebb232852559ed2de22de58cc4b14
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50259668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98efb6ef93df1971c4d4576cb9aaa59f74423c8a575ff6bc649ce811ad6d9877`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:58:28 GMT
ADD file:d0791a1d4edcc52794bd2965adf77ed544c9b3d59bbdc18231a80a617dffa952 in / 
# Tue, 06 Dec 2022 01:58:32 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:58:42 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7f06ac539a35634b05751b5ff5c4e756830cecfe00e7e2d8fb4819f222ffae80`  
		Last Modified: Tue, 06 Dec 2022 02:06:45 GMT  
		Size: 50.3 MB (50259444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c8f5b6f4c3747265074b602e0dd6da667bec7e5aa23b915ee94b615f144ad7`  
		Last Modified: Tue, 06 Dec 2022 02:06:54 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:38b115c7872f2bb37af4b96a149eb079b11b5221f83f659f112fcf6a62820dd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54319555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7cf7ba356bdb06186b369bbe7d4b23a0d82c1718482d7c6dea1da4c6048a71`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:19:49 GMT
ADD file:367b691e35faf54e956ada3e3364007085df2f74ddd0f1fdf91a024e7bbd6b27 in / 
# Tue, 06 Dec 2022 01:19:51 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:19:58 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4de1727937141bef674e14dc4797bf7bf33815fa3f805c7b62efc248635108cd`  
		Last Modified: Tue, 06 Dec 2022 01:26:21 GMT  
		Size: 54.3 MB (54319330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f893c941a96111e08be34ba057a37490195a9587e6bb9be8f8c8fd4f576504aa`  
		Last Modified: Tue, 06 Dec 2022 01:26:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:bd9b4bd9f6396890df6ce51934127e125ef667f48c1439ea5d37c2b8df1e8c2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48665127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13430861cf19a753516247d5ae92a58910d69d61d87eb74aea6b2b39ab1eee66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:44:57 GMT
ADD file:a7e1b3d0e4383a4ca6340f45b93545785afd3505c5a31189dadb9858a317d0b4 in / 
# Tue, 06 Dec 2022 01:45:02 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:45:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6c783b63400e54709b92da2c5e6fbc522592db9242b957fe68edf4bd41feec32`  
		Last Modified: Tue, 06 Dec 2022 01:49:53 GMT  
		Size: 48.7 MB (48664904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834a12bed90418673e95dc497b1b832c5494937802f91804741fb80d84782685`  
		Last Modified: Tue, 06 Dec 2022 01:50:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
