## `debian:experimental`

```console
$ docker pull debian@sha256:c8ee8bc1c645c6f9292e6cd2bd0e04bfb78969f65a1b980527f5bd2ab21bb017
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:061197a6f120a3598ad460041a8132d019f344434b6a364b07b2cfe3385e233f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55978729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d302a123be4dd38a83a60b0b9d23779926222664daa6ac83951b1c77c21963c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:25:19 GMT
ADD file:1d68ca50a803e1f7741d7b98132d1d2ba447f8e5b079dc89ce68f579b621531d in / 
# Tue, 17 Nov 2020 20:25:19 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 20:25:40 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2422b4e1b9577948c32595bdae1155337aa9e4aee12054b0e34643f0558376d5`  
		Last Modified: Tue, 17 Nov 2020 20:31:31 GMT  
		Size: 56.0 MB (55978505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8bcf2380097e8d3713576ea0f9ee26bd9b9282a7b503f84ca0a25d1c4d4cb`  
		Last Modified: Tue, 17 Nov 2020 20:31:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:dcf638cec74a2e7fac36d8ec8542f535c01ce5a9ff7e7607deb13308f193fe99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53546244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6547c20e8f1ebc02739b1a3bd89612286b0237dc4d840e5594186c746a6d82`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:43 GMT
ADD file:6a308da1fbf2bab39e57bddd15633f325efb9bf4c2ab958b2651ee6781798261 in / 
# Tue, 17 Nov 2020 20:27:47 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 20:28:11 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1144e8b182c11ffe2623bc4def5569c3bcd89ba1acbbec5701456c5080fab0f5`  
		Last Modified: Tue, 17 Nov 2020 20:36:03 GMT  
		Size: 53.5 MB (53546021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471b033a818d4f3931f4c5220e0bfd28359975431b5f0263c4c7ef143bf577dc`  
		Last Modified: Tue, 17 Nov 2020 20:36:28 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:3b0ec63ca61c059bead6fd2de6778e7401d7b709493e74035663625b3106df1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51126185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec174817e4abec2af33fb577cd07fb66835229d317245310a9ac5d87489e54b4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:28:47 GMT
ADD file:00d267d655f7d6cc681d72da96b38773249f74aa63d76184a4ed09b01ea97e28 in / 
# Tue, 17 Nov 2020 20:28:50 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 20:29:20 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:314385e0b77fbb1d0768891cc944cdffaada4149e5ac6971e9a5734dd20bbe65`  
		Last Modified: Tue, 17 Nov 2020 20:36:54 GMT  
		Size: 51.1 MB (51125962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf14cc759bb07761b90e2b674561b56933d595e063c28fe8d2dfa2741568091`  
		Last Modified: Tue, 17 Nov 2020 20:37:22 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ee82c181dd08e4aa7342413b96cd7001f6ecf5b5a1e625d5dc92d1a024fad294
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54720144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25de2df484a2c366375ff1d501eff57dff98329d2380eca977e877eb35e9b33f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:29:31 GMT
ADD file:fab13d6be31945613ea1c92476ee36f1c3f71b85a6b03ba81fd27b3bfe56c2e2 in / 
# Tue, 17 Nov 2020 20:29:34 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 20:30:01 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:48ed6323a2aaafd4871aa5c263b65294d2ae42d0a8db4bfc170732efdae1c7fd`  
		Last Modified: Tue, 17 Nov 2020 20:35:42 GMT  
		Size: 54.7 MB (54719922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281c8e52e3a7ccd14b2216347de608c171285c0571f0197c4a54da199181b9ac`  
		Last Modified: Tue, 17 Nov 2020 20:36:07 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:8ebed62f8683fa2e82d35b8a57523d0c697630cb1c89bf4448e59bf98a7371c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57102440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e0206acb58436e49bb27a06ade2606717b26f3b36a2f00dae3d6ec7d7b8018`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:23 GMT
ADD file:04c732ca3c2b2582a93a6577cd8ab41f69dfcaf974dccbeedea8c97308db2829 in / 
# Tue, 17 Nov 2020 20:24:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 20:24:45 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:46cd7ea3c4f74478a6751164279c3f1accef3a3e9d5706a995bedceed165bf26`  
		Last Modified: Tue, 17 Nov 2020 20:31:23 GMT  
		Size: 57.1 MB (57102220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df2876d558244fe0617357063ecfa95fd1af3b9242137bab945d0ced5ad8e80`  
		Last Modified: Tue, 17 Nov 2020 20:31:42 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:d9c8cecb045465791a3fa2d1a4cb3157cb65939899009a129cd0c63719cf0fe6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54247395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5efb137af2638a0e257cc9931f2c8814bca06ccccd93fdc81f4d4af50ef30571`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:22:37 GMT
ADD file:7badf1450029b15e14a11dcd1901a32e32eda71ff6c561262589f9afd42e8464 in / 
# Tue, 17 Nov 2020 20:22:38 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 20:23:05 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f1e8d5703b6f0ffc7371359728e726c9c14f16611ac1c3f72c27eb517bc832b5`  
		Last Modified: Tue, 17 Nov 2020 20:31:32 GMT  
		Size: 54.2 MB (54247173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b526403c8d5afb1910ade1723d27dbf7245c97de3a650abcb78a48e505caa1b`  
		Last Modified: Tue, 17 Nov 2020 20:32:20 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:a908e52d5355a2a26cb60952baa24b115ec4c1fce0b4405c7cd751b3fcff676d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60189559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6913c9f94ecb7c43ef8285660308b0d32fab85f6ca6d9368bf661322a2a06071`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 23:26:25 GMT
ADD file:dbbe373789a3ba2897f063390858924d6f2ace4771f0b5ec513a2a9e7c8257fa in / 
# Tue, 17 Nov 2020 23:26:32 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 23:27:07 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5c5a40ddf44192866bb0c05807090374b3439dd2b53a5fdf3c7450526cc56881`  
		Last Modified: Tue, 17 Nov 2020 23:40:05 GMT  
		Size: 60.2 MB (60189335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26c74289059a54e79c43d6699da27e83d22dd4eb38c91a5f52d247bd5ad6b45`  
		Last Modified: Tue, 17 Nov 2020 23:40:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:323aa57c5e17ab9c3d6bd4809eb7ea8f40fa1819676c94772f6d41b5c630c84d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54214621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c57729c334afefa74dc4a2c387101acd10822e8fe504f5e023e33b094c1c42`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:19 GMT
ADD file:927d2c6f4025ffd5474a6d11f2acbd48b5368edf47d099756c234b1438dc793a in / 
# Tue, 17 Nov 2020 20:21:30 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 20:21:54 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:761448970d309b2b34f8c16881deb19ef09b1959d88390e202d3ddffd0a4049d`  
		Last Modified: Tue, 17 Nov 2020 20:25:37 GMT  
		Size: 54.2 MB (54214397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af45a53b1e6aecc61358858fe97d8b4f9b0394238a2873053ad8cf1399f4c98c`  
		Last Modified: Tue, 17 Nov 2020 20:25:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
