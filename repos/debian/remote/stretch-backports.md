## `debian:stretch-backports`

```console
$ docker pull debian@sha256:ef989162ab801d1c417549ed9ca33afbb33ec659adfb2d66653e748fb4ecb58d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:521a6ff73ddd21f0f6d3afbd904d7afa47e7908e87e8e35c6bdad89c94bc2b62
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45379875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed3036dfb843e5c57bf8ab90b7e43da534e71a4e1a6e21a9846d0c9e56a3ca00`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:25:19 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf3c3fa9ce17fa21f8a0700e18f7ab0c752cc46c376d78710f739827ca41633`  
		Last Modified: Tue, 28 Sep 2021 01:32:41 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:128875e8a5f363ab74e7b001070cb4c7ba9d19a0f0de9da5cccb092314d72f9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44092158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811cbfc3b2af93a09f956842463bc44e7bdfe1c3908f25ad4f23a3910b779162`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:56:05 GMT
ADD file:f294a28ee9da17e8a289348f6b85aa865b9f1925aebadee96124e1d4a81c8401 in / 
# Tue, 28 Sep 2021 01:56:07 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:56:22 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a237f80116468b0593b0195bd02cdb78fb8bea8e44f206ec86fd61a9377d7a06`  
		Last Modified: Tue, 28 Sep 2021 02:13:48 GMT  
		Size: 44.1 MB (44091934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b632a1cac34257197b75074b7406e129588d0035a5a5dec5e75fdc260d970d5`  
		Last Modified: Tue, 28 Sep 2021 02:14:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:09aaa236c72dab26b357ed6d0e409fec560f300b7480bd7dd83865ca5ddebb06
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42119735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f69b0f6a2bf37c0d385bc03c78a2cd5b5473d510b1ba1283c387c81266d497b1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 18:09:11 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbca02aae33d72371b14f7fa585dfb9039bfada2bf08d5ce89b196520fbc2d11`  
		Last Modified: Thu, 30 Sep 2021 18:26:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:db70edf85cde3126933b6934aafb398c11b44a328de92f0b0f5d22ea13ad456d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43177083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19bc68c7b219f435b2ae7b1d85fc085ef4f4d8a04831120aaa400df6a4348a4a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:43:17 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c088801ee6872726bb97db67bdc26b30db76ae7db68f992fb7827048079e9c`  
		Last Modified: Tue, 28 Sep 2021 01:52:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:abcde3b5b8055a4846dd64b11d077a5156585005dcd210011dffb04b58d8d5d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46097276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891ff7eafeb7cea10e7bced7e0f3c8efee0b2042e81c92d84607c094da44a9c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:20 GMT
ADD file:489732b99c09023c7c1cf27548ad2ed82fd8c8411b95a4e155ebcae7546e563e in / 
# Tue, 28 Sep 2021 01:43:21 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:43:28 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:436d1bdb32419bd787d72deddc5b6a490ad25f93d42a585923767fae7698cb58`  
		Last Modified: Tue, 28 Sep 2021 01:53:31 GMT  
		Size: 46.1 MB (46097052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4760d569689cd99a4d356ac32dab8d97081a5027a5dadc7a878d012f8c4ef81`  
		Last Modified: Tue, 28 Sep 2021 01:53:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
