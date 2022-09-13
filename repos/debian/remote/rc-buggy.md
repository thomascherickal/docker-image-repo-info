## `debian:rc-buggy`

```console
$ docker pull debian@sha256:7ab4ec41fc08c37a6b6fb0cc40d829ec5e9760d223821457ca594c587ea4e458
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:fce329a56f47564bf2d6e5a9b15f02524b1e626f7a9a669bb81c5d7558321575
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52643782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c39a14745bc3b7b8073887738a8f70a3ce11450107cf459be8bcdc9212019e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:57:16 GMT
ADD file:7b7161ef988532de9a1ae3caee50f4337a445cd5d88bfe1da455ad45111e2a4f in / 
# Tue, 13 Sep 2022 00:57:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:58:26 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:fbb5199f866b772d7999f8d0fead2c513b95972d6d32ec2c8e29311458f0855f`  
		Last Modified: Tue, 13 Sep 2022 01:02:12 GMT  
		Size: 52.6 MB (52643556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e17847eda4d96df4e758ef1e8baa7097b60560bf2e504be20f159da426691b`  
		Last Modified: Tue, 13 Sep 2022 01:04:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:b17056597ba8bee3714c1383a643eab8a7c5e50fe06f8772ce875a0b24a789ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51786201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bd36a94fde9853a0930a1578a9a7ab430db65656f046653c1084c5dfba5e4f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:56 GMT
ADD file:deaaf7142ee9e9a9e95756080e3fc42695c32c1325ff22432d1a8335978dc0c7 in / 
# Tue, 13 Sep 2022 00:53:57 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:56:50 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2e65672912f1f23209ba2457b7da75b0ac0f01a46e88659ca267298886972343`  
		Last Modified: Tue, 13 Sep 2022 01:01:43 GMT  
		Size: 51.8 MB (51785975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5fc172424b64b7458f7121b0b9650cf3c2549c705a2b34602884eb448aa8b5`  
		Last Modified: Tue, 13 Sep 2022 01:05:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:8569ece440609d81c7eb23818478c2f7766a424b7f302621cd0da8da27942e3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49637644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99936c62d1a323b576d48e7d440022ef12b471793b201cfd4865e4096a7a7476`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:44:30 GMT
ADD file:63335401d9730857a474088e836b58820d062d53a4d008379a3f0bab91891ee7 in / 
# Tue, 23 Aug 2022 01:44:30 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:46:28 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:abce9a6a026c05f336d24d7c79af29d2f108767252a4737864125c7cd16cb946`  
		Last Modified: Tue, 23 Aug 2022 01:52:08 GMT  
		Size: 49.6 MB (49637416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e665ac7065911bffbaa24f2b1e588d3877e45fe7dd89eab976de2360f901b0`  
		Last Modified: Tue, 23 Aug 2022 01:54:56 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:4519d104f78130d4c92a73149d01f365fc9db4c1e02ec1d83e24b00ad07887ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53220861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c05b2e52b3b490a32cb2a29289437731d49e0ed08c51d9c7bbdc79f5aca15651`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:33 GMT
ADD file:03a6abbfc4f7f5b036b595b68d32dab2760788223365adbadd691cc6b97d3f9f in / 
# Tue, 23 Aug 2022 01:53:34 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:55:02 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:11a10710f625b85736b19b89ebf063edde4e3f2dedab0a6cc94db39e134d8cfe`  
		Last Modified: Tue, 23 Aug 2022 01:59:52 GMT  
		Size: 53.2 MB (53220635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467a8b74033da02e2ef44307af20b306d24860d24efe2d1a605425fb53e975ab`  
		Last Modified: Tue, 23 Aug 2022 02:02:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:0daaae98fc377b9b23146374b274259dc21faa1550fe78194d074d87fb7c9f7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54133919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01a18d59c9a2ea2e285beea75035380a50c02d834e01df7013077056e818cb3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:44 GMT
ADD file:56a765ed5b9c59576a105c4e82da61f928406a2ef950e7cada80b5c269a1acda in / 
# Tue, 23 Aug 2022 01:03:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:05:14 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:05690d5133887cdda89e6ae4808c08e8a92acf2163ce992d8bacbed497b1ddd7`  
		Last Modified: Tue, 23 Aug 2022 01:10:25 GMT  
		Size: 54.1 MB (54133693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a9536329a6706ca94bc60a654ea2e92e3186158fc0352c80c80866d3c08f16`  
		Last Modified: Tue, 23 Aug 2022 01:13:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:9696d90fae16cf745e90e9969280aafe3815fc7e4bf5b6969aad058462bf566a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53216859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea1f44a513ec588c37eafb3901eefb497af60fa63fe64d74e8948e5c424ed00`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:52 GMT
ADD file:372730632835dde60a084d1dc5d1d8d7840a118d3aa6413f1568d2a939e39e05 in / 
# Tue, 23 Aug 2022 00:11:58 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:16:23 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f6fdf476c348ab651944f6f008015e5c5184fa9f5620904fc65599b044dd5761`  
		Last Modified: Tue, 23 Aug 2022 00:20:20 GMT  
		Size: 53.2 MB (53216630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ddf2d67b6addc7804c51ac4e7b7d0e5ba53c3f5e82c8de6043acd4b789f339`  
		Last Modified: Tue, 23 Aug 2022 00:24:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:214ea5fe334c28c175af44d1bd8826ed816ffdcfb9cbebd01fdb0ddd8d9d015c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57314111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b881de9e9ef1821aa70faba9dc0072c4fa5416666d80fce0726ac9840c480fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:25:10 GMT
ADD file:7b8a9c1fc05e75d845ea719c57047ae432cceb7645d270a99b117d0e4e0ffb33 in / 
# Tue, 23 Aug 2022 01:25:13 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:27:28 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:515f00ecba82250b75d6d9987193afd77293c07bfaf7a95ae024c05c73a8cb3a`  
		Last Modified: Tue, 23 Aug 2022 01:31:07 GMT  
		Size: 57.3 MB (57313882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f266c47af7db10bcce91f8285a4b186ee873dbf381a654a2594defa67f75ca6`  
		Last Modified: Tue, 23 Aug 2022 01:34:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:c6263fa0d0eccecede739e225901caff707e49cb633cfd5fda1a8432571a8a03
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51537231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32a6da04fccaece0113a49ed0a0690f1ace827351dff6bdb6da47b3968802ba2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:19 GMT
ADD file:c95e2b098d871c8f60e72d16096a4bcce80e256166b62df3ac0abf8c1cc5384d in / 
# Tue, 13 Sep 2022 00:48:22 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:50:12 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a47738c5650c377467230bf819bb4be695718c6effbf5489b6e0fc8e11229d95`  
		Last Modified: Tue, 13 Sep 2022 00:52:55 GMT  
		Size: 51.5 MB (51537006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8beada893fe95a8f5664c2cc7e573b4bf40c9982c0907c9154dc41afc8d0fd3`  
		Last Modified: Tue, 13 Sep 2022 00:54:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
