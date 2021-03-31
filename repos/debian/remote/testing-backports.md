## `debian:testing-backports`

```console
$ docker pull debian@sha256:3f9b7fb334fd6163abdca9e708c0ac188d52641e335518e3bca4038279728022
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull debian@sha256:07488e56e0288aa7d5135c9f4c40337b49e7a3bcf8ba0963ccb6d852d62e3fe1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54868370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b766a1e114de1fe16b139fb549857bbebbcc6067859175f42dc19d233c410790`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:05 GMT
ADD file:43e0ccd9ab01bd6f5c0a9aef5f2ea7c9ee9af30fdf11c8a9c591587a4d089c08 in / 
# Tue, 30 Mar 2021 21:51:06 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:51:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:225ef05ef5535d13824643cc5f8d3e28d2d9fb76b074b6ec850f2d382becdd39`  
		Last Modified: Tue, 30 Mar 2021 21:57:29 GMT  
		Size: 54.9 MB (54868148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d235650169c896b4ab84277df205e0b5de90441aa387752029ae2352462bdcd`  
		Last Modified: Tue, 30 Mar 2021 21:57:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:81536fea5741c5bfe0de0469d0fa13dd639fdd84489e7188cbe983c53659aefe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52401362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e41f5413b7fe4d264d0b8b817f95d99bb9a0cc9df686cc57ffe2fa5e9659ee56`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:54:38 GMT
ADD file:d7353875b56cdaec9102bf43d71e3394442d9f0bfe92ddfb4df7fa1b973813a7 in / 
# Tue, 30 Mar 2021 21:54:43 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:54:58 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:df944c0287ea85ca4d17db5c8c07cbdf12b4f9b599d9d79ec87d0672dc222035`  
		Last Modified: Tue, 30 Mar 2021 22:02:11 GMT  
		Size: 52.4 MB (52401138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0893ae9e8b44426d95f78fa3f418e925c924c8f947bd7e7af90c78b62de302`  
		Last Modified: Tue, 30 Mar 2021 22:02:23 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:73735bbc0da9c43682bcff58165d9fb592c04d94e35a15e8851a2984dbfc07c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50069414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:855990220119e5d2e85b2a022ca02b55f3bd1c93d2d009ca5c007acf36d37ea3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:12:24 GMT
ADD file:c0c7dd2250180b510e47314411a1f1c299e0427140e3054e187c06913b1fedc8 in / 
# Tue, 30 Mar 2021 23:12:27 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:12:38 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ecfa64773a9df28af0ed2a93d1d6c9a6df5b9657b76a82b0d3258d85638b207b`  
		Last Modified: Tue, 30 Mar 2021 23:19:30 GMT  
		Size: 50.1 MB (50069189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859c965218cc26026ccce638437da5422dcf51947427f668af52f86422ebcd33`  
		Last Modified: Tue, 30 Mar 2021 23:19:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:73e72d7709321af4df95b5242e2ed47aed02537ea4764ced8d6887164a071ea0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53555427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a360737eeb25e5793d8a3ffbe898389f9c755907b6793d286b8e689f8a3e2d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:33 GMT
ADD file:f973554eedc62f5f46e9f38329e793a03f86e59390a1556f79308a27e73077cb in / 
# Tue, 30 Mar 2021 21:50:42 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:50:55 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6c5abdff1282a06d2e6071056f94730d9de00eed3f6e167672759eb8fc9eb6e6`  
		Last Modified: Tue, 30 Mar 2021 21:57:31 GMT  
		Size: 53.6 MB (53555204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92a3c942715483ad014e45b4efdae14c7dc31cd60ada8e26b5b998f730f62d3`  
		Last Modified: Tue, 30 Mar 2021 21:57:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:85282b6d07623610bfbe60a660c0f3ef1c0dc9271570bb8225caa34ff6c4c60d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55881591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20a25714999ddb1a901ffd9220d6f15e3fe0ed78904f3cda33950ddf6f9e437`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:02 GMT
ADD file:aaf8017d3d7400ca913ab70e21b97c8ad7c1d91899f2849abef662e08f7c4e04 in / 
# Tue, 30 Mar 2021 21:42:02 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:42:08 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1d667c684e28a4d55cd8b356a1aa42ab5387f7012f062b39d84b7db517a7a044`  
		Last Modified: Tue, 30 Mar 2021 21:50:45 GMT  
		Size: 55.9 MB (55881370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61ee959620477fb9e2a58a2195ac689ddd248650286c6f2d3220c64679c56cb`  
		Last Modified: Tue, 30 Mar 2021 21:51:00 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:8a941499f3b2e8d02e6525043b33ff98725ab93fe2d8db785b8ba49c3c1ca2cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53127404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f48307f0d88a91fe1d6b51bc453b9eb379435382c50a991896b916cb08054b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:11:46 GMT
ADD file:894b66014be623b08246573be16c5bf72d97625941364a30ea7a02e4aaf5c4d2 in / 
# Tue, 30 Mar 2021 22:11:47 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:11:52 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6220a047ae2abcb05177be77917e5ca0761ff39b24177e922dbf5175db92716d`  
		Last Modified: Tue, 30 Mar 2021 22:19:41 GMT  
		Size: 53.1 MB (53127182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa19a6788577d0ad3ad9f6ab453be65415432a58e08ceaf440bff6a446bae095`  
		Last Modified: Tue, 30 Mar 2021 22:19:57 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:185b08212da833908221057abf58bf9fe4029422d7826a477160a03c36d90d46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58783570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030bd8a5e88a8feacb5343d137975527396437e8ae0e1260944acfc04a999a21`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:38:18 GMT
ADD file:edfcf9830c92f6132c01327ed8606a0f69870c393e5c0c7df42b6a56f64ed7d8 in / 
# Tue, 30 Mar 2021 22:38:25 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:38:41 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4f44d41ee258a066a0c0b50b69d17bc36cebed954d5b1b5450cde5e7e38b6adc`  
		Last Modified: Tue, 30 Mar 2021 22:44:44 GMT  
		Size: 58.8 MB (58783345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298ede8389079e5c28416c739b8afaafc9591f065ec1d406e032cfa941687614`  
		Last Modified: Tue, 30 Mar 2021 22:44:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:407acc2301b0fa1312739cac228d14547ad3cada555770f913e0bb257eb73f47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53148707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeedd077fbb112f177020d6d98ddd79a5180d02e76bb04be4188c7bdbd9c5264`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:43:44 GMT
ADD file:8e1fa69c0f021a22f6b57a9caba4481a9da0cf39f239442db53eb11eacfbb45c in / 
# Tue, 30 Mar 2021 21:43:47 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:43:52 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ca6391c3ba05dc203d2d8e0b8b0b4b2351b46f0ac20ce212409979a3060a7c71`  
		Last Modified: Tue, 30 Mar 2021 21:47:45 GMT  
		Size: 53.1 MB (53148482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06992b09d67a75a09f3dd3aac001c81b4b21d90e705e33c799bcd0a62f6e1901`  
		Last Modified: Tue, 30 Mar 2021 21:47:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
