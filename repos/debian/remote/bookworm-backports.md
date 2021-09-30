## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:c8e37bac1ca7031f1abe6654ed7eaa0036f01b72f77cc90d225c37be5848fd82
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:a29fb83fecec051a14ef8041852dfe8b7aab31442111dd5905eb224a7b0f52e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.4 MB (55449704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f50089ca9bf81c09d4d1d84a7736381d9a48284db356fad44a77552dc076e18f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:21:52 GMT
ADD file:33c5dd42123c7cb6fbc82210643d05c51e9d986288a71f2388a62243ea91479a in / 
# Tue, 28 Sep 2021 01:21:52 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:21:59 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:db79fff0ba23ba0e1aea05ba623192f962d20712b5c97ec6a33cd8a544ad28ac`  
		Last Modified: Tue, 28 Sep 2021 01:27:56 GMT  
		Size: 55.4 MB (55449478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e09dd467684246e1b04c22ab46305276bb56353f0bdbdbd821f1606b191e7e`  
		Last Modified: Tue, 28 Sep 2021 01:28:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:59024235bf34c5b2f6379a3b04f447656e992ea8adbcadbbbce5ae7cc03cc0c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52959764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c447929cd47eea4410ddf69ad560886de79d48b12762254af506bbc542080283`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:49:01 GMT
ADD file:e5b7ebc5665ff11d9518dfce3e60b02bdce0023642f037b884f09fc22323f817 in / 
# Tue, 28 Sep 2021 01:49:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:15 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4b879c7dfc01a52f93bb5ff4d9942f1131710b23a296cb63b70dee80a4702b0d`  
		Last Modified: Tue, 28 Sep 2021 02:04:24 GMT  
		Size: 53.0 MB (52959538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70683b204bb34377d6a97db3b39a0a7e2bdb54201e9b50738f748a374f914baa`  
		Last Modified: Tue, 28 Sep 2021 02:04:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:ee39e46d33955440e0acbb1c5ab542d1db51e83bdab18ea2c0c85ead4c5218a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50561965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35518103b4f3c36d2a83e5be917b5dc8f1ffca9e750ea65d38619975ab924f48`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:01:14 GMT
ADD file:92236a95051df6ff2979c899eca0d9deb91c9f10e56ae2243cf94c15c8fa747b in / 
# Thu, 30 Sep 2021 18:01:15 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 18:01:29 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f3b0098193b8de476563ee4443a08e0ae90952ca99ba52ad037218f8faba2f6d`  
		Last Modified: Thu, 30 Sep 2021 18:17:24 GMT  
		Size: 50.6 MB (50561738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc5d66084c2cc033297ad2daca3f4c45f3fd38d8de7e0b6f2cb871cb68bf162`  
		Last Modified: Thu, 30 Sep 2021 18:17:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:a035d33be5b5461b9028fc43275e7c6e5c9110a972eea7694469991c31b99a4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54460595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:affab6f1fa0985021bf8b58fd5e754e2d3280c95e74e4cbc04659e3f5a887d4d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:58 GMT
ADD file:94c440499c3c1197b13933c36f0f120227436d952c1d91d89e191ba9a336c8ff in / 
# Tue, 28 Sep 2021 01:39:58 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:40:04 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cba8d43c2ef00f6c2f50c46bbd19c371de5bfd664b7f4b1cfccbb66cb1736b15`  
		Last Modified: Tue, 28 Sep 2021 01:47:12 GMT  
		Size: 54.5 MB (54460368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c7d9644409e6d391ac873afbccb6baabc6c688d36a87b9a2c7ceb62ba5b386`  
		Last Modified: Tue, 28 Sep 2021 01:47:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:7d818a91a9a4fd373931c9abc109f9cf370cc3c67f31768950e24040e42208dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56469953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0b0c39d365677423543e5bdc3b12230e9c8a46d95777967bbf3241ef76e9350`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:08 GMT
ADD file:e786d747eaa81c1360c3b52e2cacfe804caf3188af0c7adb73e1724efe7f026c in / 
# Tue, 28 Sep 2021 01:39:09 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:39:15 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:68a0e488d5e84f8e3f3e8946a06f9839bdda1793f33953bb9035ae0c0e511a83`  
		Last Modified: Tue, 28 Sep 2021 01:47:44 GMT  
		Size: 56.5 MB (56469729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbb3b716fb70b1112fe6c49e1d1942e042f40c025a2d69889dc4e5560e764a8`  
		Last Modified: Tue, 28 Sep 2021 01:47:54 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:87fc8f5d3e2a7f4650a94798649212adc6136addd9fc61ffad95acd4af3bde18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54053766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32deb81d4c120f9269c57b4d82fa5ee689c84fb918b208fa1e4c5221ed1e96f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:08:57 GMT
ADD file:26460067a4e5d47bdbd66888edea27797133a4f4398ef67554c57e6a65e45a67 in / 
# Tue, 28 Sep 2021 02:08:58 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:09:08 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1211ee44b3648250584e1991f477a7ee6e47eabbd8ff966434dabe28fda43936`  
		Last Modified: Tue, 28 Sep 2021 02:18:22 GMT  
		Size: 54.1 MB (54053540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8252245979ad25f3b4c7b7a983a180f9ba54431077f449014c2479703af911ae`  
		Last Modified: Tue, 28 Sep 2021 02:18:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:9eba3035857ca484bd0414a59bf8857405a4c64bb25c34dcb30d821c85afee6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59526527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab5cffaf828f98f3f994f38221c6f3d681194e504efd9c4b4be6b1c3be3ccb95`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:20:52 GMT
ADD file:8c4f85d12b49771f370ff2d26cbefa13b6abd92b68531781c09d00ca174457b2 in / 
# Fri, 03 Sep 2021 01:20:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:21:31 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:842eaf445b44995004f2497f1b8419fb7e9e38e2348927060a6bd434d949be24`  
		Last Modified: Fri, 03 Sep 2021 01:34:04 GMT  
		Size: 59.5 MB (59526302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56c32a2ad1caa58a0d62c25d6c203a249e19552ba2bdcd222df920eea3faae6`  
		Last Modified: Fri, 03 Sep 2021 01:34:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:98e02edc8b856c0c32e72212c5a0579d9403cfdf4b262fdc84e2356b54c2a106
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53691414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:832c01714853bfc938539b8ab3d68aefc41598d62ab050a4cbbd376f6a5188a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:03 GMT
ADD file:9ab357aee775c3b3d970cdfc3fa28e19949bba7e4541daf34233cc8f9b420ccb in / 
# Tue, 28 Sep 2021 01:42:05 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:42:14 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e1cd347e6e1dfbf875c086c979df124efc7bfdf9c2a5874cd9a6915484b71e46`  
		Last Modified: Tue, 28 Sep 2021 01:48:11 GMT  
		Size: 53.7 MB (53691191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3060920f6cfd61e624888505f07ff1035c73c93b2c454eeb85492d1c0cd5a1`  
		Last Modified: Tue, 28 Sep 2021 01:48:18 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
