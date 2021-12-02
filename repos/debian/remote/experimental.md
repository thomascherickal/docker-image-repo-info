## `debian:experimental`

```console
$ docker pull debian@sha256:c4c3eea9122443a95e04582eefd9769841419aa95efe26092ee39fa7daa3a5cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:44f9f038fe3e2e94793096b020e9d53c02420409f4022c683ec09ff9ce0e53c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55747104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04cfd8921f5e7ea5351d50f6f44d58fe5e6c8ea90c677c77269efbd3d746f03a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:51:05 GMT
ADD file:8ea96c53533f2bfc7d6a15c4d156b56c6ad3a2d3993e1a2b50e15b31bfe2be46 in / 
# Thu, 02 Dec 2021 02:51:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:51:17 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1793db1a9beb666044badf0630ef3582bbc734ee46316e7d7789cee2ba37ef67`  
		Last Modified: Thu, 02 Dec 2021 02:58:39 GMT  
		Size: 55.7 MB (55746882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1368fecb24e7c8120fd6ab0a53db8f59e2e277753fea194e6aa734b99af705`  
		Last Modified: Thu, 02 Dec 2021 02:59:03 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:1a82af1a26c8e3142df6648910031aaa68fb2a3a5d0b02327ee7311a4c0d11e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53226509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a96927b6680bc45d1b50897b3cc2f1c147e3c49e708237e683265aa9c93089`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:00:04 GMT
ADD file:bdb1bf58320a788a3b3115425f34ebf3385ed3fd166fd9f62516fd4f80512490 in / 
# Thu, 02 Dec 2021 03:00:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:00:55 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2d1699f433119b57c3eceaf5d93c93e7ca4a79b6d9bd74ae5d8a94e414aa9e12`  
		Last Modified: Thu, 02 Dec 2021 03:17:44 GMT  
		Size: 53.2 MB (53226285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7b6603ce38ad48f444a48ff36047cc522b88cd118358bc2f38fdf976da5f23`  
		Last Modified: Thu, 02 Dec 2021 03:18:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:045e674644b35bc4a2bf075445145fe9a410f7274f66d801bea71fb370dbc5c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50860530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec3c000773d608dd166eee6d899e220139f9c6f4ebd0fbaedf7ed5e65944cbd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:07:01 GMT
ADD file:930f169a86ba880df2aaea12f3e8598f194b73f18795a8cd70efcd27b241bda3 in / 
# Wed, 17 Nov 2021 02:07:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:07:35 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:61a45c58489b0c8e11c36c2b4e975b6bd6dd5cd0b16c91ccb452966e84c75021`  
		Last Modified: Wed, 17 Nov 2021 02:24:50 GMT  
		Size: 50.9 MB (50860307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8647d476eb9176d77a596dd5cef2be97e3386236a4e2f12e22d27fc8742d717a`  
		Last Modified: Wed, 17 Nov 2021 02:25:31 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6460b222d57825e8dbba8071810b435418e8459e2fc5a4a9096ebb47a83c1874
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54767296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6157a41c40dfece8c9e8f4aeccfec249a4c19835344d6ce672af84d61aeae663`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:27 GMT
ADD file:44b7578caffebde5ddfd201775779df99cb1d525113ba58609f8cdf1f47092ce in / 
# Wed, 17 Nov 2021 02:43:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:43:43 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:af0aea1ea198f6a1207b9812f667f234e3ccf829e7b41959a314d3616636bc52`  
		Last Modified: Wed, 17 Nov 2021 02:52:44 GMT  
		Size: 54.8 MB (54767075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419ceac417071c25631219677cdd697c6d7d12c3b7071efe3130a7a7bd6910b8`  
		Last Modified: Wed, 17 Nov 2021 02:53:10 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:4d07f9ec76fdca2d647f9df432aa2fbfb2c3aa033372e48c42c2e6bdda062824
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56808254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4892c67694c71e13d26f7313ae50bf308a98242dc42f60f9ca1e1cce53cb2289`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:43:27 GMT
ADD file:c8d17c45bc65348040374c6e7d5196c1d847ebed15871400c4da3df704515be6 in / 
# Thu, 02 Dec 2021 02:43:27 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:43:43 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a2779241dd313cf1f06fa859a8361159673690c680955e423984567eed669647`  
		Last Modified: Thu, 02 Dec 2021 02:54:28 GMT  
		Size: 56.8 MB (56808033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e263303a85c0d1de1a995bdb27e635bac1218c59d17e945f3fd9b5fe56e9b94`  
		Last Modified: Thu, 02 Dec 2021 02:54:56 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:22f36216c2ce0fc07cd3d0d14c933947d4ab98bb6db4f034739cfbad1bfcd293
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54455677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6f041258d541a5cd019ee60de00dd8dd7d76be95d6cd5dcfe04c327eda8a2cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:14:01 GMT
ADD file:2d61dbbf49a978c5b903ad6810df99f11bcc9585d06f3fc5eeaa97beb27d6742 in / 
# Thu, 02 Dec 2021 03:14:02 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:14:29 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7e0c1253ea9ee2c36fcc159313f9d8af0a88857a9aba47ea44e0fdee2bcc4881`  
		Last Modified: Thu, 02 Dec 2021 03:52:36 GMT  
		Size: 54.5 MB (54455453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0f42e520aefdff8b68f6604c0e9776716ee6d87ede5acb91bbf48ecbba5e07`  
		Last Modified: Thu, 02 Dec 2021 03:53:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:682b290c786b2bea60bb40637a31e82c464b357185c85c39b88365e51f94a2d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60045252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fedf50d85bd176395364a6f442d183c2fbfffbaf05c51965593223f886efa87c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:38:38 GMT
ADD file:f98cd5c0b6d1b0eca9c66a96528f16cee04c4c39c0099aeb696452eba40f7ce5 in / 
# Wed, 17 Nov 2021 03:38:55 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:40:33 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:20a855c65aabb17aca96cb4aba443be5ede8aeccac91e0e21c41cf07a4ae22c2`  
		Last Modified: Wed, 17 Nov 2021 04:17:17 GMT  
		Size: 60.0 MB (60045027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8329727e1f1f8d329e49169175a09e367d1cadc563448ad984132019f26b854c`  
		Last Modified: Wed, 17 Nov 2021 04:19:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:efe1ae8eaee5a194a51bd2ba5fb1ec2322c19836a1bd7ecc2de349b316814882
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51509504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0efc905b0f3905b3e9d6ed142793c4295ac6aef4892a5fa16fe25aa311915976`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:19:59 GMT
ADD file:a323413cfbbb9d9c5d8922ab6a65704b34c4b5057fd08cd09ec03166656c6500 in / 
# Thu, 02 Dec 2021 03:20:02 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:23:10 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:cd756f7feb59c540dfa3f77898eb4c318cd0e47cd0f90c29ac1dba47238a0322`  
		Last Modified: Thu, 02 Dec 2021 03:36:06 GMT  
		Size: 51.5 MB (51509275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f36b1fc37c32aca05d3d10d71276780689dab5ce163e9a99474a2dd1a4f76f`  
		Last Modified: Thu, 02 Dec 2021 03:38:43 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:d73fa202edf98345edf9e6534f97065f21b1cec3046305536c1060c47d487150
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (53965842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc8704ff4f7e75c9e0aa046a651029ee9276445f9942de9fcfc702e9355478b0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:45:12 GMT
ADD file:3e240d4862da4173e8dc2b043c11c59b5b8d8ea71c087729ecc0bcedf15bc5c2 in / 
# Wed, 17 Nov 2021 02:45:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:45:32 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e50a73e9a583b8d41392e2bc8c7f048886a3cea5c4319e2b919dfbc1866d9e9f`  
		Last Modified: Wed, 17 Nov 2021 02:51:10 GMT  
		Size: 54.0 MB (53965621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c88b35c8c27cbb17920e80d41e0eb4913c843ef5a4f7985f320cfe0c2cd0230`  
		Last Modified: Wed, 17 Nov 2021 02:51:28 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
