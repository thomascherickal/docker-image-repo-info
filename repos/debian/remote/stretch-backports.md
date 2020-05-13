## `debian:stretch-backports`

```console
$ docker pull debian@sha256:c65af8bf85475a110c602a43f0633395164c457508ff22273faafd1bbcafb1c7
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
$ docker pull debian@sha256:fbe8f005f31eb5537e625af2e167c5dc79b74feafe2d03264e8f95e19cd44f85
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44068041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147685a5538727bf0069484fb0bd8b53a6a8ee26f32686357b1a339d01322d52`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:54:56 GMT
ADD file:85da223f359bde63cb0354ad866044074595630104ae55a1790b83f209585e48 in / 
# Wed, 13 May 2020 21:55:00 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:55:09 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1e24629b52a5049ace3da69cc30167057bc65b6c050c9fe405d45685d76f1dd5`  
		Last Modified: Wed, 13 May 2020 22:03:01 GMT  
		Size: 44.1 MB (44067816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5ee578c38a30f4b70b15917d16defa2a23c1d8da6fd52eabf6ca599d9f58bd`  
		Last Modified: Wed, 13 May 2020 22:03:14 GMT  
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
$ docker pull debian@sha256:1ad7b378b36d3773754b6a9cd2223b241a2ae4e45adde3fc9a97b1b89e7af288
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45232927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd552688db98f03a0e460758009f4460b6040ff6735d2155bc5aaa12fa3a8e27`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:44:18 GMT
ADD file:80db5381a461bb249455c6e92a06f91a777c0d8db654106cc55f91d6252c3c44 in / 
# Wed, 13 May 2020 21:44:20 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:44:27 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dd38adf1f4e3b358b79e0f6559fa135ec376d7abbcc3f8bf0b62a2d19d972cbc`  
		Last Modified: Wed, 13 May 2020 21:48:31 GMT  
		Size: 45.2 MB (45232705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219274ce4fd79a171235fb9d0227daa3357320b8e40aa03f4e37a6f6ca5de3cb`  
		Last Modified: Wed, 13 May 2020 21:48:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
