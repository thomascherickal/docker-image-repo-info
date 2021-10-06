<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `alt`

-	[`alt:latest`](#altlatest)
-	[`alt:p10`](#altp10)
-	[`alt:p9`](#altp9)
-	[`alt:sisyphus`](#altsisyphus)

## `alt:latest`

```console
$ docker pull alt@sha256:f319bf0a20159c4f264f523d22974d5343f34d22048a56ff84cf3160e3f8db4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:latest` - linux; amd64

```console
$ docker pull alt@sha256:273a48ec7b1cda9be55fd7ae344c7c00d92ab925e40c871705861eb523107e4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41819986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9738cf9e9ed3c895c1252ea483a3b346026268532290548425045aa33bbf4451`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:19:46 GMT
ADD file:f3865144ef386c3910ffd911a2b8505180236b68aeb88d5930269e460a893be2 in / 
# Tue, 05 Oct 2021 22:19:47 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:19:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:89621db199c966be4c1eb1c9225983a5095f5809450540f8bd7250effcc71a92`  
		Last Modified: Tue, 05 Oct 2021 22:20:28 GMT  
		Size: 41.8 MB (41819794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7686f1e15c306644b670ab5796d2f33309b1e868cc1160cc23bf5bbb6ca352e4`  
		Last Modified: Tue, 05 Oct 2021 22:20:22 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; arm variant v7

```console
$ docker pull alt@sha256:a4a96b729dffcd9b441fc14da2c5a353f1b93a3feb9dfc19fe23af0b83d29ae3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38332677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:760beb8601f1b4ac7c807c45a70bbeb12ec6246a35893e7c06a2b55c23d7a0ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Aug 2021 01:09:27 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 23:33:24 GMT
ADD file:80838ae4de0e57fcd0cd5c94e14c588b9ac349846b7eee40c2ef3172ba0a339c in / 
# Tue, 05 Oct 2021 23:33:26 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 23:33:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7dac9cc917bc180b25a52242dacd876281dce4656dd61dc65170b4bd77d12d54`  
		Last Modified: Tue, 05 Oct 2021 23:35:10 GMT  
		Size: 38.3 MB (38332485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890adc6381b2623995ce251dbba0122ce5adec6d5b928a170b53c9b4c53f186b`  
		Last Modified: Tue, 05 Oct 2021 23:34:46 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:cae253d247a47d098e72f009db3fc9b75f748fbd7766528f834fa97df0f94d01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40803855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef382274d41e0c4976b427d2a4d451f41e960def6d834a08654f556bed57983`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 23:11:19 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:39:48 GMT
ADD file:2e8b90a92499ef5adf1d8e269489f5200db1e84d2ca1343e1cd8a3bfa3a55234 in / 
# Tue, 05 Oct 2021 22:39:50 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:39:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:aa6113068268a552f8c4dd6f1a26ad0a46bbaeef09546674e95c1c0486a00c44`  
		Last Modified: Tue, 05 Oct 2021 22:40:33 GMT  
		Size: 40.8 MB (40803663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee086f6d364c7f7ee7f0ca591bdba7490bee9f03884754e2b5452a8b1c5934c`  
		Last Modified: Tue, 05 Oct 2021 22:40:27 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; 386

```console
$ docker pull alt@sha256:46dc4854afa63ab93315076e344158d391225dfeb47bccdaa21a1d0e5854eab7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42530199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0a3f2d315b2208e0d588b57c95595d836c167a88b19309bc286f54df838841`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:45:24 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:38:31 GMT
ADD file:70d38e61326d67a3511ba7a891499ef9b0ab4c12dcd6366cb244194af52ef01c in / 
# Tue, 05 Oct 2021 22:38:32 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:38:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec73ddddf89886a88827955c9a8bbc4c944ceea5315338d49e5f620c682164cf`  
		Last Modified: Tue, 05 Oct 2021 22:39:22 GMT  
		Size: 42.5 MB (42530006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4638dbdd87db8e166f5b39241ff1fde618a6d0e5287b7a9e4e86266a9bd70e64`  
		Last Modified: Tue, 05 Oct 2021 22:39:14 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; ppc64le

```console
$ docker pull alt@sha256:61c9c02cfe35ac11726b5c850cfa6be5fcd31ea9325bb213a09f6a5238c4c747
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44557045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe54aa9c7b485ccbfa9a2974afa7b8ed9426ea9f351290ea85375d307443168`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 04 Aug 2021 22:29:49 GMT
ADD file:c0cd9d49037aa84f41061f2bc69c1ce6def0cf8a453db5967e378191c2afd062 in / 
# Wed, 04 Aug 2021 22:30:01 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 04 Aug 2021 22:30:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:caade519083556b1282dc1b002629dc83c9ad67894d39430973b00ca5c7263bd`  
		Last Modified: Wed, 04 Aug 2021 22:32:02 GMT  
		Size: 44.6 MB (44556853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5065b57674751c1c42172e0a6e5d6661c55821c1c9a746a1b869ab7a925f5cbc`  
		Last Modified: Wed, 04 Aug 2021 22:31:53 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `alt:p10`

```console
$ docker pull alt@sha256:f319bf0a20159c4f264f523d22974d5343f34d22048a56ff84cf3160e3f8db4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:p10` - linux; amd64

```console
$ docker pull alt@sha256:273a48ec7b1cda9be55fd7ae344c7c00d92ab925e40c871705861eb523107e4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41819986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9738cf9e9ed3c895c1252ea483a3b346026268532290548425045aa33bbf4451`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:19:46 GMT
ADD file:f3865144ef386c3910ffd911a2b8505180236b68aeb88d5930269e460a893be2 in / 
# Tue, 05 Oct 2021 22:19:47 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:19:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:89621db199c966be4c1eb1c9225983a5095f5809450540f8bd7250effcc71a92`  
		Last Modified: Tue, 05 Oct 2021 22:20:28 GMT  
		Size: 41.8 MB (41819794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7686f1e15c306644b670ab5796d2f33309b1e868cc1160cc23bf5bbb6ca352e4`  
		Last Modified: Tue, 05 Oct 2021 22:20:22 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p10` - linux; arm variant v7

```console
$ docker pull alt@sha256:a4a96b729dffcd9b441fc14da2c5a353f1b93a3feb9dfc19fe23af0b83d29ae3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38332677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:760beb8601f1b4ac7c807c45a70bbeb12ec6246a35893e7c06a2b55c23d7a0ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Aug 2021 01:09:27 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 23:33:24 GMT
ADD file:80838ae4de0e57fcd0cd5c94e14c588b9ac349846b7eee40c2ef3172ba0a339c in / 
# Tue, 05 Oct 2021 23:33:26 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 23:33:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7dac9cc917bc180b25a52242dacd876281dce4656dd61dc65170b4bd77d12d54`  
		Last Modified: Tue, 05 Oct 2021 23:35:10 GMT  
		Size: 38.3 MB (38332485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890adc6381b2623995ce251dbba0122ce5adec6d5b928a170b53c9b4c53f186b`  
		Last Modified: Tue, 05 Oct 2021 23:34:46 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p10` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:cae253d247a47d098e72f009db3fc9b75f748fbd7766528f834fa97df0f94d01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40803855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef382274d41e0c4976b427d2a4d451f41e960def6d834a08654f556bed57983`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 23:11:19 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:39:48 GMT
ADD file:2e8b90a92499ef5adf1d8e269489f5200db1e84d2ca1343e1cd8a3bfa3a55234 in / 
# Tue, 05 Oct 2021 22:39:50 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:39:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:aa6113068268a552f8c4dd6f1a26ad0a46bbaeef09546674e95c1c0486a00c44`  
		Last Modified: Tue, 05 Oct 2021 22:40:33 GMT  
		Size: 40.8 MB (40803663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee086f6d364c7f7ee7f0ca591bdba7490bee9f03884754e2b5452a8b1c5934c`  
		Last Modified: Tue, 05 Oct 2021 22:40:27 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p10` - linux; 386

```console
$ docker pull alt@sha256:46dc4854afa63ab93315076e344158d391225dfeb47bccdaa21a1d0e5854eab7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42530199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0a3f2d315b2208e0d588b57c95595d836c167a88b19309bc286f54df838841`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:45:24 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:38:31 GMT
ADD file:70d38e61326d67a3511ba7a891499ef9b0ab4c12dcd6366cb244194af52ef01c in / 
# Tue, 05 Oct 2021 22:38:32 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:38:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec73ddddf89886a88827955c9a8bbc4c944ceea5315338d49e5f620c682164cf`  
		Last Modified: Tue, 05 Oct 2021 22:39:22 GMT  
		Size: 42.5 MB (42530006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4638dbdd87db8e166f5b39241ff1fde618a6d0e5287b7a9e4e86266a9bd70e64`  
		Last Modified: Tue, 05 Oct 2021 22:39:14 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p10` - linux; ppc64le

```console
$ docker pull alt@sha256:61c9c02cfe35ac11726b5c850cfa6be5fcd31ea9325bb213a09f6a5238c4c747
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44557045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe54aa9c7b485ccbfa9a2974afa7b8ed9426ea9f351290ea85375d307443168`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 04 Aug 2021 22:29:49 GMT
ADD file:c0cd9d49037aa84f41061f2bc69c1ce6def0cf8a453db5967e378191c2afd062 in / 
# Wed, 04 Aug 2021 22:30:01 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 04 Aug 2021 22:30:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:caade519083556b1282dc1b002629dc83c9ad67894d39430973b00ca5c7263bd`  
		Last Modified: Wed, 04 Aug 2021 22:32:02 GMT  
		Size: 44.6 MB (44556853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5065b57674751c1c42172e0a6e5d6661c55821c1c9a746a1b869ab7a925f5cbc`  
		Last Modified: Wed, 04 Aug 2021 22:31:53 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `alt:p9`

```console
$ docker pull alt@sha256:f7ddb07eb44448d92b979f3bd8c6fba01990dbf743e9d5123ed051b38c317544
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:p9` - linux; amd64

```console
$ docker pull alt@sha256:363b19cb7b121457fdd8bc2e6a5be06786b7e0c8b85ddd62186ff36c988c02ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43022306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aff04ca5584f1b8ace436cf9d50ad6030df241de03912e6e8c6386702468fa9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:19:57 GMT
ADD file:a2e4594a7d07230a9a39142be3b186579cefa9417af1df4c4dee2f1741d1f8c1 in / 
# Tue, 05 Oct 2021 22:19:58 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:19:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8b8c6c608e36948d375afa16bf949132d9db690bd9b744e93d49c504c6384b50`  
		Last Modified: Tue, 05 Oct 2021 22:20:44 GMT  
		Size: 43.0 MB (43022114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfc4e4cf0b1f52711152f1fde173f673d19300daaed5d624c06e54fd5ff0198`  
		Last Modified: Tue, 05 Oct 2021 22:20:38 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; arm variant v7

```console
$ docker pull alt@sha256:9b88e1fa50a3e983f6b932aefbff014fd813261207fcc04157c0c9b9eaf79684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.5 MB (38545311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034d5f55eb45f6c747faa1a15a0fc150635de8dfeda7380fb88f7fa22e743250`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Aug 2021 01:09:27 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 23:33:49 GMT
ADD file:fcc83adb58f3a46f5ac12295a9f89719572cc3886c1a6474345f4d8a181897ca in / 
# Tue, 05 Oct 2021 23:33:51 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 23:33:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:28402cc088b7b49062dc9e39326e1d792d4cdf2c867868202d3398531252adab`  
		Last Modified: Tue, 05 Oct 2021 23:35:45 GMT  
		Size: 38.5 MB (38545119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb0b56eda2cd08f4cbd4236582e0ed0592a1f410d77d583f526a0098a2d8373`  
		Last Modified: Tue, 05 Oct 2021 23:35:21 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:c24fabad0236cec12a9b6d3991e43b6d485d13e9dee9a26af2875043af19b27d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41825580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74c7ae3299d4518d729c72d7b307d211320ea9192a55a06b984140b320ea8c17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 23:11:19 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:39:59 GMT
ADD file:2c2c793c2e8f13e0de6eb1c1fd9fc4c3d144788c2bcc6b5bc5b4c8470fadaf76 in / 
# Tue, 05 Oct 2021 22:40:00 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:40:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e9fda4b2447af251b42f42b86d973f1e5492f6ef14b11214eed99edbf9408f4`  
		Last Modified: Tue, 05 Oct 2021 22:40:51 GMT  
		Size: 41.8 MB (41825390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07d1e3bfc14ea981d8e8131f71fa4acf5fe472cb8d0ccf4027bf49e7a9f0e07`  
		Last Modified: Tue, 05 Oct 2021 22:40:45 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; 386

```console
$ docker pull alt@sha256:1d3bfdc0a76a072ae72c099a4ee5c4b05c90b41cf9daa2989fcc6f740e5a2664
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43181331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df32fb43c13f02cafeba6639df2367768af4765d40f2955f1b3c115a7af30311`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:45:24 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:38:44 GMT
ADD file:0081382266a20ae24e7de9c2c9932c67cc5110618b5625677ebde995e706bdf2 in / 
# Tue, 05 Oct 2021 22:38:45 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:38:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:42ed55dd8afdefbfcebacf9aa7bdd30efe08b1e943df7a71645df99e15cb4202`  
		Last Modified: Tue, 05 Oct 2021 22:39:42 GMT  
		Size: 43.2 MB (43181139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9ba6b64e4777a0244beb6f617952422f7ce11d918ec6599c6a2047adb8a01d`  
		Last Modified: Tue, 05 Oct 2021 22:39:33 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; ppc64le

```console
$ docker pull alt@sha256:a4c67025e48578cd93f73cc910aedc1176fd8514f272bd34c828ee0968687d31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46747248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0041eee6c38a6ac13380da96fd266fd924e59cb41c36a8a9c36f5ae302c8c9ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 04 Aug 2021 22:30:21 GMT
ADD file:c7156556f06790bef780e9ac667dfb71575fc3d6de32806eb89b932da531371a in / 
# Wed, 04 Aug 2021 22:30:35 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 04 Aug 2021 22:30:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3f69242dd4b35de85d5bed5c0f717dbf369c318e52ef194b0b56d890e03e35fa`  
		Last Modified: Wed, 04 Aug 2021 22:32:26 GMT  
		Size: 46.7 MB (46747054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b137d08f9daa2012daa2768e9f2652de7817f2e7b51399fd96dda09c7c054f5`  
		Last Modified: Wed, 04 Aug 2021 22:32:17 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `alt:sisyphus`

```console
$ docker pull alt@sha256:4a6a1cb89556f2c9f67d1cfb78ced1d9a937d2945ffeb5b43f544b4ac18e50da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:sisyphus` - linux; amd64

```console
$ docker pull alt@sha256:23d121ff1f0b4899779c115ed13a56d0f544574980126876caecf345f2b27f19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41968262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bd6443c924637e2d4eb570114dd8bb8f4037a03eb6bfcbe238f63431dd78058`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:20:08 GMT
ADD file:23a11d42a1efc414b56e2d0a970b9da6fe85f102f3c2ee6b9ea3842b5151005a in / 
# Tue, 05 Oct 2021 22:20:09 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:20:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2de1ef13e503da8b2ce4b9e2a12d52f082c57f13e729689bec0b3c4604dcf8d9`  
		Last Modified: Tue, 05 Oct 2021 22:20:57 GMT  
		Size: 42.0 MB (41968071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecde41fa05fcbc2bc7461093004f57f8fd6e30bc7ef43b20963399360463d2bd`  
		Last Modified: Tue, 05 Oct 2021 22:20:51 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; arm variant v7

```console
$ docker pull alt@sha256:ac254326f3164ad22fe7316467216248f7d0f16db2627007d6f3927814d22b38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38612193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bedbdc06e247944b408566081f1690e8d2c238088e81090cac6ddec54aaebd19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Aug 2021 01:09:27 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 23:34:14 GMT
ADD file:ee81978960b88085534d7c9ab24b43471bdb4660457e01483c19cbb904785b68 in / 
# Tue, 05 Oct 2021 23:34:16 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 23:34:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9eedb6a57e4fcd96fe2b31e3babcd6646646ac83cf8f53408d1764762e1167b7`  
		Last Modified: Tue, 05 Oct 2021 23:36:17 GMT  
		Size: 38.6 MB (38612001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af7c6ccc545015c27c428ff91bfea82868a8947ec66360a840e9ae01424f555`  
		Last Modified: Tue, 05 Oct 2021 23:35:53 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:67eba06940960a171938e546beb23a4f44bfddc196aec900383cd8127835bc22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40859960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87692fceca9c314268b1dee8fea1dbcd6e13d28d22f6b28c410202b5cf6ace6e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 23:11:19 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:40:08 GMT
ADD file:ee5acfecc85907b2402d0c02fb3760cd403cd3ea494773ef5c09fd351a71b31b in / 
# Tue, 05 Oct 2021 22:40:09 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:40:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:460ce4384fed12be2e1b021107561ee35cd1ec59424cc3bd30ed6dcb4487b021`  
		Last Modified: Tue, 05 Oct 2021 22:41:06 GMT  
		Size: 40.9 MB (40859768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc47075c25e9a725558ec066bd3e8fecbd5bfff1a91ccc97a3d3d9cd9508c423`  
		Last Modified: Tue, 05 Oct 2021 22:41:00 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; 386

```console
$ docker pull alt@sha256:f43752a433a92dc3e6f648b39a3b974959883ff0bc346ed53785b5b516b13e51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42460143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0ba0ef2c42f463fcacfe5b27b817cdba53ffc621e16d44284f118c9f495ce3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:45:24 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:38:56 GMT
ADD file:618e851010a6813dee96534552c96c3fb71dd6158ad79094182d2ec0c7bdafe8 in / 
# Tue, 05 Oct 2021 22:38:58 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:38:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f8f1b43b3fcfdd7da6037fee94e91acd8f8a01ea20f655495873b40b58004a46`  
		Last Modified: Tue, 05 Oct 2021 22:39:58 GMT  
		Size: 42.5 MB (42459954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3743ac4a7595caf6f43fa10b4f926c6dfa97e4f48bc21fcd5c0afdc07d38f48`  
		Last Modified: Tue, 05 Oct 2021 22:39:49 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; ppc64le

```console
$ docker pull alt@sha256:d1e86741366780328d41011f3f6b47b4952a5747ac382a8e9452ef898fa4f83f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44544413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4426e7a133bae48e6fda19ef98d4971571ead2dac074b4f1d4609303101216`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 04 Aug 2021 22:30:52 GMT
ADD file:d941821de800b392c866c83fb24f5743ef60a7ebfc9a85d084423f2bcdf86315 in / 
# Wed, 04 Aug 2021 22:31:06 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 04 Aug 2021 22:31:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5aea9ecf92cd1ea08204252b06906f016d538959a434604392383782a3acff94`  
		Last Modified: Wed, 04 Aug 2021 22:32:46 GMT  
		Size: 44.5 MB (44544220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49daf7270026bde36af0a2c43da0619f9dfcb146daf7c584824b936db54cfcd1`  
		Last Modified: Wed, 04 Aug 2021 22:32:37 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
