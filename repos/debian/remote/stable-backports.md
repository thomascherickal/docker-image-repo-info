## `debian:stable-backports`

```console
$ docker pull debian@sha256:a276134fc0d3a76bb6c3daf6efe3b21baf30c3defe3b1748a680edc287eb105d
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
$ docker pull debian@sha256:19f2f2cba4862eb12c1fec937fb07832850b7b9a0f54df567592a1067f8a2357
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55046577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f42075c7867812c41ccee6f5aec514ba9952e462403190d496802a208b40d98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:59 GMT
ADD file:eb0fae6cc9ae20c0b4bc19663618c9ccfae7108a10ba50b6871d0813aba15a26 in / 
# Tue, 25 Oct 2022 01:44:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:45:02 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a8a0e642eaa9e08096819dffa91eb5676ca8f05d60577ab1887b2368c630c6ae`  
		Last Modified: Tue, 25 Oct 2022 01:50:13 GMT  
		Size: 55.0 MB (55046355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0161a9c82cc1f8c3f9537d2c1d6dcd108f33d1edb2e8c2cc50c5a4124eaa8943`  
		Last Modified: Tue, 25 Oct 2022 01:50:23 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:99ca02e7492ebe446d3f51cf90c771fe6ef8da686c1ece741026bc43a476020f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52547737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef34b899b8b4ea8006583b7107b2c3c85a5b6b5c7af1f5ed95d4a1b1e5c54f0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:14 GMT
ADD file:b4b336b219230fc4fa51e6866dad4207f35b8a48b135964bfaaa1fc030036470 in / 
# Tue, 25 Oct 2022 03:07:15 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:07:23 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b16eda5ab81e20867ad6ae9d4d0f15af5c4d84bbb03591bb014827298594981a`  
		Last Modified: Tue, 25 Oct 2022 03:12:58 GMT  
		Size: 52.5 MB (52547512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57a45674c5d5334b6b5cee375edb0ca90fd0aa96a314ef880317b3a10dde85c`  
		Last Modified: Tue, 25 Oct 2022 03:13:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:af5047d96905d354f1dee8edfe12ec0e42402902c45b2582399d4c04ebf2baae
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50210192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca4b843ff47b2eab805a49bcdbd0daba89c8ea1dd1a83938decb4d17a323c3ad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:16:00 GMT
ADD file:5fb92b027e053fa16dbca39628c6b2ec013b2dfd110cdb7a19326fa3f8a46be6 in / 
# Tue, 25 Oct 2022 03:16:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:16:08 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:acd1a98a2c73dc28425e3c4f7a91e304e091e2cefdbbf761f79f77dad187d05f`  
		Last Modified: Tue, 25 Oct 2022 03:24:01 GMT  
		Size: 50.2 MB (50209970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbebecbf26eb9fa64e5c696fec375cc8f9a954a57884a24709b902507ad8569`  
		Last Modified: Tue, 25 Oct 2022 03:24:13 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ef86292ada56103664a96d9591c3e98885913af72a2c9d9541e203f508890ac6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53700862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26390ffaf62fdc04a7bc552e952778d6b889a812bc38ae467c092888ffd6a777`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:46:08 GMT
ADD file:7432f9080ffb61ff1296169ced0f40910583cddc75781f01f3881da808070c32 in / 
# Tue, 04 Oct 2022 23:46:09 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:46:15 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:993be7e6361f35123f2a260d8c5268cbc9e9b61ca852da08a93a1c14051208d4`  
		Last Modified: Tue, 04 Oct 2022 23:52:50 GMT  
		Size: 53.7 MB (53700637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b34bb1cd7e6ce8b32b3324b404a5e485f4e74838a4fb1366cab02c6269cdb9`  
		Last Modified: Tue, 04 Oct 2022 23:53:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:4c560c3f814e998d6892db462a1285ea2a82256aa5e0f892abe127feae6df1b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56024129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0872c7e19ee13c7d19a489f8375cd5c6395707d36a826365f06958edc23917d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:59 GMT
ADD file:d1e61ec6bcc13c0f2be29c9a7c416f33a3ead644d86bd578d694a6d840d677d0 in / 
# Tue, 25 Oct 2022 02:23:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:24:05 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b21ff3d84fd66b712e899a213d8f49c895874393ea653c7abff016c0960f79a3`  
		Last Modified: Tue, 25 Oct 2022 02:30:55 GMT  
		Size: 56.0 MB (56023905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d50f6441168801da16afe8aa36ff1c1c3e5d15d79549782e4fcbe5795484f3`  
		Last Modified: Tue, 25 Oct 2022 02:31:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:db6391d8a69c6c7b2a3f5bd036d9e4a395607e53178f5c2b9043c946d5bf9efa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53266051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:039e88e7d35a1cb7cd414d1813d5197296f1ab120e68be02fe2ee4ef7bee494e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:12:03 GMT
ADD file:a5fe154c8830989b9086566c70d43c8392077f2aad8fcd9ba028026c98283805 in / 
# Wed, 05 Oct 2022 00:12:08 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:12:21 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0001d895ca18d1d863f7db1cee733d5592b2a5a08d4a6fe8fcc44c35884e82bf`  
		Last Modified: Wed, 05 Oct 2022 00:20:32 GMT  
		Size: 53.3 MB (53265827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef6ab0e583defa86e603ee0a7348220c69c30191fe64814d9e44c92d2a057d9`  
		Last Modified: Wed, 05 Oct 2022 00:20:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:625cb627c9ba695d42832868127ecf24957f30b77b20f5d8325e5557de5b26ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58916587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9256d50765debf26e3a744d665d63f0c51466294f39f64bfee5da1f111d57492`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:40 GMT
ADD file:1335c37daace74176f6bd2cd32410c9aadd667918de3bb505493a193bfa65b5e in / 
# Tue, 25 Oct 2022 03:14:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:14:48 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:17607ab435960d8f13ec9725dd133641f8dd970509586337246d1238893448d6`  
		Last Modified: Tue, 25 Oct 2022 03:20:48 GMT  
		Size: 58.9 MB (58916363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31618c3968576d147ddc708d8439072d3ca80a5c950cab42f7d4265ce3f88b88`  
		Last Modified: Tue, 25 Oct 2022 03:21:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:60817a639240d8cfbb880610a702d6f4fb90d8330dea28ff53355673f33b4c48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fa9a5f8b00bb55524ad83626d6defea163a7c6ffb9448d2f2a5ed46b0d2555`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:15:18 GMT
ADD file:1b01648d65d9b1c7ed1894e357e1b51d87a2c86c8e5a5a7051f8773a95b7d9f8 in / 
# Tue, 25 Oct 2022 01:15:21 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:15:28 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:facde612a2c394cbe497ea9610c4e1f37a765e53d3bf62a88620338fa8890860`  
		Last Modified: Tue, 25 Oct 2022 01:19:43 GMT  
		Size: 53.3 MB (53279173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54b062704f5375d79ade07d3309be1ed57ac2c1f4c2183298f8ee6baad932eb`  
		Last Modified: Tue, 25 Oct 2022 01:19:50 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
