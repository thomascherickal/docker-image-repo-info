<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `alt`

-	[`alt:latest`](#altlatest)
-	[`alt:p8`](#altp8)
-	[`alt:p9`](#altp9)
-	[`alt:sisyphus`](#altsisyphus)

## `alt:latest`

```console
$ docker pull alt@sha256:7d9aeee98ab20ca73dd7447fa467b62b90a6445aff4f18edc447639b230f26eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:latest` - linux; amd64

```console
$ docker pull alt@sha256:f0f4c74168b712cc7f1953cb106cb99d1ff94a9a3ba63e5f3aa730823637ef9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42402845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa7a4e7b43b8c39804edcc28d3c9054b6946d73cce1ff7f70df62a64a2faec8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Sep 2018 21:19:34 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:20:30 GMT
ADD file:2d06afea910d9968616d800ef8051c9a310341a5ebf7d6e2d0e8dcc35dacb369 in / 
# Fri, 17 Apr 2020 20:20:31 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:20:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a7f990b672518341cc3ab2b0ca77d33a1e5241443f33558b19b6dce765b8787d`  
		Last Modified: Fri, 17 Apr 2020 20:21:32 GMT  
		Size: 42.4 MB (42402665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d15b4d031b574e5e8a9e108544c242a42b4317b3fd2b07a00c0ec81c91beda`  
		Last Modified: Fri, 17 Apr 2020 20:21:23 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:3048ec6af4886a3a96f2347f154e54706e24f5e92008eb16b41b3674ac3030ff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41196983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cc17b1cc026b8a31b396a884b75cd3487eb0940538184d41d790cf2febe6224`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 May 2019 22:39:34 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:52:40 GMT
ADD file:610dad395b67002fb5c133f808e9f29a836033d66440ce1d52258b39e46077d6 in / 
# Fri, 17 Apr 2020 20:52:45 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:52:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:989db8cdbac34d0dcdffe069780f9fd0b9e681bf6645164168e6ed5fc7a7e789`  
		Last Modified: Fri, 17 Apr 2020 20:53:35 GMT  
		Size: 41.2 MB (41196800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5b93c0c1d774cce81cb8b2eda896d36078e9937265045912c3ed2bd411472`  
		Last Modified: Fri, 17 Apr 2020 20:53:25 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; 386

```console
$ docker pull alt@sha256:bcd8de279ee81103614114c64f9201bde7210c1e5cd1b297742ce55073bbc686
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42594068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88f07dc7c31927bcd60847ca77541db74722d89a276229db5267ec7216420503`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Sep 2018 10:38:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:38:55 GMT
ADD file:6b64bdf711a63686f6ed2662d9a257fb7229f8b2a94edf0744e3d9bf6b1d046a in / 
# Fri, 17 Apr 2020 20:38:56 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:38:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3e67baf00d718ba790dde80ef3b86d68fec111df67c570a0fe26054ae56052e1`  
		Last Modified: Fri, 17 Apr 2020 20:39:51 GMT  
		Size: 42.6 MB (42593886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139b377770205804800b11d89a62f3eaa537e26ea26340db484a81a4f41490e7`  
		Last Modified: Fri, 17 Apr 2020 20:39:41 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; ppc64le

```console
$ docker pull alt@sha256:f2e8120c80334f416ec7ee95a9d880fd80ef73227735df9649e677c06d8afc8a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45973743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4804e3516b5055eb4b2dc26114e5499f803d84e4fc6e6bd18b6b304df3039bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Jul 2019 23:03:07 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 13 Dec 2019 23:27:07 GMT
ADD file:76539c1d57a239f951036e0c316cdb655660941707c2748325601fe0d1785b14 in / 
# Fri, 13 Dec 2019 23:27:15 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 13 Dec 2019 23:27:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a30f2ba42b32764b713c7c27eee458486aa98158488c2dc7f88333cc429d60d7`  
		Last Modified: Fri, 13 Dec 2019 23:29:50 GMT  
		Size: 46.0 MB (45973559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd676883cee989b61541e0e6ae7e898fb317fe2335a4d5aaa86d4da3de308464`  
		Last Modified: Fri, 13 Dec 2019 23:29:27 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `alt:p8`

```console
$ docker pull alt@sha256:1bc52054d21c4163d2fa8c4608f2074dc6fb7b7cff7e3d4070fc21b9a7b465d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386

### `alt:p8` - linux; amd64

```console
$ docker pull alt@sha256:c9abe92b0cfb4db927be600f8418249a12713ad6146552d0345767e05a77245b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35783815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f898227d4fe17e5abdc0353f47728e4f988bc255f934801e979a7285cc05d4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Sep 2018 21:19:34 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:20:56 GMT
ADD file:f72c839d28157bfc5dff9fd80bbc88facdf6b16e8aa7e671e472032dfd2d9dbd in / 
# Fri, 17 Apr 2020 20:20:57 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:20:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0b02a1fa02d3e924b7f7543dacf1159e7fbecc6c3b49910697751e5e884aa188`  
		Last Modified: Fri, 17 Apr 2020 20:21:43 GMT  
		Size: 35.8 MB (35783635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fdf19384ef2e48550acc53d92ecbba1353f7521cb7c7ef07e21af235907cb3`  
		Last Modified: Fri, 17 Apr 2020 20:21:37 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p8` - linux; 386

```console
$ docker pull alt@sha256:00309a30a09de55b43b6cb09033a2409d57595eca9c399c9a77fac54a57735aa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35940680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec492149008b874a3bc6e6661c45a9942043ce13f8405585a496646d6e62d4f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Sep 2018 10:38:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:39:13 GMT
ADD file:fbf04a50b6ecd44ec455383f64fc5cf4f089d7fc895caee88dc0dadfce000166 in / 
# Fri, 17 Apr 2020 20:39:13 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:39:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:68b9ef91f33e3125d2500957556b9e9fbd7dceabb7bd4ef2f85eb2173941a20e`  
		Last Modified: Fri, 17 Apr 2020 20:40:04 GMT  
		Size: 35.9 MB (35940499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ac4d1342ef06f596e5aca1e277825deaa7ce8dbb1bdcf835be64302a1f372`  
		Last Modified: Fri, 17 Apr 2020 20:39:56 GMT  
		Size: 181.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `alt:p9`

```console
$ docker pull alt@sha256:7d9aeee98ab20ca73dd7447fa467b62b90a6445aff4f18edc447639b230f26eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:p9` - linux; amd64

```console
$ docker pull alt@sha256:f0f4c74168b712cc7f1953cb106cb99d1ff94a9a3ba63e5f3aa730823637ef9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42402845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa7a4e7b43b8c39804edcc28d3c9054b6946d73cce1ff7f70df62a64a2faec8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Sep 2018 21:19:34 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:20:30 GMT
ADD file:2d06afea910d9968616d800ef8051c9a310341a5ebf7d6e2d0e8dcc35dacb369 in / 
# Fri, 17 Apr 2020 20:20:31 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:20:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a7f990b672518341cc3ab2b0ca77d33a1e5241443f33558b19b6dce765b8787d`  
		Last Modified: Fri, 17 Apr 2020 20:21:32 GMT  
		Size: 42.4 MB (42402665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d15b4d031b574e5e8a9e108544c242a42b4317b3fd2b07a00c0ec81c91beda`  
		Last Modified: Fri, 17 Apr 2020 20:21:23 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:3048ec6af4886a3a96f2347f154e54706e24f5e92008eb16b41b3674ac3030ff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41196983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cc17b1cc026b8a31b396a884b75cd3487eb0940538184d41d790cf2febe6224`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 May 2019 22:39:34 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:52:40 GMT
ADD file:610dad395b67002fb5c133f808e9f29a836033d66440ce1d52258b39e46077d6 in / 
# Fri, 17 Apr 2020 20:52:45 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:52:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:989db8cdbac34d0dcdffe069780f9fd0b9e681bf6645164168e6ed5fc7a7e789`  
		Last Modified: Fri, 17 Apr 2020 20:53:35 GMT  
		Size: 41.2 MB (41196800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5b93c0c1d774cce81cb8b2eda896d36078e9937265045912c3ed2bd411472`  
		Last Modified: Fri, 17 Apr 2020 20:53:25 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; 386

```console
$ docker pull alt@sha256:bcd8de279ee81103614114c64f9201bde7210c1e5cd1b297742ce55073bbc686
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42594068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88f07dc7c31927bcd60847ca77541db74722d89a276229db5267ec7216420503`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Sep 2018 10:38:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 17 Apr 2020 20:38:55 GMT
ADD file:6b64bdf711a63686f6ed2662d9a257fb7229f8b2a94edf0744e3d9bf6b1d046a in / 
# Fri, 17 Apr 2020 20:38:56 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 17 Apr 2020 20:38:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3e67baf00d718ba790dde80ef3b86d68fec111df67c570a0fe26054ae56052e1`  
		Last Modified: Fri, 17 Apr 2020 20:39:51 GMT  
		Size: 42.6 MB (42593886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139b377770205804800b11d89a62f3eaa537e26ea26340db484a81a4f41490e7`  
		Last Modified: Fri, 17 Apr 2020 20:39:41 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; ppc64le

```console
$ docker pull alt@sha256:f2e8120c80334f416ec7ee95a9d880fd80ef73227735df9649e677c06d8afc8a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45973743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4804e3516b5055eb4b2dc26114e5499f803d84e4fc6e6bd18b6b304df3039bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Jul 2019 23:03:07 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 13 Dec 2019 23:27:07 GMT
ADD file:76539c1d57a239f951036e0c316cdb655660941707c2748325601fe0d1785b14 in / 
# Fri, 13 Dec 2019 23:27:15 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 13 Dec 2019 23:27:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a30f2ba42b32764b713c7c27eee458486aa98158488c2dc7f88333cc429d60d7`  
		Last Modified: Fri, 13 Dec 2019 23:29:50 GMT  
		Size: 46.0 MB (45973559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd676883cee989b61541e0e6ae7e898fb317fe2335a4d5aaa86d4da3de308464`  
		Last Modified: Fri, 13 Dec 2019 23:29:27 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
