## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:ab4b0e3024295f546c5aa2bfa612c1979851dbc1afcc1de8513b770cc6255ace
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:b1f28eaf2b0f6e1c4fcb2de8d2e55f1500310cd6f8c702a34add85c9ab3031d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55578956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69efe536855be0685b2bb92a85e7729b27558103d276a9517abee930f368caef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:42:54 GMT
ADD file:b5180fc4d45b984afa69f3cdfa95980bcdfd76d75f704f74f1aa60e416272f1a in / 
# Wed, 20 Apr 2022 04:42:54 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:42:58 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8cb01d170a54a4c7fd7c1969e79df0a453468ebabfe1d860b863f7a3b6fbbc2f`  
		Last Modified: Wed, 20 Apr 2022 04:47:18 GMT  
		Size: 55.6 MB (55578729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02313a896ab9477f41a3f1fdb81b645fc2ff3eeebe183d0249e0f7a7ff945c17`  
		Last Modified: Wed, 20 Apr 2022 04:47:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:f9aa794f100bb865ba0671b9e7fa5472c5b98cf48542a2cea87a70e3711088e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53001322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9b70998c55de1abfc130a0e3a9c2f2912467dec649f4cb8fed40f243f41058`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:15:05 GMT
ADD file:e283a0d8ab69b94018679c485439a2b5700bcbd73218180b0a334a00df340093 in / 
# Wed, 20 Apr 2022 07:15:06 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:15:18 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e7b4944a983e7a423568be713ae200d96e80ca1893c45b7758ec97be00ab710b`  
		Last Modified: Wed, 20 Apr 2022 07:30:20 GMT  
		Size: 53.0 MB (53001097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425c158578cc53fa219a5b15e47609f914eb51269df1330bd97ad98a76b6dfc3`  
		Last Modified: Wed, 20 Apr 2022 07:30:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:6a5ee7b5b875a2767b92a0abb98f0cc28d5916b46e9bfdc22cebae0b284649c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50610028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac9386130d42b43f0a6aa0ba7b15d2bcefbd0fe80b757b6ffc3311fc5a7da7f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:16:59 GMT
ADD file:5ab9a8a4847f677425562eebef8854e58592bb57501d4bc6f521315d90815c3c in / 
# Tue, 29 Mar 2022 02:17:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:17:13 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c7c8b286eb908a262d0005e4560150fabc15db4a3531f7e00f77b76643457e6c`  
		Last Modified: Tue, 29 Mar 2022 02:32:14 GMT  
		Size: 50.6 MB (50609802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f44aedd4e60510861dcb7935a8a1c48882ad350349c54e886ef5f07f034098d`  
		Last Modified: Tue, 29 Mar 2022 02:32:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:a7ce268a65810bc0a624aa6f8c2252b1898767a3b9951cad9258803b3a366919
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54493515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bac6fdfbac43d0d5177740962c16caac4303ff648ed775e86bd445f839dba1ff`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:28:29 GMT
ADD file:23397ad30e34521aa2c0881ab09c9c75f58316594a1c14f01cfcb212161c32fc in / 
# Wed, 20 Apr 2022 04:28:30 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:28:36 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c6d996fb7c2fde9d95056213e2cc0a2ea025cc86ce1ceeac46b8c51b2d458d84`  
		Last Modified: Wed, 20 Apr 2022 04:34:39 GMT  
		Size: 54.5 MB (54493289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf32b5d72b6a2412051bc228e2f98ceb6276b3c68dcfaf7b951d518ae387c31`  
		Last Modified: Wed, 20 Apr 2022 04:34:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:0ca5c9c0fefccf8f4879086d2d8fedb0a7561a5b6da6a9da69f6ff261bb3050f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56624764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90185cee737e64c059da56cd54770d2893dbe87ab190ad0bad25088bb47a0729`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:36:51 GMT
ADD file:469d404c80a1f5720a0a00e4cd116adfd490349ede3a368fae44c6409add4819 in / 
# Wed, 20 Apr 2022 07:36:52 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:36:58 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c3d3d77c2c71a18bcd4eead6143eb6d36f5096a31d00bfdb4cbd88058ba444c8`  
		Last Modified: Wed, 20 Apr 2022 07:43:35 GMT  
		Size: 56.6 MB (56624540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e438fe680fd64a42ebf4a25e6e6e716baa6faaa6e3296b8cf3fbe8567a303450`  
		Last Modified: Wed, 20 Apr 2022 07:43:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:718685db3cd4f848161727a37e8452a499e8ebb8fdbc4bd98662e8a9085c0f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54240562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:595d136793bb4f998f309a5990bb19fbbd7014f1738ce8775e136c6a0c99c17b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:40:39 GMT
ADD file:88e75745fdbfd0784c1c18134a0a52a5534df18201a6f49555a5c618b4531804 in / 
# Tue, 29 Mar 2022 07:40:44 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:40:55 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bdc3f4c024aea887030bcf477ee808da6aa3e6683fb111845d94ab4f2480ff24`  
		Last Modified: Tue, 29 Mar 2022 07:50:58 GMT  
		Size: 54.2 MB (54240334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c073b220886baed5bbefb457357d80edad91c1cb4c1f6285abd66f85bcfa6d`  
		Last Modified: Tue, 29 Mar 2022 07:51:08 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:2cd7223e27cf66a3c8792c95aae14e23bd260e64c1efcd14579e9b7aafafe48d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (59982881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940d95447bba21279b3c6f0f5d6cec558c36821bbb754071e5c3a0cda6a65c25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:44:36 GMT
ADD file:b40661820352e5ff94b93927c06b3375d894c06269350d442169c7a7b3952388 in / 
# Wed, 20 Apr 2022 09:44:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:45:08 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9f7d9b4a813a5ec1ec0b3475149a2c942961debb65bc15ebf43901246ca6a9a3`  
		Last Modified: Wed, 20 Apr 2022 09:55:28 GMT  
		Size: 60.0 MB (59982654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f5e48829c886141228a6d3cd15ccd8091ce900fb2ba7f1018c907181b192ae`  
		Last Modified: Wed, 20 Apr 2022 09:55:41 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:152f1c32652e2647df5621f0e756f2ff8f756af222ac1169d99d0c42cf883843
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53813658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f8e6acd8eee5a1459a198c28b9a985434eaaf11159c198963ddf489606db08`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:37:57 GMT
ADD file:dd66488219818707ab57e2b9e87dcec876513326c64a733dcf95396ad5f22cd9 in / 
# Wed, 20 Apr 2022 08:38:03 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 08:38:12 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2b24c47356e8597f2e75ec110237cb3350c6d41c44b019ed531f1d9069ab1a82`  
		Last Modified: Wed, 20 Apr 2022 08:48:48 GMT  
		Size: 53.8 MB (53813432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a403ace6777bce26af1254889ec8d1e1ea0df2437dc2ce68f3d784caaa4c9c`  
		Last Modified: Wed, 20 Apr 2022 08:48:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
