## `debian:stable-backports`

```console
$ docker pull debian@sha256:b5b9e3e0a8a40f38fe44d33947475ad6e7969ad83cbe00aaf62f485095238c6c
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
$ docker pull debian@sha256:3b9d7a5e898b0dc129d9e3a41becbb306e47fcefb98f1a2ed4cb9887d958f35b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50134475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1477a0e7e7d58e64624d8706f0f1b42eb6a11db85b962f8c41454abf3321b1d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:09:40 GMT
ADD file:544c822f836f49f5e182ed70d111afa02054c3f56a9f3a24a0256dfb9b28455c in / 
# Thu, 02 Dec 2021 09:09:41 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:09:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f0b1154e6665dd07060d16b5ad6b925d011f05938e36d9956a816a3e5607445c`  
		Last Modified: Thu, 02 Dec 2021 09:26:43 GMT  
		Size: 50.1 MB (50134253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e900ae0d6eaf4287f4122bc7354d2f2be9baa70f71ac689f2f29fc5e17dab3`  
		Last Modified: Thu, 02 Dec 2021 09:26:55 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:d290a74fd92feca29cc69667809cfa5181f944506c7642d359522ec3abc2fd51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53619249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a01c7029ccc819e837a6a62aafaa605c5606e10fc33588a67335632188f3391`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:09:46 GMT
ADD file:fd7fb10ac6848a12754b7621799eea9c23b5ef143de525a6be75d60fa308106e in / 
# Thu, 02 Dec 2021 08:09:47 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:09:53 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:068d4584d7e45560ff7147a5b0c30b1fffd5ad515f2016f48897cb2750e5ffad`  
		Last Modified: Thu, 02 Dec 2021 08:43:49 GMT  
		Size: 53.6 MB (53619027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a177aee66e7fd1bf62ac2b76a95c318182e322670cddf21e803765754bbd4f20`  
		Last Modified: Thu, 02 Dec 2021 08:44:00 GMT  
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
$ docker pull debian@sha256:612a23a8d5168b14c5fa70032097565488aef2dedf12f094bc58d9052d982960
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58819817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540b93cb23ca4080d4610498609e20f2715cc09c816160639f9c2404fbf7c549`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:24:11 GMT
ADD file:c3d40efaf33d2455dd6715c1167d413e62556f2f94475afb72e120d99841bc62 in / 
# Thu, 02 Dec 2021 07:24:16 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:24:31 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:672360b9a6ab75e79b4d477b6e4c3b29bfdf938b152f44e6d1a93e7e18edda54`  
		Last Modified: Thu, 02 Dec 2021 07:34:35 GMT  
		Size: 58.8 MB (58819591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efc5f6b428c035886496c11b594e0172e25a4182c755ad3e10e87220af13fa7`  
		Last Modified: Thu, 02 Dec 2021 07:34:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:11a8bfdb404463cf3efcaae254d9ddc2f7a8535b1bb3422db201aa5c54bb5aba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53207606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0581fba5eee3142367d4dea181f541718e2fcd8f88d0b56e8a23327456962a6e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:20:51 GMT
ADD file:9fc88d98f1ef4c66f74ea61b65412642d2964494d131bcc4ecf98db4addc2641 in / 
# Thu, 02 Dec 2021 07:20:54 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:21:01 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cae83ef09aa79288c95b5d10ddd6a9ec7f5c79593cea2d5f7ce7ff8576a1d14f`  
		Last Modified: Thu, 02 Dec 2021 07:26:50 GMT  
		Size: 53.2 MB (53207384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3f7ea82ec0181d001b7887bfc49767823ed7d9cfe3bd483155dba29950226`  
		Last Modified: Thu, 02 Dec 2021 07:26:56 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
