## `debian:experimental-20210927`

```console
$ docker pull debian@sha256:68c693db0df4ac1f75e594fcd0af796a09f1830afe66c0de8aa329a077c46d6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental-20210927` - linux; amd64

```console
$ docker pull debian@sha256:b279cc9c72c9fa3cf7e544f2ce727bb9bf8ce1038c85bc59f14788529aee7a07
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55702303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31fdaa2dc57071f1e17bda59e7fd5c9bd4575b5f15f22339a6ac7b84f5289f91`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:26:13 GMT
ADD file:d9d629780e76b855e899e172dd9c2c5af25041582089ee1b21e93ff0203a3521 in / 
# Tue, 28 Sep 2021 01:26:14 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:26:32 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f2a8c55f290b62847a927b026f135fd01ab2550c4deb33fa1781c18f90374632`  
		Last Modified: Tue, 28 Sep 2021 01:33:49 GMT  
		Size: 55.7 MB (55702085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6618546fc27afaf845d3034394cc0f15d38e1045cac3ae34bcce417a6ae678`  
		Last Modified: Tue, 28 Sep 2021 01:34:13 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210927` - linux; arm variant v5

```console
$ docker pull debian@sha256:8a4f916d9e36311902a2846279e485d51dd8dda020a8bac2bcb071effbfc527b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53207960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f414c2011f484535429080214eae9b51a49df68d6296fed8e5024b5598e9d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:58:14 GMT
ADD file:b63a63ab01fc172b4c28551c27b70aa05bdd15acd85ba9856649862ea4daae06 in / 
# Tue, 28 Sep 2021 01:58:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:58:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:784c6ec35bdda3101d17229a73642faa75436d502a0c481971177b209007970b`  
		Last Modified: Tue, 28 Sep 2021 02:16:54 GMT  
		Size: 53.2 MB (53207737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4f4d1fb80cd4ed429bd3201c7ddb31fa5a5ea10dfcfd1a4835981f97f7d2d6`  
		Last Modified: Tue, 28 Sep 2021 02:17:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210927` - linux; arm variant v7

```console
$ docker pull debian@sha256:917787bdd085fd63839072e8c4092351111580f39244c02481e324fc2915cfc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50822669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73e69af3de455b9eae67b2a154230f2aea2375706abea9965a97e0bf31784f01`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:11:13 GMT
ADD file:9ffe3bae13530198f02a2ef712137eb102ffc6212264c54fe79e7c06f1181b38 in / 
# Thu, 30 Sep 2021 18:11:14 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 18:11:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:00fdcd55dc79d7fc97bc4d765aca503b1366c51a697f46ebe60e7c125c0cd121`  
		Last Modified: Thu, 30 Sep 2021 18:28:56 GMT  
		Size: 50.8 MB (50822446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9082bef6bd9b460f092f8484b4910f1db8b3eafca4836974b08424596aa41e`  
		Last Modified: Thu, 30 Sep 2021 18:29:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210927` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ffa74a7edf8c16771aa3e1e8af3d5eed4d24c30294faef70447e4b33931dd550
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54725540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b42c7c97535bf9e53241809cc92cc2ee42df0f24ab42d1f7bed7824a66e8740`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:06 GMT
ADD file:c6c834163255512247f4299caa0071f4b3fe9392b02ab3867c05508f08da5a03 in / 
# Tue, 28 Sep 2021 01:44:07 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:44:23 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2d3594ced7745eb15a2b7007358597197a2ed8197194eae33fc3ea0db03f123f`  
		Last Modified: Tue, 28 Sep 2021 01:53:59 GMT  
		Size: 54.7 MB (54725321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666b3a15a5395971b6741d18737f616db4b8eebb644c0e355d1c2d22f4c81821`  
		Last Modified: Tue, 28 Sep 2021 01:54:25 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210927` - linux; 386

```console
$ docker pull debian@sha256:c74b9a5b86929bf602240b6eb825c153181d6439af544dd0785bf56566f88012
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56733439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5410856927dbddda32c12d7806b55a3f365832967069630f6bb160dd032c0c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:32 GMT
ADD file:6b060b0698e864f6ef8a07c3a6a71205dca18a95b9b8c95d64d2a2fdee7d7846 in / 
# Tue, 28 Sep 2021 01:44:33 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:44:52 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9b5dc80bbd482cc8a27c804eb711f6f3216dcd2c0e78e2cdb9b847151d747ea9`  
		Last Modified: Tue, 28 Sep 2021 01:55:19 GMT  
		Size: 56.7 MB (56733217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2cc89fbb9e27513abfcf28343eefd536efaa49cd6b001560ae862aa0b02a23`  
		Last Modified: Tue, 28 Sep 2021 01:55:49 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210927` - linux; mips64le

```console
$ docker pull debian@sha256:de21027ebd272fd0828e54c30e4a673b107f7beb2e3ddd670fd03151f8703406
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54326360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d627a90d79edeef28d33441680c6cb090bc52928c4425cae9e59a28408afaa09`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:16:31 GMT
ADD file:a3359fc361a8952f634e3c84f469a8c69d0816435eb925b63e9faf6d64a1a7e4 in / 
# Tue, 28 Sep 2021 02:16:32 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:06 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:53686cb2581609804e932bf9e4dc26f71ce57d5f52779db0c55a744f5c9e7b44`  
		Last Modified: Tue, 28 Sep 2021 02:27:56 GMT  
		Size: 54.3 MB (54326138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba4b103249d10ab8981d6c1fc6629424cfa92ab9ac445f010fa19f921c7e30b`  
		Last Modified: Tue, 28 Sep 2021 02:28:36 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210927` - linux; riscv64

```console
$ docker pull debian@sha256:57239468a78e8b8f052ca4b0c77bf4b541e793d9c4da74717d87765a16e4ae24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51531366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89427f4bd1cc4ef6234609933bea2c10e15932fa53482781c52910f6bd2b4975`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:17:51 GMT
ADD file:d0c4e0ace19c426515e6adbcf8eaa8133ea5dd24e60616cd60ccfa7f66c35139 in / 
# Tue, 28 Sep 2021 02:17:54 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:21:00 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:941c9215000d0e61468dfcdc88c236b17ace591d854919c008642a650d855d0b`  
		Last Modified: Tue, 28 Sep 2021 02:33:41 GMT  
		Size: 51.5 MB (51531140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9996ca2097185367490a26f1ab401620b5760f10cfaf228911e5acdfc28cdd38`  
		Last Modified: Tue, 28 Sep 2021 02:36:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210927` - linux; s390x

```console
$ docker pull debian@sha256:76a9aec81cbf2ff1cf52171e5a57fd696d2bc9a2601dfbbce0e85cce3d17ba2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (53954079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:173c91a279f8fddd18831e4eda741ba964397b1fb423c6b4738a69715f8b3be1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:45:37 GMT
ADD file:8209381c87e3a9b971b314c7cb23655d9eaddd1cad08b612f6f6d0c97fa2fdc8 in / 
# Tue, 28 Sep 2021 01:45:40 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:45:57 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:95d1bea7bb30019c440a4a51393275efc64a586b9a0f916a69c27a386c444240`  
		Last Modified: Tue, 28 Sep 2021 01:51:40 GMT  
		Size: 54.0 MB (53953860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2ea63ed6a7e4e213858f4021cd6e8ae74db5bd9ad85c27ff53f739d566aa1a`  
		Last Modified: Tue, 28 Sep 2021 01:51:58 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
