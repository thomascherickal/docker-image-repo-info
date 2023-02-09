## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:4bccd75cbccebeed0f8ef1e6e79dedc1ae848b03c4dcf216c191358afd3dfbfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:3c397b03fc19ddaf72792b44c23fe7cae2190ad1a1d12c90609c9e667aed213d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50449847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c33d1f15cb9d94319c5dfb5e82eebd56d5767670556687fdbd04d6af600c6021`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:21:01 GMT
ADD file:b07b483f9100ee4d1707a013be28ddc215278371c1f2fc5c48173d4019f8085f in / 
# Thu, 09 Feb 2023 03:21:02 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:21:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:842765569df3e6156da53d2764ab60aaf56f23a0e5b3e3d9cfd2add74e4769b2`  
		Last Modified: Thu, 09 Feb 2023 03:26:13 GMT  
		Size: 50.4 MB (50449623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b41015146f5ceaabedab28eef0754098f61365fdcfe5035d74d83049343865`  
		Last Modified: Thu, 09 Feb 2023 03:26:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b0005fa57a61e834ccefe3beb64aac86daf00cea70d12cf1c8102bfa703f2085
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b481121ddc17720fae5c4d4a84a1f145a34dd5fa2132c6a73ca0e2fcf66c4d98`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 10:00:21 GMT
ADD file:e57b072389ec9e66f0357e15adc45e73ca2fc0ea2691c9ca290fc24f4c0ab669 in / 
# Sat, 04 Feb 2023 10:00:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:00:27 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d86d3cf2d692b7c4950efe13261c152649078f1e681ed507837ecb23d90b25d1`  
		Last Modified: Sat, 04 Feb 2023 10:07:41 GMT  
		Size: 45.9 MB (45915787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbba320524f30be451c699070981adc922f09c574363b4b90ff67f9107bb7685`  
		Last Modified: Sat, 04 Feb 2023 10:07:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:8587e46060033387a47a8d56681aef3cb0d94ea15c1d50e43dc70be776c3df85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49239338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f1ae28606df5d478523b899a014ba272f48f13079385a5d2c4ce69df2598f0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:59:08 GMT
ADD file:878f5e27c23b154025d9a7dbf3a170e273d5ba5cd9a7b8dd260a7eb55c8fd7a9 in / 
# Thu, 09 Feb 2023 03:59:08 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:59:11 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cf72ea4feb35fb006baa39d1a196d82de4ca2171787f76ae6d69351a4e05cb12`  
		Last Modified: Thu, 09 Feb 2023 04:03:33 GMT  
		Size: 49.2 MB (49239114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71ca1901546005b4eaf64c623cd1ec67cba3ed39a3a1a0d926130a9300fdef8`  
		Last Modified: Thu, 09 Feb 2023 04:03:41 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:b5435309d94a8339f723e9d92e5e674c77f452693ecca59d045ab8322cd0fe80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e2d1269e138760a42dfe96d6b568b021912b3979548789eae3f04d5b9b086fa`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:59 GMT
ADD file:09cee105151d95c2e15eacee8803ba5a44a2bf8b6e29a2390f424fe677ee9122 in / 
# Sat, 04 Feb 2023 07:50:00 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:50:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fe16db46e3396ef38850aa05ff1811778e5f85ddd3fed7559ccc867e54a3a3f6`  
		Last Modified: Sat, 04 Feb 2023 07:56:14 GMT  
		Size: 51.2 MB (51207654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c7104789d6edadaa4051ebd514f0804d3b8367544ed6df99150e9cea609ccb`  
		Last Modified: Sat, 04 Feb 2023 07:56:24 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
