## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:6da71dec6ef884569a70040865f8f6592af25b070a478b317bdb483667ecc3a3
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:da108526586b32e512b61973c31d46c255d6d08533ffd3f34c6c92e3e370a65c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54999631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69413af002459083faa34ab6c7a74eed2284c34e8ec50a03f470db41590ee8b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:19:57 GMT
ADD file:3451708ab45bc1bcfc1ebb2075d3af16767477cbeb79334959e0d1ff02b0864b in / 
# Tue, 12 Jul 2022 01:19:58 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:20:01 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d836772a1c1f9c4b1f280fb2a98ace30a4c4c87370f89aa092b35dfd9556278a`  
		Last Modified: Tue, 12 Jul 2022 01:24:06 GMT  
		Size: 55.0 MB (54999406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c8a6f4a0f6e4b29ff568c93a66d333a252c5c88cfaa55438796f5106f95d3c`  
		Last Modified: Tue, 12 Jul 2022 01:24:23 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:2fe3c44af76274e3f43bb00ccab79e1328dc1bf58a6c9a33db3f21b721a18cea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52537120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eec75c48187be807cc5d5e075024d37b6f3a1c7cb30428a37ef77ec6c3b644ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:49:58 GMT
ADD file:a600937adf471d1624223b1e4fc5af3391a3258d28051f9f9990c978177db2ec in / 
# Tue, 12 Jul 2022 00:49:59 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:50:19 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:458c615f383e394cdb1d249caac254a3148895cc59ef0f317e0c342507c0a43e`  
		Last Modified: Tue, 12 Jul 2022 01:02:12 GMT  
		Size: 52.5 MB (52536893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0929cd39ff8cf6b8e0c9a68574aed9563b4915a56e13d809c92e961d456d56ee`  
		Last Modified: Tue, 12 Jul 2022 01:02:34 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:67f5c51aad373583fdd28cfd0aeb11cfde3da1820ceac7d46d0194f6b4a97bac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50195109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88cf229d8fba8a053d45934b1b20504c835b1d4732233bd3594ce5c628b9aeb3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:59:33 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d77ddba5e5f233e30ea44c0f01b926812dad820d4702b5eb023e1933f8428e`  
		Last Modified: Tue, 12 Jul 2022 01:12:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:a5ac5e89f243e9a250f009beeff2ed7026a9aaf14b4cd3f7ae28c3409bf59759
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53683354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b3338ab7b3c643465ce346a9d71c45e12db9c3b8ae044bd441ffefbd46ca4b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:18 GMT
ADD file:2dcc013bca5a420cad3b6a1ac61f52ea58a29ae05fe282078a744979c0e1a89e in / 
# Tue, 12 Jul 2022 00:40:19 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:40:26 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cfc947b533a3ed8b8ce79820c7fe5e7634bf9c08479ed0aee1e74ee7b4f2b068`  
		Last Modified: Tue, 12 Jul 2022 00:45:41 GMT  
		Size: 53.7 MB (53683129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97294e460374d75f06cf34e4fc8e398589db00292d870745571319671b23748e`  
		Last Modified: Tue, 12 Jul 2022 00:46:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:236125fa06dc1a03ce3bc97d868eb88de3470024a0ad29cd9449c39cca44a91e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56001996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58b77494a1e210c5deb7668fc469e2924e0ee1858462a749fd2b9fe7961abf55`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:10 GMT
ADD file:0fe47b589e2fdec2c7f7e92ab50ee94c37df9276c6771e612d29fde3aefb04b6 in / 
# Tue, 12 Jul 2022 00:39:11 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:39:18 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:992c2740c28ef02c375c076416e9a24c9172d5343205500b8388cf087a76bbce`  
		Last Modified: Tue, 12 Jul 2022 00:44:46 GMT  
		Size: 56.0 MB (56001770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24697d160b3eb352f26c9c25b6a6e0b4068d6ae1c6687196d4eddb81d27153a`  
		Last Modified: Tue, 12 Jul 2022 00:45:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:61dfe093ddb75fc76c4f8586e282649cbdd0e34cbce9ad7fda12eeccf8bdee31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53263512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3d5599538b4ff2b29574aac39d039a0d48efdcdff7b176fa20bb0bb01c53f3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:40:19 GMT
ADD file:5a045303c511235feda23815b401564f1db25de2c312598258626e9be22c303a in / 
# Tue, 12 Jul 2022 04:40:23 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:40:37 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cbe8f2bf6b579db32fc573a5f145cbb10fddffc9fced5f528ed1b70b2c18dd94`  
		Last Modified: Tue, 12 Jul 2022 04:51:00 GMT  
		Size: 53.3 MB (53263285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc94d84bb97f5fc18171b4aa50922247c6311250ce53531d1a8513ad6139b006`  
		Last Modified: Tue, 12 Jul 2022 04:51:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:a144a911429c4cc4831215527d4ea72d99bac39e827819b9fe5de1f76e0cf65e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58895848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e97e2bad411f7da2326d7004931439be41a4663a7e96c16ce15bb7823f857d34`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:24:58 GMT
ADD file:98243e1bfc9c04ce4d47bbf13011c502c01aeea3a0417b4e2b8f90b4debfdd32 in / 
# Tue, 12 Jul 2022 01:25:03 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:25:16 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6fb3da208bae11b3dc38c4ab84ad048c030a1da966740d02681a11866ba2230c`  
		Last Modified: Tue, 12 Jul 2022 01:35:06 GMT  
		Size: 58.9 MB (58895620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d935ea3c248e78a97e7be0f49897db18aaeb20447bc81183d20920ba4b3e7ef`  
		Last Modified: Tue, 12 Jul 2022 01:35:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:63912caf6f29a6e0012181a33f83f0b1bc7abb08d04233bd41c6ee4335b62df1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53269176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:855bff6d3cff15da6198ed0cc95023d3deda92a82dfa07d2153a3bf4ce1ecd8a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:43:15 GMT
ADD file:2a729374ad3e12361206aeffbdface900970f010684d6409328d6be136facfa0 in / 
# Tue, 12 Jul 2022 00:43:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:43:32 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c8c4856949e70ae5ad889cfc6a747677ca43e6945c3d56e2d4e3ea5e17da91a2`  
		Last Modified: Tue, 12 Jul 2022 00:53:19 GMT  
		Size: 53.3 MB (53268948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8031283e4d003489903734334375fc74ccfdef4894e7fcb4e62caeeb11ddd47c`  
		Last Modified: Tue, 12 Jul 2022 00:53:33 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
