## `debian:stretch-backports`

```console
$ docker pull debian@sha256:70a49141af58ee6e6ebcb5f26f33f6b885d5f9ccfc6c4573cfdbad163f14b389
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

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:2a99c76d99ff78530bb062185d63964e1ad786a1b819149e1cb5505d119ff568
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45376159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3776cb1214157d66ec82aa9bfe7832d71eadc131b2e91055b9458fb837b1ea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:23:35 GMT
ADD file:82e0eb87c6ff97b66f86c9fee44884c4cf1b08f5721f36878fc7a15a125b5079 in / 
# Wed, 13 May 2020 21:23:35 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:23:41 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e6ce7b04634a37b5c20274b3cc1469490cb28f734448d2c84d01454465418e1f`  
		Last Modified: Wed, 13 May 2020 21:29:57 GMT  
		Size: 45.4 MB (45375936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a60e9291474a48588e74a7e95f8a0d0b34dd0f2194f183ef185a2d2338a1baf`  
		Last Modified: Wed, 13 May 2020 21:30:04 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:dff4fc1027a7ddcdc6bdaeaccffe69b3baaaa801d3505836a8b65765b2133a1e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44072101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f22d0964ae4be97a901af1eed8d146c570b23911809f8620e65b68a43ffbc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:21 GMT
ADD file:57aa6b37e4a65a6ce77d5943dfa67cd85ae4b6c145f9d2baa87ee4e569a77100 in / 
# Thu, 14 May 2020 22:42:22 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:42:34 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:910ef58b27ef80c5e71df714f5f3d3c8d01b34e7e567691809a33f51d01953c1`  
		Last Modified: Thu, 14 May 2020 22:50:41 GMT  
		Size: 44.1 MB (44071876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df89348675db734e9741e17b7a7818d3bc7463c32a080714c94a79fe31b39023`  
		Last Modified: Thu, 14 May 2020 22:50:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b50f05cf1d2fff91c8b40f94f1f43365d983ba9ae26ab7fe76694fa5e6f4485d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42101330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50c6227bac356cd16baf2ae54cffc7d869796cec994ad0ebf22ce8a2a9b7071e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:18:55 GMT
ADD file:22401e33698b1bb830736dfb4dcfcae97faee4aeb57fbc910c50a0806fb726e3 in / 
# Wed, 13 May 2020 21:18:57 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:19:06 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6d01aee5144e594ba9bd007624dc3b8437510d15e6c34689c8475bf2d6b5c3e4`  
		Last Modified: Wed, 13 May 2020 21:28:12 GMT  
		Size: 42.1 MB (42101107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61579d0860cc3d2f9df0f144e27a919837b9f031175ce1a7076d2632487f1fab`  
		Last Modified: Wed, 13 May 2020 21:28:22 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1e7e55120add01c2acceaee252750bdc623dec07a1d18b021131a13629362e04
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43159201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e633ba98a25b626d89c7b72d84c2f9b961149d61114758c2c70121a1a1b8b4ee`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:47:38 GMT
ADD file:e7776aac0b87be303e31e5947db89f835a4e17175e339ec23becf5fe4a9548a5 in / 
# Wed, 13 May 2020 21:47:41 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:47:50 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0480c895dd1d5b237cb931426f18706cbe8dac16e19ed583f3010f3655094efa`  
		Last Modified: Wed, 13 May 2020 21:56:03 GMT  
		Size: 43.2 MB (43158976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95577346c562a1f777b63f880a6ac354a1dad120dfc943ff6b8785db80e5fd53`  
		Last Modified: Wed, 13 May 2020 21:56:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:b6d02edceede28b540ed5b71fca163391e23a2f1e0e03934a91cf431c883cf63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46095263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:770660eed773babb60d96d175dc66e51c0ec920c14f7396e3a709aca9890c46b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:23 GMT
ADD file:0d501ab6846646b4793ce31bd08a81ee75bf7ca50e44fad4f41d38ea73217f94 in / 
# Wed, 13 May 2020 21:42:23 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:42:28 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:738ccd27fcd21d91d1826e5bb5ee29ef3a82a770de7e1407c86b04395fdd1335`  
		Last Modified: Wed, 13 May 2020 21:49:47 GMT  
		Size: 46.1 MB (46095041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d67272d3cab0be41ce90e33f0d03c5335478fbf14e5331b84d746bcc563eeec`  
		Last Modified: Wed, 13 May 2020 21:49:53 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; mips64le

```console
$ docker pull debian@sha256:518d751a58a6992a3487840b44ec9ad2468a52b02f2b1bf712ccd2bc40e4f793
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45049000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af60d4b2823a8bef2accfd53f908d7eda8ee828093df48e76925d68945fba51`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:52:06 GMT
ADD file:7bf5ef3df2c7fedfe3177de091f107679e7882507d08882b3203eff7ac42da5b in / 
# Wed, 13 May 2020 22:52:07 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:52:16 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:690bb78d0f5d6a469cf42f228761b11696fe51dbcca8ec4392ae892677a415b6`  
		Last Modified: Wed, 13 May 2020 23:02:33 GMT  
		Size: 45.0 MB (45048775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b2cc59b7c3ff4dc6b9b6f00879e37e51ba8f5841ceac389a6ce2fde44d43bb`  
		Last Modified: Wed, 13 May 2020 23:02:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:e67585bb62259c6edbd63ae88c8c2e8a90f1c51a25c69148cb39fb9a615808ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45646416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b02bb7cfc805ef7774740ccf74f071ac7569b5a87c3d1f84e44e864b3df9caee`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:39:29 GMT
ADD file:fa4c7e3ca04f092e53cc791a32c929663412df3f68de2733bb867053577bf1d1 in / 
# Wed, 13 May 2020 22:39:34 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:39:52 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7732483b686efe14a1cf8add89a1568b83892e243798fba30808f1fc6287210b`  
		Last Modified: Wed, 13 May 2020 23:02:10 GMT  
		Size: 45.6 MB (45646193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04812356da9416f8d0da9fe331892f11d403afab87d7089b8832a97f350bee3e`  
		Last Modified: Wed, 13 May 2020 23:02:25 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; s390x

```console
$ docker pull debian@sha256:1fe84f896f85f303a699d07527ab5c0a4c0cc14854579edf67d046b4b2880113
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45232303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cebed9aaedfc2cd9d614d651305131e4a96f291ef56a9bd365356e952f5712e5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:08:23 GMT
ADD file:32ad2f356c0ec407aa31085089417aaa9f72a5dc2757ed68a0adf7a432e4bdaa in / 
# Thu, 14 May 2020 23:08:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:08:31 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dc69489da20ae5bdf6cefc772e7ff8420ffbd2c920a57165de6ead66d1a997e4`  
		Last Modified: Thu, 14 May 2020 23:12:48 GMT  
		Size: 45.2 MB (45232081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89c5379fd35e4805a32fb5020985ab799b0668198ec5374246cf68c03df3d4b`  
		Last Modified: Thu, 14 May 2020 23:12:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
