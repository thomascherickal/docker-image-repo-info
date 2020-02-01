## `debian:testing-backports`

```console
$ docker pull debian@sha256:bc73ebbbff860204508f1dc9fbe1b6d3945d4443df3a4a53515efdeafebc1d53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:0d1a1c5fe1ae0cc8abbf02779ea62541602a9b79d790e33fb01e410819e90826
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51490954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0768aa7e5cd079faa7eff4c6bfe23810e54dedc305ea302b3bba4563f2480697`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:24:12 GMT
ADD file:eefa3f1929486475ead0aa6a9002891b3b05a98556bdd8b07a78536ccb66b2c9 in / 
# Sat, 01 Feb 2020 17:24:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:24:17 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7c9fdd8a58ab01cb58d1c1eb32a2f697f78cf9bdaa500ee2c436b7acecd65d44`  
		Last Modified: Sat, 01 Feb 2020 17:29:16 GMT  
		Size: 51.5 MB (51490733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b23541d52b6ef09ecbbd6cb6b7cd1529799db5ddd343078a77e897e269f3176`  
		Last Modified: Sat, 01 Feb 2020 17:29:21 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:89ec27d5bd9a255fe69b00037ad1ea0b980b730e370de6d5dcc3ed3f5aef6292
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49485275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d85c4317167a5ca9a56433f9bf01e7c6387e6e4b590bc7a870ecf84c985aef05`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:54:14 GMT
ADD file:ae8ba1ca1afba05a5c2e742b53e5327fc31461ce3ba6cc1d842a85616599336d in / 
# Sat, 01 Feb 2020 16:54:16 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:54:23 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:91026fcd0d4f9301275f1dcdd3aa8601af59bbd3c9b5c0d12fbf33a12b62c736`  
		Last Modified: Sat, 01 Feb 2020 17:01:26 GMT  
		Size: 49.5 MB (49485050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0645e3f1abf50c1a6b7a43afdaec99fd3a9c3ce15ccae504d6c954071e7c4b59`  
		Last Modified: Sat, 01 Feb 2020 17:01:33 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:d67c6774c0dad6509641599ca15536ed5ef18a132ed832d3e7340989e81f93e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47233952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de77ecae80b2c92c47858bf833fa9c3a4a1bc30f0f6bb328b4a575c8ed8c6c09`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:48 GMT
ADD file:dfc2213b46d6288c8ba30547b950ae299bfc0c436f2e8a8d3f6376e91bb05256 in / 
# Sat, 01 Feb 2020 17:04:50 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:04:59 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fe08c30a3140b22ac1acabc19c0e5e86ef978758eba0be5489e35746bd43f3d9`  
		Last Modified: Sat, 01 Feb 2020 17:11:51 GMT  
		Size: 47.2 MB (47233726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98064400c58c98947e8ed18501e6eadc7b2fd49cc0eabe1a165f6e027e21634`  
		Last Modified: Sat, 01 Feb 2020 17:12:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:43c707699bf04cde0747f2dfc649cc80d5201419cfe4293e32740e3003962a08
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50453225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7e698da5eeaa6bf0847c016cb252fbfbcc1865692fccb31d43ec07f785807e2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:35 GMT
ADD file:db821559bc10f9e72e5927bea485644dbba15b9be5d035d29e74ff74c90eaebc in / 
# Sat, 01 Feb 2020 16:43:37 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:43:44 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6a8ea3b8ec391d7f13575570e7881031715ff8ef67e1224726395e166f3c9ea7`  
		Last Modified: Sat, 01 Feb 2020 16:49:35 GMT  
		Size: 50.5 MB (50453000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e95db6fc964d7cd9655bb1e41e35c3bc4f86f811a7a12d9d056f508300e6e0`  
		Last Modified: Sat, 01 Feb 2020 16:49:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:8147025efd6a15af8bf99997348d57dbc05571add504c43c0ca43731f0d879f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52628593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3440e0108303fcefe3f3a3e5c8ab8f32adcfd480935c634a10fece1d46c0f606`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:19 GMT
ADD file:f2c5833c2a0a4a12b2882d4cf6e597cb55b5d434cc5f30795f3f0eb61cc71331 in / 
# Sat, 01 Feb 2020 16:42:19 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:42:24 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:02ae370ca056ac7552a68d5652c7c4b1a22034b3e3fc7d3794f22ccae9cec7d9`  
		Last Modified: Sat, 01 Feb 2020 16:47:44 GMT  
		Size: 52.6 MB (52628371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02432ca9681d6f4fd7b7da20aacfc3b678fc3df0ac9a9723f4b57a527cc06166`  
		Last Modified: Sat, 01 Feb 2020 16:47:47 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:908cd401bc546273c622187bedf03aaebd6ddd1403b15a1548bb829f45c6063e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.3 MB (55316543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ebcf543e1c15b7dbc4ac0ebbe4e043ec2682a1e0211922c69f019341c81189`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:21:17 GMT
ADD file:51c285746d844fee079ad0e2a25ef1f75e4c1bfcdf0f42f42342c83505723548 in / 
# Sat, 01 Feb 2020 17:21:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:21:30 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2ca90af24fd5c34f627715eb0513e46e570af7b73a18c9254dbe592577f983ba`  
		Last Modified: Sat, 01 Feb 2020 17:31:53 GMT  
		Size: 55.3 MB (55316318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7c10eb8397d055439b6bd2b4772dd63757ee122f43be5c4f408e387561b804`  
		Last Modified: Sat, 01 Feb 2020 17:32:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:7bb9f390c359809d1c280d77cf0271dae97bf3a88954fd32a78be7e4d47a0be4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50133361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32fdecb22edf8fbe3f6a872742ba96e55112f76410d62812da95b43c85358e99`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:44:04 GMT
ADD file:36116a9a93cd7aa1b8833e81b76f12a7f4bcad34c03b1fa7b7a989aaef10e039 in / 
# Sat, 01 Feb 2020 16:44:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:44:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ec2c5ae8e3e76894a1679f12164b46f8665104cdc245059af4f020253123a66e`  
		Last Modified: Sat, 01 Feb 2020 16:47:56 GMT  
		Size: 50.1 MB (50133136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0ab714cb645932cebc5a2db29c5af7812cb56dfb51d6ed128a7493f8ad7d53`  
		Last Modified: Sat, 01 Feb 2020 16:48:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
