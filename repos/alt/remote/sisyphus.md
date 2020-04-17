## `alt:sisyphus`

```console
$ docker pull alt@sha256:520e297b77477433c2ad9c1d59d2236df3a5aeb60e0545e5cf84ae16544988f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:sisyphus` - linux; amd64

```console
$ docker pull alt@sha256:b38012f5a92bbe2bd1ce9d9a652cead4415dd9b95dea8360b1f52e72664c466f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42516711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0255885cb0fa2b6c8c9ebe19455053f5cd1047ad1aa164ce730b17f529fc3aa9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Sep 2018 21:19:34 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:21:15 GMT
ADD file:bdc95de4a2134b26633b0cf33f5ea909da0ec8c98d5450ee3d16996b2dc91968 in / 
# Fri, 17 Apr 2020 20:21:16 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:21:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a486e48e06c564fc25aea11e4075c481d81cfefac16ca8154834d8f788da5fe3`  
		Last Modified: Fri, 17 Apr 2020 20:22:30 GMT  
		Size: 42.5 MB (42516529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f854ecf46147bf3123f7664e92b805a3f98c0a02fd0a4d89c326842aab345aa`  
		Last Modified: Fri, 17 Apr 2020 20:21:47 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:87f7d21699475e321a001066e06b5be08b4d2e032edf2223baa52cfa74d415d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41450509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d50d2c032633af162388d7f2b0d9c6e973b4f4c17bc4d4c20f8d17d38795f901`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 May 2019 22:39:34 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:53:09 GMT
ADD file:f6ed3d9bba90a1e88e3f18bf780263eb99e8832d4f55be40a217b2742dca5e69 in / 
# Fri, 17 Apr 2020 20:53:13 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:53:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fb95dca6947e373b5fa76230a7fbd765112dcd69cb8b68725c25f57a89ca6569`  
		Last Modified: Fri, 17 Apr 2020 20:53:52 GMT  
		Size: 41.5 MB (41450326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1a64449e3977f1a6ae25332e0350bd729b16d84690697d0a6212d1e995b9da`  
		Last Modified: Fri, 17 Apr 2020 20:53:41 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; 386

```console
$ docker pull alt@sha256:3d580a5c9fda073d808a5cec6b5eb70d4b8c5568ec541fa678ec9e10bcc0e582
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (42983776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf66fd79e0268d31b1e3a2dbc228e38a66bf4623db248a0dd744b065b9f4712`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Sep 2018 10:38:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:39:32 GMT
ADD file:7e9203f8033407ce397c14c2cf32e0cd3e453e17f1dc5237945a3f771c21eca0 in / 
# Fri, 17 Apr 2020 20:39:33 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:39:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:71721a1bdd8f1dae99dcd35ef8fbaeccf05fb70a020f31529f397affbccad29f`  
		Last Modified: Fri, 17 Apr 2020 20:40:35 GMT  
		Size: 43.0 MB (42983595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3b229641aed5df96ba41d6074fffb4c1ce979a6607aa7bcbb34c305d598e48`  
		Last Modified: Fri, 17 Apr 2020 20:40:09 GMT  
		Size: 181.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; ppc64le

```console
$ docker pull alt@sha256:50dbab36635fe39ce0478d51359af0bacead1c871e7d0410db1112e2b2b444e2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45980294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b9a706fcc943446923d69f5e44bcec1e2324f64fd2c73c3cd827d7d5ce9b7a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Jul 2019 23:03:07 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 13 Dec 2019 23:28:56 GMT
ADD file:775e42d8b94f8000aa91f09e044d81512bb39d132cd55da96571e659201dd341 in / 
# Fri, 13 Dec 2019 23:29:02 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 13 Dec 2019 23:29:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f21e5c19aa4a0e8af2854d79a47810deda11e779c7915a8b6a8821328bbf5593`  
		Last Modified: Fri, 13 Dec 2019 23:30:10 GMT  
		Size: 46.0 MB (45980108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4252e9e543879b0cb367d932e4e2e201c9056b919e3588a12bde9cfae0ea717`  
		Last Modified: Fri, 13 Dec 2019 23:30:00 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
