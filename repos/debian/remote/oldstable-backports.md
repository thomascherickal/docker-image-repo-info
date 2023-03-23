## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:6247d98cb36e30f44494cbb74367443d8304c4017c64dd89179a1b4984a0fee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:5408cbf2685a8bcc47ee70cea0ae7cc1722081ef6204b9f7a529655db274f929
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50448896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d8eaa3dadf5ed79cf62162d26dc10b03d33d1dc0a0d1ee5c5d740571fe1187`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:31:02 GMT
ADD file:6dac3729cf301591c40d31adcb399d65a85a569523017144b98bf79b5dc4696f in / 
# Thu, 23 Mar 2023 01:31:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:31:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:84d5364bebdbc37f3fb353dfcf4323018e20f84c04413aa7d48e8d7a6bd09bc6`  
		Last Modified: Thu, 23 Mar 2023 01:35:19 GMT  
		Size: 50.4 MB (50448672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468d6a17e15b27d0c92f9ddd30ecb8fa4682e764d7e04b7b5db05aa757f7a5ee`  
		Last Modified: Thu, 23 Mar 2023 01:35:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:82bd27211274978389a34df0ca1b59e6a1d17a2c1de0e20c14ccb30552ea7983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3410d8572fe3252660f1e106d0d8dee14d844ae0a79ae3d7b7dea1d4a253b4b9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:23:57 GMT
ADD file:4b6566b582541d63a29b4baaff448f21e267427bc9459c7284e28c5956db5ff1 in / 
# Thu, 23 Mar 2023 01:23:57 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:24:11 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:751e8e387da1081af495846cae3f04e63d0896e9cd4a95b317c9227f368071c4`  
		Last Modified: Thu, 23 Mar 2023 01:33:50 GMT  
		Size: 45.9 MB (45915862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ac23773af5ad7e20adda1a4774302d0df4c3175f7cc7ab17f9daf1faa1f684`  
		Last Modified: Thu, 23 Mar 2023 01:33:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:74a7bfdba6deface0fd6eb129e24ba466f44a16150c82af82befe9c6ec63f9d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49239950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a853a2cf140be3de76719487194d1dfe79994db1b69b7088539c62b9f9a8575`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:29 GMT
ADD file:3ca838a216948e310a97603cb0d9809d74545e5716bb4fc07adbe101331d351a in / 
# Thu, 23 Mar 2023 00:45:30 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:45:31 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bcffd7be664cb5f76625b6b2cfb4a0c025363fb1f228f6c32b05eb1acfe61188`  
		Last Modified: Thu, 23 Mar 2023 00:49:02 GMT  
		Size: 49.2 MB (49239727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a910a056ba2e8163f623e871d4ee317120d610d1350401255a547c54d8ec1466`  
		Last Modified: Thu, 23 Mar 2023 00:49:11 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:7dcdd9a8f4f1a42d478936d99b6b52617eba2c16bdc8ee00c90ec5dd09859783
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef85777f4ff00aed9ed34153960955501ba726af98e4aca36b7e29ce7855d37`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:50 GMT
ADD file:7a37d1452774d17cc1cdc4ef3b04834f1dc2ff2255df329ad99273bcff617b80 in / 
# Thu, 23 Mar 2023 00:39:50 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:39:53 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:35af01d500b72dc26ff46cb1e4d6300700fe5cad14db1a17127ff2faa2a3cdbe`  
		Last Modified: Thu, 23 Mar 2023 00:44:17 GMT  
		Size: 51.2 MB (51207092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302873df793766dc819b6a4e8512a7b38ff7a02e7789ab88e3577bd37e04d1d5`  
		Last Modified: Thu, 23 Mar 2023 00:44:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
