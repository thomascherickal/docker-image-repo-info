## `debian:experimental`

```console
$ docker pull debian@sha256:1dc9fb341d10b1c469b716e910209210db470a7cc77738f2b32114287fbc1b65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental` - linux; amd64

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

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:1a82af1a26c8e3142df6648910031aaa68fb2a3a5d0b02327ee7311a4c0d11e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53226509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a96927b6680bc45d1b50897b3cc2f1c147e3c49e708237e683265aa9c93089`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:00:04 GMT
ADD file:bdb1bf58320a788a3b3115425f34ebf3385ed3fd166fd9f62516fd4f80512490 in / 
# Thu, 02 Dec 2021 03:00:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:00:55 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2d1699f433119b57c3eceaf5d93c93e7ca4a79b6d9bd74ae5d8a94e414aa9e12`  
		Last Modified: Thu, 02 Dec 2021 03:17:44 GMT  
		Size: 53.2 MB (53226285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7b6603ce38ad48f444a48ff36047cc522b88cd118358bc2f38fdf976da5f23`  
		Last Modified: Thu, 02 Dec 2021 03:18:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:f9c85f62bf4fdb01773fb7a2f5fa22aeae0d746cf054824e41d3b8b58c8d35dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50857607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7646a327e5f887fb806cecde8395560626ea4211c46f210c107e93ec3ba4f09f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:12:45 GMT
ADD file:03b458905caf536d61b3add19dc8f858f06c4e82879f3e1cd4587a2c664f4e4a in / 
# Thu, 02 Dec 2021 09:12:46 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:13:20 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b03360ff38e107a289ac03d4fbd1501c05ce15569412d6c2e435c46509a4de82`  
		Last Modified: Thu, 02 Dec 2021 09:30:31 GMT  
		Size: 50.9 MB (50857384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1644a17e5c3669bdef4d7fb815aab60ce87fdd4ecf888f2ec8168ea3732a3f7e`  
		Last Modified: Thu, 02 Dec 2021 09:31:08 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

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

### `debian:experimental` - linux; 386

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

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:22f36216c2ce0fc07cd3d0d14c933947d4ab98bb6db4f034739cfbad1bfcd293
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54455677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6f041258d541a5cd019ee60de00dd8dd7d76be95d6cd5dcfe04c327eda8a2cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:14:01 GMT
ADD file:2d61dbbf49a978c5b903ad6810df99f11bcc9585d06f3fc5eeaa97beb27d6742 in / 
# Thu, 02 Dec 2021 03:14:02 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:14:29 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7e0c1253ea9ee2c36fcc159313f9d8af0a88857a9aba47ea44e0fdee2bcc4881`  
		Last Modified: Thu, 02 Dec 2021 03:52:36 GMT  
		Size: 54.5 MB (54455453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0f42e520aefdff8b68f6604c0e9776716ee6d87ede5acb91bbf48ecbba5e07`  
		Last Modified: Thu, 02 Dec 2021 03:53:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:9894707f571ba621d7921ca0027b53653fd2b16958bb92ea2c2bdabe54b526c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60041524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ee6d7495f7a579484c93d0420b37f02eed8ca1a94936c6a5d8e37724a650172`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:25:56 GMT
ADD file:7e5bc595211481735bf56d25c004454540b6d862f1182a6c081d0ff2af59e55e in / 
# Thu, 02 Dec 2021 07:26:02 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:26:36 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8c52ef0044c78f251a9b910bd764737e42811adf6c3b0eac5a67436f3ed21b44`  
		Last Modified: Thu, 02 Dec 2021 07:36:14 GMT  
		Size: 60.0 MB (60041300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027de17665c2f2511fcac186617e59fde020c7565b240b3155e3f929f92c4ab3`  
		Last Modified: Thu, 02 Dec 2021 07:36:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:efe1ae8eaee5a194a51bd2ba5fb1ec2322c19836a1bd7ecc2de349b316814882
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51509504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0efc905b0f3905b3e9d6ed142793c4295ac6aef4892a5fa16fe25aa311915976`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:19:59 GMT
ADD file:a323413cfbbb9d9c5d8922ab6a65704b34c4b5057fd08cd09ec03166656c6500 in / 
# Thu, 02 Dec 2021 03:20:02 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:23:10 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:cd756f7feb59c540dfa3f77898eb4c318cd0e47cd0f90c29ac1dba47238a0322`  
		Last Modified: Thu, 02 Dec 2021 03:36:06 GMT  
		Size: 51.5 MB (51509275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f36b1fc37c32aca05d3d10d71276780689dab5ce163e9a99474a2dd1a4f76f`  
		Last Modified: Thu, 02 Dec 2021 03:38:43 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

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
