## `debian:experimental-20211220`

```console
$ docker pull debian@sha256:a003df52e22b419bcf0b5e52b548f9d837a7a7799ca89d35f64ddfa45db72229
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `debian:experimental-20211220` - linux; amd64

```console
$ docker pull debian@sha256:ae5a92c4a5e74db308253f8a3d61b011e80a52f0935b7c6c38d962ec234aacaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55798195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef37997e03fbd52ec8a362c8fb10926d1f76b1f83b120a1f26a11f81e5ec787`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:25:12 GMT
ADD file:48125de314404b5ced792c318b5f07c798b024ff765bfb646af1bbf4772924fc in / 
# Tue, 21 Dec 2021 01:25:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:25:25 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:bd3794a0f2768355393f3911f660530b0280b17bed920ed2afb90c7aa975de1d`  
		Last Modified: Tue, 21 Dec 2021 01:32:33 GMT  
		Size: 55.8 MB (55797970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb6443f37b6eb317c0e1f61f8e5bb5fdc4811925b07e4b5273a650d2d64c79b`  
		Last Modified: Tue, 21 Dec 2021 01:32:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20211220` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:70695dd61c309a9352530aa11778225f1ac9ba8a3d38230fed2271e13eea9f96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54781096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19d944ae667df30aed2d652d5019fb0b77ff70d9e6d9c17fad3f0bd0b3d55bf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:45:13 GMT
ADD file:7bbfdc666ed306d3c9e28a2b869378806f86c1640ea684e9f14a54de89208f1f in / 
# Tue, 21 Dec 2021 01:45:14 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:45:28 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:067276bef0f1e1a0d26e7028971339aee89b0a9a61bc5b45aa7efbf4b08ab8ff`  
		Last Modified: Tue, 21 Dec 2021 01:54:08 GMT  
		Size: 54.8 MB (54780875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05072134342ecf6f3089ef264f4f833be7661975a24dbfcc25e105e8f6415c79`  
		Last Modified: Tue, 21 Dec 2021 01:54:33 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20211220` - linux; 386

```console
$ docker pull debian@sha256:80da6c305335ce03d872e0f13582d431ca5242e7428833eb1e5bda994ee2f51d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.9 MB (56851919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fdda4af7c02361723a8b762a99b3da05b73422bcc80c4d12b31aa2005e8dec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:13 GMT
ADD file:f52ad383331ad64becf207e93847af259a33309a89447a23e6c38c82aa9685f1 in / 
# Tue, 21 Dec 2021 01:44:14 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:44:30 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:24e98c1e6129732b99ca0b8ac8d6ecb76c94380d46f6bf54df2db7eb94bbb3be`  
		Last Modified: Tue, 21 Dec 2021 01:55:03 GMT  
		Size: 56.9 MB (56851699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c807ab96816302ea8431aafda6ebdd59787f1b62317676af8b0fd9c55d1a22c2`  
		Last Modified: Tue, 21 Dec 2021 01:55:33 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20211220` - linux; s390x

```console
$ docker pull debian@sha256:8e911f89e1853b29beaa5b5f25297e2ff2657aa9d2f678d2ecd4aaec7d4f0af5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54090402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e75251548d1d0cd053114d0529041e5c6e4ac152d31bbd5a2c87d786c606abf6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:58 GMT
ADD file:e76938b8ad072e015b92e5de79be47dd882886dbc87218441c2ea6c4023aa989 in / 
# Tue, 21 Dec 2021 01:45:00 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:45:16 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1335c6a8992ed83758a594f9813a6eab266e49fa2cfb3cd09413a599ae0941a3`  
		Last Modified: Tue, 21 Dec 2021 01:51:03 GMT  
		Size: 54.1 MB (54090179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8c7e653d714f040d14cdefed97fc39acb48b66a0264996fa10675a969e5594`  
		Last Modified: Tue, 21 Dec 2021 01:51:22 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
