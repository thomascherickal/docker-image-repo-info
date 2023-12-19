## `debian:testing-backports`

```console
$ docker pull debian@sha256:62fa877e515c5e29f8b99f2c37f05a90c5c3d8296864ec87d1ba45b11f59b6cd
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
$ docker pull debian@sha256:b9fa4f82b5d77b154491a9aadd3ac1f6aef84e20b97af5e81f8674bb6cfdf1cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49583633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a14f3aa532d36591188cd3b8f3a8b819faf4fe2a89629f1144790e66c39ada8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:47 GMT
ADD file:bf1a099790136a24feb4eac287781f4d35a1188036c126be1ae0a93f2e5d2adf in / 
# Tue, 19 Dec 2023 01:22:48 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:22:52 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2be50d1418f669b761525b481330d50356bbd66349941bd0ed8e3c04c64c8ada`  
		Last Modified: Tue, 19 Dec 2023 01:28:59 GMT  
		Size: 49.6 MB (49583409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bcee675dae3f6c5395e325c49b689b7c49bfe289c5ba9cb2163a5c6a00bb8`  
		Last Modified: Tue, 19 Dec 2023 01:29:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:2e21519dfa166a9258f38257c441b2d2b3cc403cbcaddd6dba66970f7d74a743
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47284955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f23eccc468089bbd49134231ad2cc7713a3e3103a3a7fd9d50c9188cb6939c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:56:31 GMT
ADD file:d8b6beb37e6678413282dd91b769543d39d217ccd9690612f5f791520851772d in / 
# Tue, 19 Dec 2023 01:56:32 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:56:35 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6c793804354876ca2c75c7e97da2eff0f5d0e9a706cd7388ea3efc1fa9f48886`  
		Last Modified: Tue, 19 Dec 2023 02:01:34 GMT  
		Size: 47.3 MB (47284732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee2e520b3fcf1e0021512bae514b023495292ac0690973456733ffb808fabe5`  
		Last Modified: Tue, 19 Dec 2023 02:01:42 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:9c1529065be2b3c022fd43b6fe4ffd0f57e5ab5aa3523ed5337ded656ad7052e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45080811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6859ae099a198a7da689972fc77eec9d5f8c9fdbaba3839ff53deb91c9a6509b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:09:45 GMT
ADD file:665d63b4590f576f7f2c941c6b0068630d22deaaaefabe08822d866a7b023cad in / 
# Tue, 19 Dec 2023 02:09:46 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:09:49 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ae3efe9bb7367b9c9932f59d6e25fa0e41758b433d837af8e58701e9ca1a8192`  
		Last Modified: Tue, 19 Dec 2023 02:15:34 GMT  
		Size: 45.1 MB (45080587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030ab12d73007dfb894e98d4b61822b89e514e0fec7e1064877f341261cb006e`  
		Last Modified: Tue, 19 Dec 2023 02:15:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:443482a3b21df698ef825c36d3e28bc2dbe0d6e82126b587ecce01c3be875422
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49615345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3abbc367650eecdaecbb73ceb0757afe92247cedbd317514a74dd16da00da15e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:40 GMT
ADD file:dbbb993dac6c8edbddf62b02c1d0707eef4b03bd3eff63b52695164d74107a5f in / 
# Tue, 19 Dec 2023 01:42:41 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:42:43 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:213618833fd5881108293b9462f290a43dd94e2e52deef4db473db151b0cc080`  
		Last Modified: Tue, 19 Dec 2023 01:48:21 GMT  
		Size: 49.6 MB (49615121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe7a735eef1c6e2d3be0dcd44c4fcd5014c710c3f6c49c727dcc0d2cfcaa532`  
		Last Modified: Tue, 19 Dec 2023 01:48:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:28b00ae96d5cf0498ca48a3a741b843da5f1874fe8fbe197bf203f29fa05d8f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50558721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37c17fcbe041e610a0a1a7116723e1efef5c7b67764e2c9860ef6a9ddbf020ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:29 GMT
ADD file:175be0521791398a6f5ad381847860bb6cd956562c8ef8b9559d65c1067038b3 in / 
# Tue, 19 Dec 2023 01:41:30 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:41:32 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:581879089909952f3988928f11d01973e09cdfaa743a76ee73766a1fed3f9769`  
		Last Modified: Tue, 19 Dec 2023 01:48:13 GMT  
		Size: 50.6 MB (50558498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44016014d0cd5a172a45ba46ab6b6fb0da30734ab68d1678d4e3764f04c266b`  
		Last Modified: Tue, 19 Dec 2023 01:48:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:04fd92e120c644527c941a7dd1e3a1637afc127b486ff14b49f054a91e956ecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49068626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f5354c13c737f324e8a737c838948ed4437527116b7c2efc40deafb585d77c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:19:04 GMT
ADD file:3bd31d88d1869efd5f5d14bf6b88c2efb46cc725424199d8840b26c4d619527e in / 
# Tue, 19 Dec 2023 02:19:08 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:19:22 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8c37c1aefcae50b3a2a9b0a693811618cf6b89a4a5ca356542f23587b48a01a3`  
		Last Modified: Tue, 19 Dec 2023 02:30:27 GMT  
		Size: 49.1 MB (49068401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cffcbda459cfd6c0349798f6820a243f5be4d865f992924efcc14672c2ba8a7`  
		Last Modified: Tue, 19 Dec 2023 02:30:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:c97262c2507625ec35d94dc51fdcd97c6aeeb11f9485130306219910560c6a37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53476669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2dcc80204cf5515cb0ba2a795d791f5dccb653c4227dc340a5b458bd0978d2b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:23:50 GMT
ADD file:ee3cb605ce884e3fd7b604dfca909636e0b59216fe3336f2825e7337ba916a2e in / 
# Tue, 19 Dec 2023 01:23:53 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:23:56 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bc865b325cbd5fad6fb967a293ffe0e52c3003a42cf80fdc316014fe20a7d923`  
		Last Modified: Tue, 19 Dec 2023 01:29:30 GMT  
		Size: 53.5 MB (53476443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733f9beb7072778ed815bdc4ffa9d9c7b2e0b43774e85e9a50b98167dafb18fd`  
		Last Modified: Tue, 19 Dec 2023 01:29:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:edfc43edd9a5dee56989b55ccd9bbc76b46980682e228c2d3a1070ff80577b05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49047971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9f2d0aed0d2c9d4f57e390a0e37e63c422150daa395bcb5d379b8f2ec6e235d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:44:58 GMT
ADD file:632dc1ca5542f093ca4f7354e6eada70468846f8756116f18fdbaec1eaa91442 in / 
# Tue, 19 Dec 2023 01:45:02 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:45:09 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0897e866e45024ee14fbf1277f64a545d81ee7a189397842b04a9438eae6c8f6`  
		Last Modified: Tue, 19 Dec 2023 01:49:30 GMT  
		Size: 49.0 MB (49047746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d2bf95665af9d723a0920fc529d55cc0e14a4ee5e6d4338d006dd0fc00ec40`  
		Last Modified: Tue, 19 Dec 2023 01:49:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
