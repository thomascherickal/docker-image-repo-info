## `debian:testing-backports`

```console
$ docker pull debian@sha256:8de63f4484cd0969af3ea529a058d389116562e118fb4252d2982cce26735403
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
$ docker pull debian@sha256:9edd2d704e33ed2e31ca8aa8dd0501d431fcc6d82bdea18f90bb288095c77451
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50668012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b663779c017d8e9cd27687a8364842ebbe2b6faff8b834ef5098ae825b52aa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:11:43 GMT
ADD file:c21d3d7908d4b616ae5afe976c1f83ac3240f71d57af0a436a192404d7dc2fe6 in / 
# Thu, 02 Dec 2021 09:11:44 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:11:57 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0b32638dc1ab8dd9d3bf82f9e41332502a0e05dc227f1b5cf3214828cd856f51`  
		Last Modified: Thu, 02 Dec 2021 09:29:18 GMT  
		Size: 50.7 MB (50667787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e420462da7f86f26ae7487c26ad036aa13ebd0999db85fb8f77fe27a2c3b1e`  
		Last Modified: Thu, 02 Dec 2021 09:29:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ed25692a44061e519127579843c14e08ab572aa6fd70cc515b757d77b8d9af7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54576680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2e6091f01c42e4890775988e64cc13a80a3bdf00083ae3b33900c3bfcb6698`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:10:33 GMT
ADD file:c995b928797291e06c5377a4387cefffc2bca18ba823a94765628b3a5074bca0 in / 
# Thu, 02 Dec 2021 08:10:34 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:10:40 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2744bb1f76af12b9eecdb60d5636bde25a46b38beb5904c55bc003677fc54351`  
		Last Modified: Thu, 02 Dec 2021 08:45:18 GMT  
		Size: 54.6 MB (54576459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc7c20312b8c6ae6ec64d235f04626312917444aade2661b4f4c85d1d8f0608`  
		Last Modified: Thu, 02 Dec 2021 08:45:28 GMT  
		Size: 221.0 B  
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
$ docker pull debian@sha256:16d1d07d7a38d7562da7bc0775020479c3548f99f050b84f146cda0a68c95edc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59851603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adb5b28a95b6b7da518860967b339da4893144798ebb43b70086f061f4ee328`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:25:01 GMT
ADD file:972506a48e285b7044e7466c1fa928ba46a90a71739476caa955522c0964e3b6 in / 
# Thu, 02 Dec 2021 07:25:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:25:22 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5f25ee39fd078e721939a7b9f385a6d99e8ecaf99aeffe635d773726e347e325`  
		Last Modified: Thu, 02 Dec 2021 07:35:23 GMT  
		Size: 59.9 MB (59851378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f683037078d613d4b5426dca3078cb3c414be896856d0b868295389793cf7c`  
		Last Modified: Thu, 02 Dec 2021 07:35:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:32494b76b2563f986f9c3360103f7196ea58d3dd629ae2aeb52d789ffc2f8dca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53866937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:161f6c59c63c448d5995a22cb0104abde5bc8424351178b627f37fadc90e6940`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:22 GMT
ADD file:6a348f1b2d54149be6cf0ba3d61716a2dcc60830baaf5b96fbcf071b49b2299c in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:21:32 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c913837051836292f57261b37a6bad47f00975da0878d1c5c435a411dceaab93`  
		Last Modified: Thu, 02 Dec 2021 07:27:16 GMT  
		Size: 53.9 MB (53866716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f946626c4017e0959d0fa7f1478f70bbf1245bbc3282bbc86b280c0fb7127de`  
		Last Modified: Thu, 02 Dec 2021 07:27:22 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
