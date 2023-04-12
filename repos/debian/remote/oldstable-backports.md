## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:9a7adb48d433b0c42a7dbdd3f4324a95e657b32ad6711f0fa1d7037957db3ee4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:1e2621c4072e1f65d573302510841fd82c72b0101deefe817d7abc7943d0cd97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50448966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ec95d88d7f4f502f82e0a5befebd371a8f903fa31ff88604e655021f6631c44`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:35 GMT
ADD file:f847eebe128616577b0c1446a604d83f2e5b0aa0ea6558ac3fd3197acd565450 in / 
# Wed, 12 Apr 2023 00:20:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:20:38 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:86ea788dd30a5e7aa659d05425a26e2e6cc3e28456a86f9a72804a0b20c73a2d`  
		Last Modified: Wed, 12 Apr 2023 00:24:40 GMT  
		Size: 50.4 MB (50448742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0082b1a88baa4e5489c0f74586f8799157030581fa2a7ad95d350a3a1adde3`  
		Last Modified: Wed, 12 Apr 2023 00:24:48 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:c37ff97d69d0bd9f70b6988dd2e609feb7eff9aab1f9c1faae972a85ded33e42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cf597edfef6cfe7defcd8492e650bad5965b0ee8fd0be47284cd3dc3dc3d254`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:10 GMT
ADD file:cf4b865a9975f91a514a6ac1ea3d16ca0b2168ee0bd34ff1f5ff8608b55ffc7b in / 
# Wed, 12 Apr 2023 00:00:11 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:00:13 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d7eb6448f66ece8b2e1bdc559da9b93296d41b223b4eb9431ac5d847ea4e5da5`  
		Last Modified: Wed, 12 Apr 2023 00:04:16 GMT  
		Size: 45.9 MB (45916224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164123b44dafa936ada710e3d59b92e0f3b4e343d4dc1f311f3f5b40afbfceb`  
		Last Modified: Wed, 12 Apr 2023 00:04:24 GMT  
		Size: 224.0 B  
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
