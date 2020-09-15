## `debian:buster-backports`

```console
$ docker pull debian@sha256:862f5a64d585d1d487510779cd0d93e2158e5fd2352469ffc4e67fb834cb6cf2
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

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:69144d60ca675c910e0e8efe0d405c4031620f86a2218c3855cf5c5e3f8fce59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50396138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b4eaeb7691a4c549394d27fb241209061765bd7f4822a546e3b4ec115ff59a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:23:04 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800f673b4bb9d0d14a29f59f6f17ab4706ef284672a58da41a81a34825475eac`  
		Last Modified: Thu, 10 Sep 2020 00:33:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:a1554cfdfa262912113ee42319a3395899bc0841f4587a43ae32963627cf493f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48109101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7b88b66c96afbb1b3664651ae23450f30e679302f507031bd90baf8d409c059`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:21 GMT
ADD file:a4eb5b1dc9adb84c94eff31b2ba5949b13b32831aff9a39d23ba20bc76d16449 in / 
# Wed, 09 Sep 2020 23:53:24 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:53:33 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:246514107a0cb62099f20170639c25bf457998ef723200e2e9343b78321b1a79`  
		Last Modified: Thu, 10 Sep 2020 00:02:25 GMT  
		Size: 48.1 MB (48108877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f4970f8e182062a8f02aeb40732dc47fd730dab553350cfe27918ad082ec28`  
		Last Modified: Thu, 10 Sep 2020 00:02:34 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:1a980ea80142dc3777c85a5cdaf6e2d65589c927c14051ff6df6ea677d8e4634
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45869524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7311dcb602e6526e967f339638bb7d2e2a8a3fc893f430f99a666be399e599b5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:07:32 GMT
ADD file:340663c3add65bd8904ba51984e6080c6aa6d237bd845f4e0aa22626d31497b7 in / 
# Thu, 10 Sep 2020 00:07:35 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:07:43 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7d9beb74056b685831827b5f21351f021873d8ba1a1170b378e5edf5f46d114e`  
		Last Modified: Thu, 10 Sep 2020 00:17:29 GMT  
		Size: 45.9 MB (45869299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936669f0e27a00f295b6b513b21566215a80f80f6de933904b4cf2d0a8e83156`  
		Last Modified: Thu, 10 Sep 2020 00:17:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:bb8ad1527287fe6c206ecf2b90f638383a6106546fdbec6865376c4971d0f238
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49175773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:703da69b5448aa6c8084b94742fa0a9a22224d2054ff04896346226ca84b40de`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:21 GMT
ADD file:c8c11e622b1b8a1e31f32e2457ff4d1314d5cd4a7ad22b3991ab9d0542db23fd in / 
# Wed, 09 Sep 2020 23:50:22 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:50:35 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d3a32671b6316bd11f4bf18cb034394ac94d2bb3bc6d09de388b19b06fb94b91`  
		Last Modified: Wed, 09 Sep 2020 23:58:45 GMT  
		Size: 49.2 MB (49175549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4646245b23148775491ff2e67dcd0eeb9ead2be242fbbdaa9694b22cbe05383d`  
		Last Modified: Wed, 09 Sep 2020 23:58:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:f74cc2af79a9462de38df83c113d83614478643472448a9d5e11c688613af537
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51159075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf06d0576f5067edfc2e8905489b301ac0fb49b99b931e10d001bb3c81bd8c8a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:39:58 GMT
ADD file:39c4b1e1e5d34f52ad1f95b26bfbbf45f307b94a52d472a561496c440f96d8a2 in / 
# Wed, 09 Sep 2020 23:39:59 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:40:05 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c89594b72f230eaccb7faa969906602c0f8e2667b7e30e66fe230243f1b5f1d0`  
		Last Modified: Wed, 09 Sep 2020 23:46:14 GMT  
		Size: 51.2 MB (51158853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4559b9909fae8e404b8269d09323920b95f6f888c0227c3bcbea11f8537fbd6a`  
		Last Modified: Wed, 09 Sep 2020 23:46:20 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; mips64le

```console
$ docker pull debian@sha256:9797f57f415c96536872acaab35f0a83a0c1328e02731567361afdfa2aaad9ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49017552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907a2ab4da0e1aa0a409c313ec971bb04a2ac71e8c9184a37cf8faa93443792b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:09:36 GMT
ADD file:c0072df9b5371ab5f33b6c7207cc89cead1e9ee00ea0f68bc3c41a9e360d8ba5 in / 
# Thu, 10 Sep 2020 00:09:36 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:09:41 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d525d039bb76c93a9b7252a652280bfd235ea07921134a11c616ed2781990153`  
		Last Modified: Tue, 15 Sep 2020 01:12:33 GMT  
		Size: 49.0 MB (49017330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb7445103749b4c65086fb35a9f960b284ee6fc83fc76684ef0b35072ccba85`  
		Last Modified: Tue, 15 Sep 2020 01:12:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:83b5712737c0b840dae06cc377158fe4cf1ea347e467da036c0a0315853b015d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54142869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17712df69f307b8698a58eefd0cd3ae664068f274f396fb178a50246d9f1811c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 01:04:56 GMT
ADD file:a2329a0372b3b40ca345795d86a78ab4cdaa3a1eeda3a5ece35a83881543db1a in / 
# Thu, 10 Sep 2020 01:05:18 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:05:49 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:aff7fe9e9819c2b9d4338fae03bd06eb6784016bcf53b2eeab88c21e47dea428`  
		Last Modified: Thu, 10 Sep 2020 01:26:27 GMT  
		Size: 54.1 MB (54142644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15431f54042ca83924753a2653a78b275bbe28e22ae8858f8ea198dc5f344b2`  
		Last Modified: Thu, 10 Sep 2020 01:26:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; s390x

```console
$ docker pull debian@sha256:890bedf58315bc929558081738ea425400acd8a281b41fa4baededc18e542373
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48966515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fa79901422173454f8676f48984ae8eab6b354b5f977d5c2e4423298584a199`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:11 GMT
ADD file:67eedff26215ed3c8100b93d0201c563ec8efe2af7bdfff5c7717037f95057af in / 
# Wed, 09 Sep 2020 23:42:15 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:42:24 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4c594945c9b37f16bdb296d1c06754e5bbcc3c28a736d7aa6091f61a081b3cfb`  
		Last Modified: Wed, 09 Sep 2020 23:46:12 GMT  
		Size: 49.0 MB (48966294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61af016f643692a4ba7b004171dc529891b16501dac7611e857fb1b547d13c6`  
		Last Modified: Wed, 09 Sep 2020 23:46:20 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
