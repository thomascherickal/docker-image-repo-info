## `debian:stable-backports`

```console
$ docker pull debian@sha256:681f6d7332ce3f6f3cc53d3842e121b60f9b5374f5f22be6419b5149bced35a8
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:5e0d22221a9fca83d524fe85ddd6d87349e65ce562ec82c9fdb0595c9422c7fe
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50379973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d36dfd4232772a52e7aaf5f0270be3a56ec87ff78eebf3df16e27ae53122e52`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:08 GMT
ADD file:f94f55e18dff5677127aef59d338291f4cb49ddc479dbfb75e9f4473b56be40e in / 
# Sat, 28 Dec 2019 04:23:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:23:12 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:26f29d119cd154d3576d9831feb9ece7ac44f100cc089d0addf415956b8c0897`  
		Last Modified: Sat, 28 Dec 2019 04:27:42 GMT  
		Size: 50.4 MB (50379751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94881092e682ba24cc9a4a8ac182c08ff3748ab38fa595ffb17314579aeb50f4`  
		Last Modified: Sat, 28 Dec 2019 04:28:03 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:206dbfbea7813058bfa6f4140c2a5ef337eb271941788b8c79565ef9bbb67b16
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48092968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45e60f183023eceb7c96bf4b01ee8559d279907d792887c64f4ff05445d2c64f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 12:17:11 GMT
ADD file:651423dc864f1a0e0d284d81bd5286a72fccbf035f6bafbf116d6566647cc65b in / 
# Fri, 22 Nov 2019 12:17:15 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 12:17:25 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:93d286de8d4df64da5e15abc5957795a90d0cc9ad7c62dbef7cd75650e06fdc9`  
		Last Modified: Fri, 22 Nov 2019 12:25:19 GMT  
		Size: 48.1 MB (48092745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba515e62c6b744f2db0bcea3e29005ed8282c2522487f0a00cbbcfd74e759a0`  
		Last Modified: Fri, 22 Nov 2019 12:25:27 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:a2c5efca930a283d601137af9ed5a9079b83b51f3ca8b9556bdbfa7cc2bc4504
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45859709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:704d5b77762c2cf797c48bdc6db5f4f83ea02aada1a15671f402be6d53176baa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:26:52 GMT
ADD file:9113ebfe142e9cbdad49916337875ce990928a7c519adba0db0658c3f36082a6 in / 
# Fri, 22 Nov 2019 13:26:54 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 13:27:05 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3834b9595366c6d19dfdaf7cbda700f30f9d3894a193f73369bf9aab76deb9b7`  
		Last Modified: Fri, 22 Nov 2019 13:36:03 GMT  
		Size: 45.9 MB (45859485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1497c096b2aed8467c6759eb1fb69b339a49ec28ed875abca3fba2040b4038f`  
		Last Modified: Fri, 22 Nov 2019 13:36:13 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:0a8fa2b107ffdc46e0af1cca7bdccd314fd00f30e32b8bbb2db6206c762e61eb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49172101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29287c4828a7a20b632b257b8cb6243aef2bd90f6bf6801b6f59e6ebcb7fa595`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:35 GMT
ADD file:2a28113dc8599cfed44c7ea0b96a70c896de6f31d247a820a5d1aa319981ef07 in / 
# Sat, 28 Dec 2019 04:42:37 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:42:45 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:57c34c57333da71c871bb243bd02a0332a7b74ecd6713673f6f20ba6f906c446`  
		Last Modified: Sat, 28 Dec 2019 04:48:21 GMT  
		Size: 49.2 MB (49171877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6987570a6ba82c20d2f9240c51c7453fe7f2a4a8fa937a056ce9c03946d723f`  
		Last Modified: Sat, 28 Dec 2019 04:48:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:6d0574a53d394d7c698babf6a096478542b151cc6459d4a5beffc349a93522ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51142187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72c81d2b4ecf1c7424aed2533892a75660099c9138a54dc5e09ffae295b6a8fb`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:24 GMT
ADD file:eaa22b066ca93ab6762445b5b8365ac221e6fa251ca8ec7bcb06dfa00f82950e in / 
# Sat, 28 Dec 2019 04:41:25 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:41:30 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:402d97e3c1d2a14a3fd18d4c01a160f5576609718b3ab91e9d7b69fe8f3d8229`  
		Last Modified: Sat, 28 Dec 2019 04:46:46 GMT  
		Size: 51.1 MB (51141963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee56dbc43ac31e0e79cea61740713f7f7d9a12da5f25182cc6845e427a859e8`  
		Last Modified: Sat, 28 Dec 2019 04:46:54 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:b9f9f03103850c1322cd6154760499d5e6794cbc618270c4a8dbf67cb2380a10
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54132700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33cfb2cc723499016f2d7d6029bc9b25c08a24b93ede95fedcdaf4b2c2d5c498`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:22:17 GMT
ADD file:70fde2369d9aff91dda4f63e76102e7b39c8ee1d05e696c2c8d8dba151729bff in / 
# Sat, 28 Dec 2019 04:22:22 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:22:31 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7198e2ee3f566710433570c82853cb455a5ab2156d93f10580d394a9936dcb17`  
		Last Modified: Sat, 28 Dec 2019 04:31:16 GMT  
		Size: 54.1 MB (54132476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2485f19ad09e10601e933061e617d418414ae90915663d8d5e68270ef2045b`  
		Last Modified: Sat, 28 Dec 2019 04:31:27 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:1ef041db0920125d020d64e4506b22f15cce1bf11d6e4c652f7d09be6e10cbd6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48954737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0ec1af2c696c43745e4a49c0f19e0ab30db0f47a938f8a2fd86b03e474aede9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:48 GMT
ADD file:ad464e5104d7ebd85331c7da273bed2b89dba5d941ebde5613a57ac784c2e199 in / 
# Sat, 28 Dec 2019 04:42:48 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:42:53 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ccace6770a91bd4b95ab45776712a901405bc4595be38e130b67d316618f53d3`  
		Last Modified: Sat, 28 Dec 2019 04:46:02 GMT  
		Size: 49.0 MB (48954515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d768d44b5d753f8b5da3504d7357ee49a6aa54bd8d72e9d7cb266b6e016b9875`  
		Last Modified: Sat, 28 Dec 2019 04:46:07 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
