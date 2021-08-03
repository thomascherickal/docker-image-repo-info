<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20210721.2`](#amazonlinux20202107212)
-	[`amazonlinux:2.0.20210721.2-with-sources`](#amazonlinux20202107212-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20210721.0`](#amazonlinux2018030202107210)
-	[`amazonlinux:2018.03.0.20210721.0-with-sources`](#amazonlinux2018030202107210-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:d27370314abb4389b76dabe6721f034dd141e990168ce134f6769b111fcb3bf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:42daf1b227ae9fe6dd053320b910d659926fadc02f348b65b9cb182bc79acd37
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62447851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c591bfdb12c884bc1ff404b567bca8751f467d48442239f65ab63a1e18552e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:20:15 GMT
ADD file:4b16f85f418eaa2dc5061f87bad84182ff9a0908cae737752f418c8ee3b9fa50 in / 
# Mon, 02 Aug 2021 23:20:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:09b6f0cc07c54d7b46e1b5e0ada4bdd9506bec2fae181bc9715d654a48e750e4`  
		Last Modified: Mon, 02 Aug 2021 23:21:59 GMT  
		Size: 62.4 MB (62447851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:98883e114fdf3647d220fc3c13c820136d054972f7debfda13bb42bea93b58c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:faf1c1f381376b16dba4bb6422f7d66657306dcb2c5e3726e0f76c4e4d2a4d9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515035249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ecef2b71e30d2675a113d05960cbcbe07f2fd2cf2b6eb0d9e8bc9f39aa9cf6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:20:15 GMT
ADD file:4b16f85f418eaa2dc5061f87bad84182ff9a0908cae737752f418c8ee3b9fa50 in / 
# Mon, 02 Aug 2021 23:20:16 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:20:42 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-96900e11bba57b06a0616a0bb6faa31e2d768b29001d11fdfa65375353e22e14.tar.gz"  && echo "a7a8bd81dd43de9a5705d1c943c0fb3dac49c485a21cd198a445164eab8a7b02  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:09b6f0cc07c54d7b46e1b5e0ada4bdd9506bec2fae181bc9715d654a48e750e4`  
		Last Modified: Mon, 02 Aug 2021 23:21:59 GMT  
		Size: 62.4 MB (62447851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2b693288ab0a22247e28a2e046ea9615b796e0f7e85c4e690f029ac7aa0b3d`  
		Last Modified: Mon, 02 Aug 2021 23:22:28 GMT  
		Size: 452.6 MB (452587398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:93e55c026fe5dba304ff3f24690b07cb39f610b160844a575bb8f3fec41b3a5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:01877b26680da875b275c57eab5cfc6c6b88d4d86f549c1820be19da720385e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61965674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d85ab0980c91ee67db6e44ba204dfe39f7bc0c51c0233c2038337f34a831aa6a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:19:37 GMT
ADD file:4cbe5850096b1ae39fe377dfe25245d1d635eafcbe0f58e1dc20e75716131cd3 in / 
# Mon, 02 Aug 2021 23:19:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d36ac8072fa22f99e1b8c66984e2fa09296890d37276e65dd4dc83503a3cf4c2`  
		Last Modified: Fri, 30 Jul 2021 16:48:36 GMT  
		Size: 62.0 MB (61965674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:048dd4c931375373002bc8d47f7fe29e65cba964f44a326ac1ff168d6848d787
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63546854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e061d71970e6f0b5a825826d5dd5d10cb9411fd6fdfe7aec8f2b9c4324816d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:39:27 GMT
ADD file:d3c0f2c17135c35c4fec5abfa25c0f77c04517a31107e754d182e5985e962fbe in / 
# Mon, 02 Aug 2021 23:39:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:63f4e95aab55922b1bd380df3233d11cc34653d71768884de620d921e24daf17`  
		Last Modified: Mon, 02 Aug 2021 23:40:24 GMT  
		Size: 63.5 MB (63546854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:10a89e26c570e6e9673182484c5509396099ab492edd8cadef2c7e1f072df2b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6beffd46592ecbdb9e7bb63998a8adbe73203b2a0b6411cf1546046d7188b7a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542940673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867fa952e4d51ef0c41cf888e945cf0903a76806f0cd2ef2e9cff60d01357584`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:19:37 GMT
ADD file:4cbe5850096b1ae39fe377dfe25245d1d635eafcbe0f58e1dc20e75716131cd3 in / 
# Mon, 02 Aug 2021 23:19:38 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:20:03 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e832e506d930c525d101385e90322663126ac63fdca0b7d3797be8c2f6efb8bd.tar.gz"  && echo "fe52788ded649399eb7ba6e867c4373d3eafc99b9353955de47a39408b8ad366  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d36ac8072fa22f99e1b8c66984e2fa09296890d37276e65dd4dc83503a3cf4c2`  
		Last Modified: Fri, 30 Jul 2021 16:48:36 GMT  
		Size: 62.0 MB (61965674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4581db6484e98433b91089f32a94db775460fb253ce6e3204dfc7b3349e97a10`  
		Last Modified: Mon, 02 Aug 2021 23:21:38 GMT  
		Size: 481.0 MB (480974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:192eeb0e12a69e30106d70e84fb0f0d3486a79de43e92a9f24be379cedfd7fa0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544521863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd858173ea3067285d35fb6e39c53242ea58d9b08897493eada5f2c603ad966a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:39:27 GMT
ADD file:d3c0f2c17135c35c4fec5abfa25c0f77c04517a31107e754d182e5985e962fbe in / 
# Mon, 02 Aug 2021 23:39:28 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:39:50 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e832e506d930c525d101385e90322663126ac63fdca0b7d3797be8c2f6efb8bd.tar.gz"  && echo "fe52788ded649399eb7ba6e867c4373d3eafc99b9353955de47a39408b8ad366  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:63f4e95aab55922b1bd380df3233d11cc34653d71768884de620d921e24daf17`  
		Last Modified: Mon, 02 Aug 2021 23:40:24 GMT  
		Size: 63.5 MB (63546854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cadb9bf01fac34b09b53130aea8878867dd024801d8042a65d7cee698eb48e8`  
		Last Modified: Mon, 02 Aug 2021 23:41:03 GMT  
		Size: 481.0 MB (480975009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20210721.2`

```console
$ docker pull amazonlinux@sha256:93e55c026fe5dba304ff3f24690b07cb39f610b160844a575bb8f3fec41b3a5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20210721.2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:01877b26680da875b275c57eab5cfc6c6b88d4d86f549c1820be19da720385e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61965674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d85ab0980c91ee67db6e44ba204dfe39f7bc0c51c0233c2038337f34a831aa6a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:19:37 GMT
ADD file:4cbe5850096b1ae39fe377dfe25245d1d635eafcbe0f58e1dc20e75716131cd3 in / 
# Mon, 02 Aug 2021 23:19:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d36ac8072fa22f99e1b8c66984e2fa09296890d37276e65dd4dc83503a3cf4c2`  
		Last Modified: Fri, 30 Jul 2021 16:48:36 GMT  
		Size: 62.0 MB (61965674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20210721.2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:048dd4c931375373002bc8d47f7fe29e65cba964f44a326ac1ff168d6848d787
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63546854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e061d71970e6f0b5a825826d5dd5d10cb9411fd6fdfe7aec8f2b9c4324816d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:39:27 GMT
ADD file:d3c0f2c17135c35c4fec5abfa25c0f77c04517a31107e754d182e5985e962fbe in / 
# Mon, 02 Aug 2021 23:39:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:63f4e95aab55922b1bd380df3233d11cc34653d71768884de620d921e24daf17`  
		Last Modified: Mon, 02 Aug 2021 23:40:24 GMT  
		Size: 63.5 MB (63546854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20210721.2-with-sources`

```console
$ docker pull amazonlinux@sha256:10a89e26c570e6e9673182484c5509396099ab492edd8cadef2c7e1f072df2b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20210721.2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6beffd46592ecbdb9e7bb63998a8adbe73203b2a0b6411cf1546046d7188b7a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542940673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867fa952e4d51ef0c41cf888e945cf0903a76806f0cd2ef2e9cff60d01357584`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:19:37 GMT
ADD file:4cbe5850096b1ae39fe377dfe25245d1d635eafcbe0f58e1dc20e75716131cd3 in / 
# Mon, 02 Aug 2021 23:19:38 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:20:03 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e832e506d930c525d101385e90322663126ac63fdca0b7d3797be8c2f6efb8bd.tar.gz"  && echo "fe52788ded649399eb7ba6e867c4373d3eafc99b9353955de47a39408b8ad366  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d36ac8072fa22f99e1b8c66984e2fa09296890d37276e65dd4dc83503a3cf4c2`  
		Last Modified: Fri, 30 Jul 2021 16:48:36 GMT  
		Size: 62.0 MB (61965674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4581db6484e98433b91089f32a94db775460fb253ce6e3204dfc7b3349e97a10`  
		Last Modified: Mon, 02 Aug 2021 23:21:38 GMT  
		Size: 481.0 MB (480974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20210721.2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:192eeb0e12a69e30106d70e84fb0f0d3486a79de43e92a9f24be379cedfd7fa0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544521863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd858173ea3067285d35fb6e39c53242ea58d9b08897493eada5f2c603ad966a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:39:27 GMT
ADD file:d3c0f2c17135c35c4fec5abfa25c0f77c04517a31107e754d182e5985e962fbe in / 
# Mon, 02 Aug 2021 23:39:28 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:39:50 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e832e506d930c525d101385e90322663126ac63fdca0b7d3797be8c2f6efb8bd.tar.gz"  && echo "fe52788ded649399eb7ba6e867c4373d3eafc99b9353955de47a39408b8ad366  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:63f4e95aab55922b1bd380df3233d11cc34653d71768884de620d921e24daf17`  
		Last Modified: Mon, 02 Aug 2021 23:40:24 GMT  
		Size: 63.5 MB (63546854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cadb9bf01fac34b09b53130aea8878867dd024801d8042a65d7cee698eb48e8`  
		Last Modified: Mon, 02 Aug 2021 23:41:03 GMT  
		Size: 481.0 MB (480975009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:d27370314abb4389b76dabe6721f034dd141e990168ce134f6769b111fcb3bf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:42daf1b227ae9fe6dd053320b910d659926fadc02f348b65b9cb182bc79acd37
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62447851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c591bfdb12c884bc1ff404b567bca8751f467d48442239f65ab63a1e18552e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:20:15 GMT
ADD file:4b16f85f418eaa2dc5061f87bad84182ff9a0908cae737752f418c8ee3b9fa50 in / 
# Mon, 02 Aug 2021 23:20:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:09b6f0cc07c54d7b46e1b5e0ada4bdd9506bec2fae181bc9715d654a48e750e4`  
		Last Modified: Mon, 02 Aug 2021 23:21:59 GMT  
		Size: 62.4 MB (62447851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:98883e114fdf3647d220fc3c13c820136d054972f7debfda13bb42bea93b58c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:faf1c1f381376b16dba4bb6422f7d66657306dcb2c5e3726e0f76c4e4d2a4d9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515035249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ecef2b71e30d2675a113d05960cbcbe07f2fd2cf2b6eb0d9e8bc9f39aa9cf6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:20:15 GMT
ADD file:4b16f85f418eaa2dc5061f87bad84182ff9a0908cae737752f418c8ee3b9fa50 in / 
# Mon, 02 Aug 2021 23:20:16 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:20:42 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-96900e11bba57b06a0616a0bb6faa31e2d768b29001d11fdfa65375353e22e14.tar.gz"  && echo "a7a8bd81dd43de9a5705d1c943c0fb3dac49c485a21cd198a445164eab8a7b02  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:09b6f0cc07c54d7b46e1b5e0ada4bdd9506bec2fae181bc9715d654a48e750e4`  
		Last Modified: Mon, 02 Aug 2021 23:21:59 GMT  
		Size: 62.4 MB (62447851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2b693288ab0a22247e28a2e046ea9615b796e0f7e85c4e690f029ac7aa0b3d`  
		Last Modified: Mon, 02 Aug 2021 23:22:28 GMT  
		Size: 452.6 MB (452587398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20210721.0`

```console
$ docker pull amazonlinux@sha256:d27370314abb4389b76dabe6721f034dd141e990168ce134f6769b111fcb3bf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20210721.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:42daf1b227ae9fe6dd053320b910d659926fadc02f348b65b9cb182bc79acd37
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62447851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c591bfdb12c884bc1ff404b567bca8751f467d48442239f65ab63a1e18552e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:20:15 GMT
ADD file:4b16f85f418eaa2dc5061f87bad84182ff9a0908cae737752f418c8ee3b9fa50 in / 
# Mon, 02 Aug 2021 23:20:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:09b6f0cc07c54d7b46e1b5e0ada4bdd9506bec2fae181bc9715d654a48e750e4`  
		Last Modified: Mon, 02 Aug 2021 23:21:59 GMT  
		Size: 62.4 MB (62447851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20210721.0-with-sources`

```console
$ docker pull amazonlinux@sha256:98883e114fdf3647d220fc3c13c820136d054972f7debfda13bb42bea93b58c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20210721.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:faf1c1f381376b16dba4bb6422f7d66657306dcb2c5e3726e0f76c4e4d2a4d9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515035249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ecef2b71e30d2675a113d05960cbcbe07f2fd2cf2b6eb0d9e8bc9f39aa9cf6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:20:15 GMT
ADD file:4b16f85f418eaa2dc5061f87bad84182ff9a0908cae737752f418c8ee3b9fa50 in / 
# Mon, 02 Aug 2021 23:20:16 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:20:42 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-96900e11bba57b06a0616a0bb6faa31e2d768b29001d11fdfa65375353e22e14.tar.gz"  && echo "a7a8bd81dd43de9a5705d1c943c0fb3dac49c485a21cd198a445164eab8a7b02  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:09b6f0cc07c54d7b46e1b5e0ada4bdd9506bec2fae181bc9715d654a48e750e4`  
		Last Modified: Mon, 02 Aug 2021 23:21:59 GMT  
		Size: 62.4 MB (62447851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2b693288ab0a22247e28a2e046ea9615b796e0f7e85c4e690f029ac7aa0b3d`  
		Last Modified: Mon, 02 Aug 2021 23:22:28 GMT  
		Size: 452.6 MB (452587398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:93e55c026fe5dba304ff3f24690b07cb39f610b160844a575bb8f3fec41b3a5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:01877b26680da875b275c57eab5cfc6c6b88d4d86f549c1820be19da720385e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61965674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d85ab0980c91ee67db6e44ba204dfe39f7bc0c51c0233c2038337f34a831aa6a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:19:37 GMT
ADD file:4cbe5850096b1ae39fe377dfe25245d1d635eafcbe0f58e1dc20e75716131cd3 in / 
# Mon, 02 Aug 2021 23:19:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d36ac8072fa22f99e1b8c66984e2fa09296890d37276e65dd4dc83503a3cf4c2`  
		Last Modified: Fri, 30 Jul 2021 16:48:36 GMT  
		Size: 62.0 MB (61965674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:048dd4c931375373002bc8d47f7fe29e65cba964f44a326ac1ff168d6848d787
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63546854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e061d71970e6f0b5a825826d5dd5d10cb9411fd6fdfe7aec8f2b9c4324816d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:39:27 GMT
ADD file:d3c0f2c17135c35c4fec5abfa25c0f77c04517a31107e754d182e5985e962fbe in / 
# Mon, 02 Aug 2021 23:39:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:63f4e95aab55922b1bd380df3233d11cc34653d71768884de620d921e24daf17`  
		Last Modified: Mon, 02 Aug 2021 23:40:24 GMT  
		Size: 63.5 MB (63546854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:10a89e26c570e6e9673182484c5509396099ab492edd8cadef2c7e1f072df2b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6beffd46592ecbdb9e7bb63998a8adbe73203b2a0b6411cf1546046d7188b7a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542940673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867fa952e4d51ef0c41cf888e945cf0903a76806f0cd2ef2e9cff60d01357584`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:19:37 GMT
ADD file:4cbe5850096b1ae39fe377dfe25245d1d635eafcbe0f58e1dc20e75716131cd3 in / 
# Mon, 02 Aug 2021 23:19:38 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:20:03 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e832e506d930c525d101385e90322663126ac63fdca0b7d3797be8c2f6efb8bd.tar.gz"  && echo "fe52788ded649399eb7ba6e867c4373d3eafc99b9353955de47a39408b8ad366  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d36ac8072fa22f99e1b8c66984e2fa09296890d37276e65dd4dc83503a3cf4c2`  
		Last Modified: Fri, 30 Jul 2021 16:48:36 GMT  
		Size: 62.0 MB (61965674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4581db6484e98433b91089f32a94db775460fb253ce6e3204dfc7b3349e97a10`  
		Last Modified: Mon, 02 Aug 2021 23:21:38 GMT  
		Size: 481.0 MB (480974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:192eeb0e12a69e30106d70e84fb0f0d3486a79de43e92a9f24be379cedfd7fa0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544521863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd858173ea3067285d35fb6e39c53242ea58d9b08897493eada5f2c603ad966a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:39:27 GMT
ADD file:d3c0f2c17135c35c4fec5abfa25c0f77c04517a31107e754d182e5985e962fbe in / 
# Mon, 02 Aug 2021 23:39:28 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:39:50 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e832e506d930c525d101385e90322663126ac63fdca0b7d3797be8c2f6efb8bd.tar.gz"  && echo "fe52788ded649399eb7ba6e867c4373d3eafc99b9353955de47a39408b8ad366  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:63f4e95aab55922b1bd380df3233d11cc34653d71768884de620d921e24daf17`  
		Last Modified: Mon, 02 Aug 2021 23:40:24 GMT  
		Size: 63.5 MB (63546854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cadb9bf01fac34b09b53130aea8878867dd024801d8042a65d7cee698eb48e8`  
		Last Modified: Mon, 02 Aug 2021 23:41:03 GMT  
		Size: 481.0 MB (480975009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
