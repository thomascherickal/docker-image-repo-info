## `debian:rc-buggy`

```console
$ docker pull debian@sha256:9a8a77ee697c9e3d573e4a7b2d74908135d9e69f6ececa212446bdedaddc736b
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:3f7a8d150d6400a53198e6d4b890375771496b482188540f394c52cd5e201ea7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49552191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9598b8eae75731d5616b6521473ce7a1620a95799ea808615ffee90da42a4140`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:22:34 GMT
ADD file:8ed2c72091b90575b320038c2ad715760d6382aeea5c416dd16f7ed04e955217 in / 
# Mon, 12 Jun 2023 23:22:35 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:24:31 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2e79cba44192968ca6ea42058e67723ae58bebd2ea54b31f432b1ffed9fea9d9`  
		Last Modified: Mon, 12 Jun 2023 23:28:29 GMT  
		Size: 49.6 MB (49551965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75902ec6fa24003aa6eafbb12464d5631a1b2c913f2a6d8c271ebb25209a56fd`  
		Last Modified: Mon, 12 Jun 2023 23:31:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:8431f23413f063c89ca1c5c6bc53816226370f5d807f28478533251d83a23ca3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47322701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c31435e717296b9e24b2c39649540a77f07be5b3086d293441493344b7841809`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:49:11 GMT
ADD file:e6181e27889c016519d8d701345aafff7138df96a76fb6a29403c8a33a3365fe in / 
# Tue, 04 Jul 2023 00:49:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:50:28 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:667272d8fe1bc81ce33874dbc84976c86d6b95f50198465a6ab672c71d87f666`  
		Last Modified: Tue, 04 Jul 2023 00:53:33 GMT  
		Size: 47.3 MB (47322473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2190885d65eb97f69c0c7c0c158851e72bdf60e2cfdb2b1136c8de3f6dd6c37f`  
		Last Modified: Tue, 04 Jul 2023 00:56:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:7ab5870e0bdbdeeecef461a5b5fbb2906ea9ee2ef4c5da1c1b8998deed1c8a18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45124201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bfc027409f8fba31974738384e2dfa1f2a1a243b3f73b6fd5e1b69f93300462`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:59:44 GMT
ADD file:5be8eee7722dc860882f26018d8a0de49a4db6fcaa0f35d1dfbb74eff22929cb in / 
# Tue, 04 Jul 2023 00:59:45 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:01:33 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:42cc2becb0b735f0260d9f678fb1201bbe47c438212c5faf04879fab6a2dd73f`  
		Last Modified: Tue, 04 Jul 2023 01:05:43 GMT  
		Size: 45.1 MB (45123975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce68afc01eaea6b552daf2fa88d7caafdad8a2a5bd322b779b58e945322376f`  
		Last Modified: Tue, 04 Jul 2023 01:08:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:f2d64f9dfca60b88094943e852e16d2d59f1c58254e28dbd962df581d657cc02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49592320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6166bf04153622ceb081a6d7ad917e58e19deed2d74dadaf0d34d6afdff992b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:41:38 GMT
ADD file:94f1432513f9a03b38028af02b1d1720fb0558559faf3e7f9d7097cf6b962056 in / 
# Mon, 12 Jun 2023 23:41:39 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:43:07 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8ba9ab3e6f12b9702649c2e0c7d78e22ffb9183f68c288b9edef2387bd8d4efd`  
		Last Modified: Mon, 12 Jun 2023 23:46:36 GMT  
		Size: 49.6 MB (49592096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a26a4b55b505c1b8811d5ef643065d6a511757cd32a9e5903a600bbfdb41fa0`  
		Last Modified: Mon, 12 Jun 2023 23:48:55 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:f327ffb8e721124d17d34e11573771bd0bfe2f4cca46b564b50f46352d1bc39c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50562922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2917eca95e35bdc009a86c37d220a588cf15dc13bfeba7c3593f86304916cbf`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:42:10 GMT
ADD file:209e3bb955801ad81eb18a280f9fbd5500a0e1f04565e6c94c9cd24dcba4c0af in / 
# Mon, 12 Jun 2023 23:42:10 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:45:04 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8bce10b6f772acc79b03d87add4bd359f98c767e3599f82d8e351cced14c1a11`  
		Last Modified: Mon, 12 Jun 2023 23:49:26 GMT  
		Size: 50.6 MB (50562699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9dcb6086059e0e729dfeee6a8981c17e9a8ab6cd24b8230607a0442ec8cec23`  
		Last Modified: Mon, 12 Jun 2023 23:52:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:e22162bafbe5ff7e199da64bdbb05a5e1a9d73af060a0cec82099bc3e314584e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49455626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:551188c58f26c946df80410bde70b326be018cf165af6aaa6c09ab618459e2ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:12:32 GMT
ADD file:ab2873cb088258c79fab5dde2d754d1967ca11e58adcf6a08811206759a323d5 in / 
# Tue, 04 Jul 2023 01:12:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:18:03 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:796c2f1009ce9a433d10a1f4708cbb79ef733dcb0ca992041a6aa621e85d8410`  
		Last Modified: Tue, 04 Jul 2023 01:23:15 GMT  
		Size: 49.5 MB (49455398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619a4904f147ba7ddbe54aa9fa10e34000a998f58d5372d5f112bd3a1bbdc738`  
		Last Modified: Tue, 04 Jul 2023 01:28:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:f444f0a3398423022d1d74efb121bf81d09bf32a510b56bb14bddc08672af7f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53558740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02da704596a01ec55697a318a9010f9d43c226519cee0226066b6cef34d88a4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:19:31 GMT
ADD file:aded196ce7e0c005fe55d5a92492be8cc5d7934fac082b7ab95b8c946e71e0a2 in / 
# Mon, 12 Jun 2023 23:19:34 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:22:44 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6e3f8e732e00762188b5ba00db7db3f36c97d0fccdf3d6121db4ca1febc7d190`  
		Last Modified: Mon, 12 Jun 2023 23:26:13 GMT  
		Size: 53.6 MB (53558517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbb443cafb17945962722ff343dcc88bc037e146dc7a95e4fbd9a82bcd7271a`  
		Last Modified: Mon, 12 Jun 2023 23:29:48 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:6efa5e58837f36317915683b39fe74ebfbc52a2c219f3a4f7fa26782cac1bb3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47920807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccd4555ec09bffca72a19aad479fe7c3627663fea88260d5c3bb79a70195b53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:30:54 GMT
ADD file:7ea0e5c460c626891cd3fc90639d6bfb9a27beeb7f5c79fd9c348c5b6244bd0d in / 
# Tue, 13 Jun 2023 04:30:58 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:33:22 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a129144c9fdcf79f6394b7f7bfa3d7e6a0c8ebfd424dca918695356a1b3bf970`  
		Last Modified: Tue, 13 Jun 2023 04:35:27 GMT  
		Size: 47.9 MB (47920583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d1517ac888f7b6f5262c426b14a1af632f244495c7cbed76920d5ad6e9fe39`  
		Last Modified: Tue, 13 Jun 2023 04:37:13 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
