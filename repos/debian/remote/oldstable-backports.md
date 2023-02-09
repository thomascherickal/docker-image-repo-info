## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:9cff0a31fc9923228a746825916d4864ac018f85a32c3fea01dd61e713ce5878
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
$ docker pull debian@sha256:3bdad9e1b3f90992f0176d269be71933ae4e0e8b266c1a1537e488f37fb60d5e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:949a5d0f7a5fca996530fff4d66fd5ce9ca2b13c0bc90be6d3e294cce24f2d51`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:58 GMT
ADD file:5c25f33d305694b2b67b96c3f499cd7a290f7e24f1cbf7b57eb0b1a9e2e31efb in / 
# Thu, 09 Feb 2023 06:13:00 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:13:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9eddf4fc6cef1731110025cf2b9bac8b00ac855cc69b91c4f4c199171c2ace2f`  
		Last Modified: Thu, 09 Feb 2023 06:20:34 GMT  
		Size: 45.9 MB (45916633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b888d549ff318eb603035e9a42626142515036305d3b27b2678862cafc9c99`  
		Last Modified: Thu, 09 Feb 2023 06:20:45 GMT  
		Size: 223.0 B  
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
$ docker pull debian@sha256:00f1b2653c16f6838c261e08e9790dce635938dec3fd72fd60c74556e8cfdaa5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf6dc70ef31be6638a4436494758dbf4078953dba070b08ab8ac8be04bdcbc9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:13:33 GMT
ADD file:46ace83217019849e2d62b30173c4be2d574581608bfe65f4007a707225c6cbe in / 
# Thu, 09 Feb 2023 05:13:34 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 05:13:41 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:595e64097c4300ec9eb28c13e1cb5411d02fa5157588e7ba50c1968e71844e4e`  
		Last Modified: Thu, 09 Feb 2023 05:19:53 GMT  
		Size: 51.2 MB (51207772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ac13207e71d49215b1c07c0e11ee0dcf5b487f0b68f2337fb835fe95d9eb0d`  
		Last Modified: Thu, 09 Feb 2023 05:20:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
