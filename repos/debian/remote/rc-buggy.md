## `debian:rc-buggy`

```console
$ docker pull debian@sha256:bd83cad723b91a8113fd8ba82f903eb426c34d6e62dc0987ae7acde6b041b162
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:e363259cb289ee0fa871225f86d0f0db5c72a752eb99c19a2d2d670adede3b2f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51549760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5112a3c5120891db4b5f78b7416d3fc023f38d0ff5d23323c247adb07fe6d4e6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:22:27 GMT
ADD file:5055617b757ba2ab1ac6772dc2ee4cfe2ba79dd3900150b470dc61e950b9ce78 in / 
# Sat, 01 Feb 2020 17:22:27 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:25:01 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:32a93ca5e0379da8be0d576367bec537380c472d398bfe5587345c3b95c3bf4e`  
		Last Modified: Sat, 01 Feb 2020 17:27:53 GMT  
		Size: 51.5 MB (51549534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab01b650122ab6a2d4d14835931be0e316a3f295bcfdebb1cd5b92815c87edc3`  
		Last Modified: Sat, 01 Feb 2020 17:30:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:f7d00200b8a361c1c24dc1a74cb2a5a9f10698979ce9be95fc35aa60a0245bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49540933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e706f5fe42914af3a5f1eafd2caa79fb6736e0a1c053071f5898e8c1fde63632`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:52:33 GMT
ADD file:e863dd2efdd5f4a6e29a4da391218d83cf13d07b263a55c438361d48079dd528 in / 
# Sat, 01 Feb 2020 16:52:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:55:16 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:25551be68c42d4da1cad9359e21cdc842a69363b035a77721ddf9ad7db276105`  
		Last Modified: Sat, 01 Feb 2020 16:59:21 GMT  
		Size: 49.5 MB (49540705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5a2852a86975ff9ed71acd2f73480ecaa8f2d2a146105a7af12def788c63c`  
		Last Modified: Sat, 01 Feb 2020 17:02:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:4a39b42d36b30334d34fdb351309624e9fc94a469f5c904653f9f5f30e7bbbb3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47282438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbcec3c54757098b976a26c20a514d9a0ef4e39e848ee12539df8544096ac81c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:02:49 GMT
ADD file:a4c8ca5f07a6e213b314bd30a4cd27bba9df71ed8ad4f5f82c07878e8cf99f39 in / 
# Sat, 01 Feb 2020 17:02:51 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:06:03 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:983ca3edff7a1184ea4165bcc490182822501d698a99e9d6bc8d6c042881bb97`  
		Last Modified: Sat, 01 Feb 2020 17:09:51 GMT  
		Size: 47.3 MB (47282209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626d72ac9f557f53db42a91599066504aa90f699280d8e7c6b7d4a7440bf2267`  
		Last Modified: Sat, 01 Feb 2020 17:12:56 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:a2a0a0539db37620c276923de1389cbe00af0ef5d7ff3881459cb15f6d03d40f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50506193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73cc9047b7908a0f76b4cc341e4b5aa4f847c828a553084fb3a025e6be5cbdaf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:58 GMT
ADD file:636edb6845120aa418f3291c0858ab38c7d658cb2790c08b113e8068fe152a32 in / 
# Sat, 01 Feb 2020 16:42:00 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:44:39 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a3f06cbd9a524c44b9b8c92922dc9c06d87668d76af414bd34aeb7238502e475`  
		Last Modified: Sat, 01 Feb 2020 16:47:18 GMT  
		Size: 50.5 MB (50505966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4554b3a4141fe6ec503ef574315adc11f4dbe07069f0b9aa568063a89a2c2dda`  
		Last Modified: Sat, 01 Feb 2020 16:50:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:f1176fb2e2d8c7863d304909b64c9837e288bbd322f9fb7b2e9526f6326fedc1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52680018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:260659741db57588eba3fad884b0157818993f7a9af8bfe5a233876c20a43b50`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:00 GMT
ADD file:941e54a7461d61d84748dacc44e888cce50acfb10e34f38a7e4083e19f23b7ce in / 
# Sat, 01 Feb 2020 16:41:01 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:43:06 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8901e4e25f1677947cce32c9111e1a14e167a08c1c9b0f38aa3b62ad8dfa24aa`  
		Last Modified: Sat, 01 Feb 2020 16:46:18 GMT  
		Size: 52.7 MB (52679793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922cf9e65f569188d4d0521c24565a61116234b3df879878fc8d5906e5d5977e`  
		Last Modified: Sat, 01 Feb 2020 16:48:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:a7ae674298f93f6cb93de731353feff954b82150c12a2a8cd12676ffdab2abce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.3 MB (55349273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e282e7d230b72b2f6876864b1e32b6c20e75d41ffd1390dec83d823d5dadf17`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:19:01 GMT
ADD file:2546930304b6d429e56e56557d14acb509152fb02a657d195dc0595d0f5a4523 in / 
# Sat, 01 Feb 2020 17:19:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:22:36 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f9186c7a47276773316addd180b90c065065663e993fe107956ff3f68e5245ad`  
		Last Modified: Sat, 01 Feb 2020 17:28:20 GMT  
		Size: 55.3 MB (55349044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01e7d0bb44913ee63bde01454c1250d94799fc985987c4861b422edc2881284`  
		Last Modified: Sat, 01 Feb 2020 17:33:27 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:d1ac88a9aa29cc4062664e233cc446347c4d519cc046e15f86d217ee71928040
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50192539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51915cb465344b2349742e8e88503081fcac665d30b9ac97427c002c0daa6334`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:00 GMT
ADD file:967a85341ab042321428ced1b4d7f5dbdbb8d9f2356b825a4904ac635fd3d22d in / 
# Sat, 01 Feb 2020 16:43:03 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:44:45 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0f7573b6b276747f41f68da62a4262a7441ff49e4c1231d18c674b31be00a6d0`  
		Last Modified: Sat, 01 Feb 2020 16:46:30 GMT  
		Size: 50.2 MB (50192313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657ca68076ac08d81e204617c21eb9580bb20f8e7f6b89677b8b3f7371960049`  
		Last Modified: Sat, 01 Feb 2020 16:48:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
