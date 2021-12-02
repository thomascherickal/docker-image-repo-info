## `debian:stable-backports`

```console
$ docker pull debian@sha256:94365ec984eff34377ba475f3af167f5dc0cfb8673939ef48cc2bd1afa427ba7
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:b6b307db31e55c92d413f7a5b45126ccdddd0eb22ab82a299aa81c0d8ebb83a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54933099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4db5bb851a23554682ad9d7dc6236691d05b6acb9839c1abc8379339153095`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:49:57 GMT
ADD file:797b322930a0ad7851a2a92a503cf7b050f1db0197a69d9ca321877f9cec7786 in / 
# Thu, 02 Dec 2021 02:49:57 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:50:01 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c061c8f46aa17f16da148b92c7203c48331fe04148493039228900abde7d81d3`  
		Last Modified: Thu, 02 Dec 2021 02:56:36 GMT  
		Size: 54.9 MB (54932875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff305f4683bdd71cf16c4e631df2b6cb4e85c66feaca34122ec9b47c1236aabc`  
		Last Modified: Thu, 02 Dec 2021 02:56:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:7d6be8625e6304516c009d53de63efddc48ae4bbed8091e7ab7762009255e2bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52468153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89be2a8c575185a12780503565c2f11af3758749d2bdcb58ae3c3c1c0a782499`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:55:55 GMT
ADD file:94cdca07d28891adb1c12d7e775d2ea566857d4249cac7e7725fefbccf2a3dd6 in / 
# Thu, 02 Dec 2021 02:55:57 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:56:14 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b9536ae862a698378e6bb295b7af4566365a2d1d38a1e99d7248d87270015850`  
		Last Modified: Thu, 02 Dec 2021 03:14:21 GMT  
		Size: 52.5 MB (52467928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859afa44ee589e1cba970339373f548d9cc990a5e45f90b9f73d635975d5a120`  
		Last Modified: Thu, 02 Dec 2021 03:14:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:a0a962ea97c7eb3e7f392816727f7ce54b15e0314cb8464dd0bad786aae7dd64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50134369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a26fc5ba15848f589fec1b4d50fdc2aebc3170114d9a80eba6699a072e4e1f54`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:59 GMT
ADD file:ca44c08236db78d5b80510c54cdee9150d6a9d941329c2beae1caac598751e6a in / 
# Wed, 17 Nov 2021 02:04:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:04:13 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:189f1a1f83bebf899831dd3d429cbad6c3a317cf7441cd397d2170d70a38bb63`  
		Last Modified: Wed, 17 Nov 2021 02:20:52 GMT  
		Size: 50.1 MB (50134145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b577c408d3e309c68e7e84153c035102adc60605230ac923be81173287988e`  
		Last Modified: Wed, 17 Nov 2021 02:21:03 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b7d77d784950050b9142e76ff2a4332f3d703ebe7d870ea351a4424430146df5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53619268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1080748dd6feefa12216691874d26c7285642aa8a08df2e753f2e9d88a6d9d4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:1a630039cb75bd98ec72465cbb0b0d8d5c5dc123f40d39f719d2bdd7d3e13210 in / 
# Wed, 17 Nov 2021 02:42:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:42:15 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f9d8cc8f1c6c951399aaf87bff2af9b7abf020cb01d5d29652d4654f5bf5e5bf`  
		Last Modified: Wed, 17 Nov 2021 02:50:27 GMT  
		Size: 53.6 MB (53619046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27fbc4590ebb15316daaed18526114b8809eab2fa6dd2c42e1ce5811ad0500d3`  
		Last Modified: Wed, 17 Nov 2021 02:50:38 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:3c00db58ae9d53b3dab3a312b1b73b8f5e4b6af839e40e53ee6fa225957f384a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55937792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a9253ee611e54ed8ec93fc4a5eba883bdd2f6a34fcdefaf909d56956c08bd58`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:41:59 GMT
ADD file:142ba9f894d6e040ff57296f714fbd722daf479319e0a6b01478cb81a932f389 in / 
# Thu, 02 Dec 2021 02:42:00 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:42:05 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:70f9f59ade5dca41286db5019ded5ab4cafc9b895c2b9e4cf3e5e13eef52fa77`  
		Last Modified: Thu, 02 Dec 2021 02:51:49 GMT  
		Size: 55.9 MB (55937567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b7409c282eb1168c50cfbc13e3ee1a0be32b8603dbe7d128fa55d93757abc0`  
		Last Modified: Thu, 02 Dec 2021 02:52:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:651fa3ef9190164cd4beb2dba71a4ee72e0b20f514e5249b3667a7a64982a16e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53184080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:575a117ee345e272252a856b5e78cd770e37911edef9d5d268bc6aa365b79522`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:12:13 GMT
ADD file:edc7c8309e49aea9304c225740ae1ef4a331832bfaee41c524df95ab29f48795 in / 
# Thu, 02 Dec 2021 03:12:14 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:12:21 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a25baf1522352f088acb1da1b108d77b0bcb49d0271d4182caae670825e713b7`  
		Last Modified: Thu, 02 Dec 2021 03:49:56 GMT  
		Size: 53.2 MB (53183854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f3bd27519e72e81d694f57537f30df2a572a6a732ab53c55893891b50c6fc1`  
		Last Modified: Thu, 02 Dec 2021 03:50:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:093b7a7fc569488b0788cfb6e340bd6984f46a44385ce0f2f43022df9966cce3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58819723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c184c267bc27dee45fe273f1262a62a7f23b160dcf0bb09b1f54777696a772a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:34:18 GMT
ADD file:bdd203d3aa82e66b1a4391f79c6433884ab123bd50edac2f11a721860eb13935 in / 
# Wed, 17 Nov 2021 03:34:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:34:55 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:984a1e73e76ac4abb413782fe27b8ab9f8d6a7b98b4ae3940a9c620b678703e7`  
		Last Modified: Wed, 17 Nov 2021 04:08:19 GMT  
		Size: 58.8 MB (58819498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f5cb40f8bb5f9ae96513693e2f5ff1c7831cdb26be3dff78f1078c5488d5f0`  
		Last Modified: Wed, 17 Nov 2021 04:08:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:4c4742de8edf8878fd23c7cd11e2a71a07ee3230b604143237af932d6ec1ac09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53207379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3e76f0a1673c1760155300519c0fa60733713fab06ff835210b7f2e77823082`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:44:11 GMT
ADD file:f1ea9110d656eb3478ede77049c3fea3eadf89037d13f2b6799ce8c86708778b in / 
# Wed, 17 Nov 2021 02:44:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:44:20 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7a62fd5c373212657c719868b2144dd6f23387e47af5bda68af8785210025ec9`  
		Last Modified: Wed, 17 Nov 2021 02:50:12 GMT  
		Size: 53.2 MB (53207157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1393d13e4a191ed8615f817e0422c47b3976ea05c8ea4c2688b4492d0e5bd2`  
		Last Modified: Wed, 17 Nov 2021 02:50:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
