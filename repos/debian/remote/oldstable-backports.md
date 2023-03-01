## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:b559ebe0a6af57fb9ec6fa4d189acb03efaebe5c6706a273cd4e9eb1d9cd8a44
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
$ docker pull debian@sha256:34b7941b50ec36e2639b99b1de127c9a26ff694efc40e8e183c4a4e440b30699
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95d52d5909bff9a48e8bfb27887fd4f0ca72a8930b61e64ba66dd6dfb99f84e9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:21 GMT
ADD file:ccafb0d4746567d93ef1a3ac27400488eb9d41acb93e3a18f1e77377ff97c8f1 in / 
# Wed, 01 Mar 2023 01:58:21 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:58:25 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:548799b11fde653a3d163dd7bb5426257f268b7c2b7133518be0cd64df798a73`  
		Last Modified: Wed, 01 Mar 2023 02:04:13 GMT  
		Size: 45.9 MB (45916081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10367b73896194527344a35e5c5fa3746f93197523f34ef9b1c66a6faba22c22`  
		Last Modified: Wed, 01 Mar 2023 02:04:23 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:e933844f3fedff1eb34d732d82c50b94af343fa3f594b9d67420861d8bed2849
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49240231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe2d4a15e43b3fe9aeb10949454b84ed03ee547f2470f5ce97d9fc2b72ad968`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:21:03 GMT
ADD file:d30c63a27172705fbf489d5393d7c5c2e1e89d8243e39b9eeef4ddb8ec9c7fba in / 
# Wed, 01 Mar 2023 02:21:04 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:21:07 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:eb7717bd039c193f3eef114c67fef1b76e73860d00d322acef59019c6c561a60`  
		Last Modified: Wed, 01 Mar 2023 02:25:13 GMT  
		Size: 49.2 MB (49240003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a92d766846ffbbab94fd3f24ac9bd4155c7be330057a44bd1434c44f01bd9fc`  
		Last Modified: Wed, 01 Mar 2023 02:25:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:5c84b108adc339d7d5a956e3967ebc6f03bf7fe6ba55d217eb9f4ac118ae75e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1056e4c655fa99d313bcad7fa44b70590c4202e03d56b7ec9e2756a5276dada`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:44 GMT
ADD file:ba1f3b4548523bc0d8aa4ed5bbe6fc6bb29fda65a8fcc8c60ef142590b253f83 in / 
# Wed, 01 Mar 2023 01:39:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:39:49 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2feb9b8f3b71378feaaaa0653ed32983eb258b997f8ac24d01093bc3d1a25c0a`  
		Last Modified: Wed, 01 Mar 2023 01:46:01 GMT  
		Size: 51.2 MB (51207370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ed57e711eec887a1071d8aaddc50889c1b0994c486fbfc4443503eab225f1`  
		Last Modified: Wed, 01 Mar 2023 01:46:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
