## `debian:testing-backports`

```console
$ docker pull debian@sha256:0f3ebd1bdb466d68c87ba00669bbc8986cc8931c38693e04f7fa2ee7912c11b7
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
$ docker pull debian@sha256:d8165cb440b721bc96f77d87d4591809fdb460c1cf2bd3cd66922abdd16f47b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55567382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:637fce4e5bfdce4eaf59e236f5bd2ba32dda3b9010346b2ad805de92753d6d40`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:41 GMT
ADD file:31a3d405e7e9d997819ea8e6e3988121b5abaa06c8bbfcc777bf3564aded3f21 in / 
# Thu, 02 Dec 2021 02:50:42 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:50:45 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e3875f34eeed9a22ac1e5f2fe94e6fe0cd72a84f25c5a217f38aab0504154634`  
		Last Modified: Thu, 02 Dec 2021 02:58:02 GMT  
		Size: 55.6 MB (55567156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20489488bfe11f36dcf0a5808f549ca9131975c90ede4db2b412a3e2203aee1c`  
		Last Modified: Thu, 02 Dec 2021 02:58:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:78afc7c25430a890c957acaa76cc5b52ef1102464ebb4482cf86229adcca76ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53031472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c69ac556ed9cbe484dc5a910246951dce3e3d6badab284cef3e5a1d986e54bc5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:58:37 GMT
ADD file:24d5cbaf475011d519415bede0f00a59e3d60e3fd564ec5377d69f12a2e79146 in / 
# Thu, 02 Dec 2021 02:58:39 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:59:00 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c46357bdde6cd4bf4e75bdbb33f3b028ff99f5015c3d52a5e57ca8a33eda9b26`  
		Last Modified: Thu, 02 Dec 2021 03:16:41 GMT  
		Size: 53.0 MB (53031246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961a7932cdb8bc61f8a247cbf698e484c224e9b6aa5276f65eeaa132f53c1633`  
		Last Modified: Thu, 02 Dec 2021 03:16:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:e6c65237faddc55262028b030dafe111a6f7292720add98216df351ad6fd2063
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50589184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae19dc1738a34453d77f7c5f911344ef46fe28b96e7e88bb63d21cbdef189dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:06:01 GMT
ADD file:8534f2bd64383fee1357c8ed655d672d2fbef92507e2f11927991fbda800894c in / 
# Wed, 17 Nov 2021 02:06:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:06:14 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f099bc7a544c0fb4c5bd6b5b93da81e7b614c293d9032904d5b37dae9baefe43`  
		Last Modified: Wed, 17 Nov 2021 02:23:28 GMT  
		Size: 50.6 MB (50588959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f34119a13d10b1574733baadd3a547946864926973228efe0c3cf5565655b`  
		Last Modified: Wed, 17 Nov 2021 02:23:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:3ff5108bb89b7d0d2f533b47dcf8b7195d9c0e6505d100485a314d8e82cb395c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54464618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1f3c7bc1d2e2852613a7c84fde94ead968a9aaef007d68ccbd44d0e77c99b51`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:59 GMT
ADD file:c4d68bcae684e69a17ac01569a16c332bc925c4359383dbf3f27066f3abb295c in / 
# Wed, 17 Nov 2021 02:43:01 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:43:07 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3306c77e3ba6c6431765bbac6b0bbfb35079cfb5d567c3db405aad7687a02603`  
		Last Modified: Wed, 17 Nov 2021 02:52:02 GMT  
		Size: 54.5 MB (54464394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b268af8c50dfeb7aaf05c78db001badc1728730f4d7985c3eef1fe34ec8916`  
		Last Modified: Wed, 17 Nov 2021 02:52:13 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:6505f10cdcd1cece05d7e023a6e4bba5fefdfbe50f216fbed5cb0266f2aeb3b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56610358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1988e244454b959afd0eb10b1e149c04d3e0c725dcc6cd92c7ab7825118bb6cb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:42:57 GMT
ADD file:f97e8d450942e5807a6d08c157d8c09a86539aef93e79057b4a71919252ef9b2 in / 
# Thu, 02 Dec 2021 02:42:58 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:43:04 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e918487894f63d0afe78db5f683cd1185312e5cd115bded7a719d018c32ca4fc`  
		Last Modified: Thu, 02 Dec 2021 02:53:36 GMT  
		Size: 56.6 MB (56610135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f192783125d3dd06419c64356bf670e60b4a9307c3f65e49abef2e105a8daa`  
		Last Modified: Thu, 02 Dec 2021 02:53:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:7ee00aa23f795c51c4d67f5410de3632fe94eb73d119a7f5e49abb9d9baf2914
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54269653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041961c10f8a86f8d06df9561685284c922eb8c57efe4d0799bdf10b8c032ed0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:13:07 GMT
ADD file:f2e37e70b9a9096d2fb1678f2c206aaec8dc42e69e0036fc44f20c968ce3b6bd in / 
# Thu, 02 Dec 2021 03:13:08 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:13:15 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:31362d457f7840e760c1c73187ddb15944d8264def91872c40ba7eba7e592b20`  
		Last Modified: Thu, 02 Dec 2021 03:51:16 GMT  
		Size: 54.3 MB (54269428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6706e0fbcc3bcee354a93169c8547bf70727c39d46b1a5c5c461bf40da3eb2`  
		Last Modified: Thu, 02 Dec 2021 03:51:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:9e3c39a2c4432137da727787e18ae428ea12f36dfdf4c813a5dcd56e47a5a333
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.7 MB (59706332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c838dc60d8eadbb19b20a5d831326dc22e973f055d3f56b223b76bee02ba532e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:35:47 GMT
ADD file:6ec33732a5ce54ae880804c7d4ce9bbc89ad76007b04d23e694d60679162abdc in / 
# Wed, 17 Nov 2021 03:36:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:37:20 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1c92bc8c2e6cbcb9f02ae352b98981f7632bf82483d2ab5a0394f4a3139b3c5b`  
		Last Modified: Wed, 17 Nov 2021 04:12:49 GMT  
		Size: 59.7 MB (59706108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ef0f52d5c4aaa96e76420e8169c0b31d1d9afde93e1bf873f6dedf2e749994`  
		Last Modified: Wed, 17 Nov 2021 04:13:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:6027914093fc1280d22d7fd85f944020ee2ef5e501ca736305b88aa3c2ecc644
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53669412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e01388f51f58cd4a3bd79c8ae54a48df7add1b34ebc3161f5f1b2353e5d434`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:44:42 GMT
ADD file:6b07f3691aed718fdd31338ceb571ce22ffe4f9410f48df5c16f190258ace5ae in / 
# Wed, 17 Nov 2021 02:44:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:44:51 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1c02d7cb6bfcee3d40b1f3c9461f47e72e2f51d514b5df5ddb147d175da65910`  
		Last Modified: Wed, 17 Nov 2021 02:50:40 GMT  
		Size: 53.7 MB (53669187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1936d53cdd6ac9bc0483465e90743bf275dc82a32ddb19601dd4903c2cecba5a`  
		Last Modified: Wed, 17 Nov 2021 02:50:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
