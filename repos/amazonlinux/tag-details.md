<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20220218.1`](#amazonlinux20202202181)
-	[`amazonlinux:2.0.20220218.1-with-sources`](#amazonlinux20202202181-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20220209.0`](#amazonlinux2018030202202090)
-	[`amazonlinux:2018.03.0.20220209.0-with-sources`](#amazonlinux2018030202202090-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20220202.0`](#amazonlinux20220202202020)
-	[`amazonlinux:2022.0.20220202.0-with-sources`](#amazonlinux20220202202020-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:2e21218a068141128509da3b5a0352ac9e8941937ad3d9b34b267369d3eed3a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:10b73bf006c43fff1e2e5f25fd23f11d730145f94fc8d9d96a4de417277ef9b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62366933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef7a8ac5b70aa541fef41e309e139ad535a13bc507122369b6c80fc4980ac6a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 26 Feb 2022 02:36:39 GMT
ADD file:e2a9332f7a6ac3bad7b0c1c9cf654d3a7ff3139013c2a2e315d219e7f51b2f0a in / 
# Sat, 26 Feb 2022 02:36:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:243bb3077bc0f28f0b2dd4489a2aeefa4d1a3afad6aa579aa9de653fc5dde576`  
		Last Modified: Sat, 26 Feb 2022 02:38:16 GMT  
		Size: 62.4 MB (62366933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:9b216b739f4bf9f7bec04e31066705dab48f596b5a778374be44f7c1865c3e44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3a51375eb97e43cd90422b3263eba67b348b05325b274901bac64fa2d26afa94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (514978058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:059a456ad03a6cc52fb1459fa5a68d1921ae1c7295f2528e1bca32b1f5eaa9d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 26 Feb 2022 02:36:39 GMT
ADD file:e2a9332f7a6ac3bad7b0c1c9cf654d3a7ff3139013c2a2e315d219e7f51b2f0a in / 
# Sat, 26 Feb 2022 02:36:40 GMT
CMD ["/bin/bash"]
# Sat, 26 Feb 2022 02:37:12 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-61ca3a50468582bc69c53c50f6e1cb49a44054a672c55189905f1aeeab9e866c.tar.gz"  && echo "d8777443388978ad4e7717cf420aadc073caa843bd410bc5ba7410ec73237440  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:243bb3077bc0f28f0b2dd4489a2aeefa4d1a3afad6aa579aa9de653fc5dde576`  
		Last Modified: Sat, 26 Feb 2022 02:38:16 GMT  
		Size: 62.4 MB (62366933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99fdb0ce658bd85cf1e30c481bafab589fe407d7106e82fde2cdd1ceeff0e3e`  
		Last Modified: Sat, 26 Feb 2022 02:38:46 GMT  
		Size: 452.6 MB (452611125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:3807816d350446a722cfc8cf366e163ebf566a52a333d87372b77320a5d7eb4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:a4cfc190f7c549bc8a3f260a8f3af45ddeae63fb10ccad70f914d411aec1e431
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62237845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab2a8d1dc5555599378fc9c5a5661470b0151ed10e3d663a8fbf0b09d6e3d09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9a75e593b5ca191b5ca33df38a76dae3a64ef1c5166a202cd8aa3896c8ebd36e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63816961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70fe3a7e5673d1977cf1600b59c9e91d75769aea7bff0abfd978fe809a9f8c21`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 02:54:31 GMT
ADD file:d8fe7ad66f762a8aad81401877fc5d61f1a4b58eac91f47145e6e443aa3ac8ee in / 
# Fri, 04 Mar 2022 02:54:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:12990ee66856745f12f3a508d82e3d48a09d0378d91aaca8ca153c3819e7a686`  
		Last Modified: Thu, 03 Mar 2022 02:21:31 GMT  
		Size: 63.8 MB (63816961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:c1ee9fc091e36d67cbe79f8acc9c56c133d8a8f0fcfdd327b2ccdab85bd088b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c2f6a88e3f9cb6221b13a2d961456a081975b936580387b6933cfff6e664af9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.4 MB (485371765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8932d75666cadda98036af5cd135cad7a648d26fc9b62458558ca3b2a56a435`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 23:40:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-86059ff059c15219c13900625367028ea52b1d95d6f6515947fe04983baf9add.tar.gz"  && echo "7cbab49134e393024873c4c8ad4937d84c8b7ed316b4d6260ae6b425cdd89e91  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df40d5f106fd4ab71023a3b15de586ad3165bbec356559856b77c24ad4d33883`  
		Last Modified: Fri, 04 Feb 2022 23:42:04 GMT  
		Size: 423.1 MB (423133920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2896d84d7d4d35a3b2107ee151860013ff99c1b84fe61ee1dc6200724c51e84e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.9 MB (486930828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc9dae5a26f2292aff8c56adebc728b2a363264201f58e30e964116af4c4832`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 02:54:31 GMT
ADD file:d8fe7ad66f762a8aad81401877fc5d61f1a4b58eac91f47145e6e443aa3ac8ee in / 
# Fri, 04 Mar 2022 02:54:32 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 02:54:54 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-743baa7c60c3c54741d5e55ae3430a659604633fb03e9616435ba83760e96755.tar.gz"  && echo "a2d893e0aae7d4bbe63bc587b4df87ae9ba7f2de8a15de13e766f74031044843  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:12990ee66856745f12f3a508d82e3d48a09d0378d91aaca8ca153c3819e7a686`  
		Last Modified: Thu, 03 Mar 2022 02:21:31 GMT  
		Size: 63.8 MB (63816961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88df431ce701ae5994531d21801baa8d60ebb952c1675cee8006761b12e1bb3`  
		Last Modified: Fri, 04 Mar 2022 02:56:21 GMT  
		Size: 423.1 MB (423113867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220218.1`

```console
$ docker pull amazonlinux@sha256:2e8507165756803648f581de05604831adaa390d970a7733318cc15dc256914f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220218.1` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9a75e593b5ca191b5ca33df38a76dae3a64ef1c5166a202cd8aa3896c8ebd36e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63816961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70fe3a7e5673d1977cf1600b59c9e91d75769aea7bff0abfd978fe809a9f8c21`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 02:54:31 GMT
ADD file:d8fe7ad66f762a8aad81401877fc5d61f1a4b58eac91f47145e6e443aa3ac8ee in / 
# Fri, 04 Mar 2022 02:54:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:12990ee66856745f12f3a508d82e3d48a09d0378d91aaca8ca153c3819e7a686`  
		Last Modified: Thu, 03 Mar 2022 02:21:31 GMT  
		Size: 63.8 MB (63816961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220218.1-with-sources`

```console
$ docker pull amazonlinux@sha256:bf604b80464fc7fe468964e7b0df7d20eb770858c8aa60c1173587aec0b6382b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220218.1-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2896d84d7d4d35a3b2107ee151860013ff99c1b84fe61ee1dc6200724c51e84e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.9 MB (486930828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc9dae5a26f2292aff8c56adebc728b2a363264201f58e30e964116af4c4832`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 02:54:31 GMT
ADD file:d8fe7ad66f762a8aad81401877fc5d61f1a4b58eac91f47145e6e443aa3ac8ee in / 
# Fri, 04 Mar 2022 02:54:32 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 02:54:54 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-743baa7c60c3c54741d5e55ae3430a659604633fb03e9616435ba83760e96755.tar.gz"  && echo "a2d893e0aae7d4bbe63bc587b4df87ae9ba7f2de8a15de13e766f74031044843  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:12990ee66856745f12f3a508d82e3d48a09d0378d91aaca8ca153c3819e7a686`  
		Last Modified: Thu, 03 Mar 2022 02:21:31 GMT  
		Size: 63.8 MB (63816961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88df431ce701ae5994531d21801baa8d60ebb952c1675cee8006761b12e1bb3`  
		Last Modified: Fri, 04 Mar 2022 02:56:21 GMT  
		Size: 423.1 MB (423113867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:2e21218a068141128509da3b5a0352ac9e8941937ad3d9b34b267369d3eed3a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:10b73bf006c43fff1e2e5f25fd23f11d730145f94fc8d9d96a4de417277ef9b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62366933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef7a8ac5b70aa541fef41e309e139ad535a13bc507122369b6c80fc4980ac6a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 26 Feb 2022 02:36:39 GMT
ADD file:e2a9332f7a6ac3bad7b0c1c9cf654d3a7ff3139013c2a2e315d219e7f51b2f0a in / 
# Sat, 26 Feb 2022 02:36:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:243bb3077bc0f28f0b2dd4489a2aeefa4d1a3afad6aa579aa9de653fc5dde576`  
		Last Modified: Sat, 26 Feb 2022 02:38:16 GMT  
		Size: 62.4 MB (62366933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:9b216b739f4bf9f7bec04e31066705dab48f596b5a778374be44f7c1865c3e44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3a51375eb97e43cd90422b3263eba67b348b05325b274901bac64fa2d26afa94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (514978058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:059a456ad03a6cc52fb1459fa5a68d1921ae1c7295f2528e1bca32b1f5eaa9d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 26 Feb 2022 02:36:39 GMT
ADD file:e2a9332f7a6ac3bad7b0c1c9cf654d3a7ff3139013c2a2e315d219e7f51b2f0a in / 
# Sat, 26 Feb 2022 02:36:40 GMT
CMD ["/bin/bash"]
# Sat, 26 Feb 2022 02:37:12 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-61ca3a50468582bc69c53c50f6e1cb49a44054a672c55189905f1aeeab9e866c.tar.gz"  && echo "d8777443388978ad4e7717cf420aadc073caa843bd410bc5ba7410ec73237440  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:243bb3077bc0f28f0b2dd4489a2aeefa4d1a3afad6aa579aa9de653fc5dde576`  
		Last Modified: Sat, 26 Feb 2022 02:38:16 GMT  
		Size: 62.4 MB (62366933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99fdb0ce658bd85cf1e30c481bafab589fe407d7106e82fde2cdd1ceeff0e3e`  
		Last Modified: Sat, 26 Feb 2022 02:38:46 GMT  
		Size: 452.6 MB (452611125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220209.0`

```console
$ docker pull amazonlinux@sha256:2e21218a068141128509da3b5a0352ac9e8941937ad3d9b34b267369d3eed3a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220209.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:10b73bf006c43fff1e2e5f25fd23f11d730145f94fc8d9d96a4de417277ef9b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62366933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef7a8ac5b70aa541fef41e309e139ad535a13bc507122369b6c80fc4980ac6a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 26 Feb 2022 02:36:39 GMT
ADD file:e2a9332f7a6ac3bad7b0c1c9cf654d3a7ff3139013c2a2e315d219e7f51b2f0a in / 
# Sat, 26 Feb 2022 02:36:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:243bb3077bc0f28f0b2dd4489a2aeefa4d1a3afad6aa579aa9de653fc5dde576`  
		Last Modified: Sat, 26 Feb 2022 02:38:16 GMT  
		Size: 62.4 MB (62366933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220209.0-with-sources`

```console
$ docker pull amazonlinux@sha256:9b216b739f4bf9f7bec04e31066705dab48f596b5a778374be44f7c1865c3e44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220209.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3a51375eb97e43cd90422b3263eba67b348b05325b274901bac64fa2d26afa94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (514978058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:059a456ad03a6cc52fb1459fa5a68d1921ae1c7295f2528e1bca32b1f5eaa9d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 26 Feb 2022 02:36:39 GMT
ADD file:e2a9332f7a6ac3bad7b0c1c9cf654d3a7ff3139013c2a2e315d219e7f51b2f0a in / 
# Sat, 26 Feb 2022 02:36:40 GMT
CMD ["/bin/bash"]
# Sat, 26 Feb 2022 02:37:12 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-61ca3a50468582bc69c53c50f6e1cb49a44054a672c55189905f1aeeab9e866c.tar.gz"  && echo "d8777443388978ad4e7717cf420aadc073caa843bd410bc5ba7410ec73237440  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:243bb3077bc0f28f0b2dd4489a2aeefa4d1a3afad6aa579aa9de653fc5dde576`  
		Last Modified: Sat, 26 Feb 2022 02:38:16 GMT  
		Size: 62.4 MB (62366933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99fdb0ce658bd85cf1e30c481bafab589fe407d7106e82fde2cdd1ceeff0e3e`  
		Last Modified: Sat, 26 Feb 2022 02:38:46 GMT  
		Size: 452.6 MB (452611125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:ba535592e8fca7d12c9f6ebe81e1fc69713740287d83c42d83af581a701f6e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:40b0ca43bd05033674743d9107fda51f6c28f54b913b03d6969a729fd97f2c5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67393012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925675097171e3c481c93fc5752fa357012a23c4fc380b600b910f47bfa3e6a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:19:55 GMT
ADD file:a17c7e0c1674512d1358af2a8ecd7d3ab42c3f853ca0d502a0a5ccf61e7cc1ae in / 
# Tue, 08 Feb 2022 19:19:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7bc2af7bb0f9d7bc2dd4e52e139b26d5ec36138f2349163c565b89eb4c5dcc6f`  
		Last Modified: Tue, 08 Feb 2022 19:20:49 GMT  
		Size: 67.4 MB (67393012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:68af4691e62c48340d588b8a3fbe468d7b0c1d8463b3a60cacb6bc22876c4497
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66145238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7cd89050ed8e72dc51c91f0ec7cb56ff8c721e291d30c9f5712450d7744024`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:39:46 GMT
ADD file:0dcd3603971e922307b1605e2f1d589bc5f4c8bc61afc2f0aefa817d58bd6071 in / 
# Tue, 08 Feb 2022 19:39:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6cc7ee6c96e110fb553a963091caccb5d86b21e544eaa942b6c0790d4278c681`  
		Last Modified: Tue, 08 Feb 2022 19:40:48 GMT  
		Size: 66.1 MB (66145238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:fadcb4baca649109a8625d85ea703ae24c8b53da551bc2124d3f5fbc06b547ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9de6068deba3e5af8e83805b27dfc79d1e4728948d781f9eda038e8e84912374
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **473.8 MB (473797024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37cca01d65d7d629d2f44cf3d2ac822fd1fecd185fbf0e00ceaaea97842450c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:39:46 GMT
ADD file:0dcd3603971e922307b1605e2f1d589bc5f4c8bc61afc2f0aefa817d58bd6071 in / 
# Tue, 08 Feb 2022 19:39:47 GMT
CMD ["/bin/bash"]
# Tue, 08 Feb 2022 19:40:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-cc7e5469c58d5d340a4834dfcb1b4f5cd38df8115a8622b945b52156d73005e2.tar.gz"  && echo "356327ddb540b40c52a2a4a6392991c4fb8a6b15c8f6a0bca616a7751d776175  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6cc7ee6c96e110fb553a963091caccb5d86b21e544eaa942b6c0790d4278c681`  
		Last Modified: Tue, 08 Feb 2022 19:40:48 GMT  
		Size: 66.1 MB (66145238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12d51930db801eff88ca3450938771be2dc3af5155289546b3b8c372ecc0506`  
		Last Modified: Tue, 08 Feb 2022 19:41:19 GMT  
		Size: 407.7 MB (407651786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220202.0`

```console
$ docker pull amazonlinux@sha256:ba535592e8fca7d12c9f6ebe81e1fc69713740287d83c42d83af581a701f6e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220202.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:40b0ca43bd05033674743d9107fda51f6c28f54b913b03d6969a729fd97f2c5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67393012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925675097171e3c481c93fc5752fa357012a23c4fc380b600b910f47bfa3e6a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:19:55 GMT
ADD file:a17c7e0c1674512d1358af2a8ecd7d3ab42c3f853ca0d502a0a5ccf61e7cc1ae in / 
# Tue, 08 Feb 2022 19:19:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7bc2af7bb0f9d7bc2dd4e52e139b26d5ec36138f2349163c565b89eb4c5dcc6f`  
		Last Modified: Tue, 08 Feb 2022 19:20:49 GMT  
		Size: 67.4 MB (67393012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220202.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:68af4691e62c48340d588b8a3fbe468d7b0c1d8463b3a60cacb6bc22876c4497
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66145238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7cd89050ed8e72dc51c91f0ec7cb56ff8c721e291d30c9f5712450d7744024`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:39:46 GMT
ADD file:0dcd3603971e922307b1605e2f1d589bc5f4c8bc61afc2f0aefa817d58bd6071 in / 
# Tue, 08 Feb 2022 19:39:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6cc7ee6c96e110fb553a963091caccb5d86b21e544eaa942b6c0790d4278c681`  
		Last Modified: Tue, 08 Feb 2022 19:40:48 GMT  
		Size: 66.1 MB (66145238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220202.0-with-sources`

```console
$ docker pull amazonlinux@sha256:fadcb4baca649109a8625d85ea703ae24c8b53da551bc2124d3f5fbc06b547ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220202.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9de6068deba3e5af8e83805b27dfc79d1e4728948d781f9eda038e8e84912374
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **473.8 MB (473797024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37cca01d65d7d629d2f44cf3d2ac822fd1fecd185fbf0e00ceaaea97842450c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:39:46 GMT
ADD file:0dcd3603971e922307b1605e2f1d589bc5f4c8bc61afc2f0aefa817d58bd6071 in / 
# Tue, 08 Feb 2022 19:39:47 GMT
CMD ["/bin/bash"]
# Tue, 08 Feb 2022 19:40:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-cc7e5469c58d5d340a4834dfcb1b4f5cd38df8115a8622b945b52156d73005e2.tar.gz"  && echo "356327ddb540b40c52a2a4a6392991c4fb8a6b15c8f6a0bca616a7751d776175  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6cc7ee6c96e110fb553a963091caccb5d86b21e544eaa942b6c0790d4278c681`  
		Last Modified: Tue, 08 Feb 2022 19:40:48 GMT  
		Size: 66.1 MB (66145238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12d51930db801eff88ca3450938771be2dc3af5155289546b3b8c372ecc0506`  
		Last Modified: Tue, 08 Feb 2022 19:41:19 GMT  
		Size: 407.7 MB (407651786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:ba535592e8fca7d12c9f6ebe81e1fc69713740287d83c42d83af581a701f6e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:40b0ca43bd05033674743d9107fda51f6c28f54b913b03d6969a729fd97f2c5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67393012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925675097171e3c481c93fc5752fa357012a23c4fc380b600b910f47bfa3e6a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:19:55 GMT
ADD file:a17c7e0c1674512d1358af2a8ecd7d3ab42c3f853ca0d502a0a5ccf61e7cc1ae in / 
# Tue, 08 Feb 2022 19:19:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7bc2af7bb0f9d7bc2dd4e52e139b26d5ec36138f2349163c565b89eb4c5dcc6f`  
		Last Modified: Tue, 08 Feb 2022 19:20:49 GMT  
		Size: 67.4 MB (67393012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:68af4691e62c48340d588b8a3fbe468d7b0c1d8463b3a60cacb6bc22876c4497
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66145238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7cd89050ed8e72dc51c91f0ec7cb56ff8c721e291d30c9f5712450d7744024`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:39:46 GMT
ADD file:0dcd3603971e922307b1605e2f1d589bc5f4c8bc61afc2f0aefa817d58bd6071 in / 
# Tue, 08 Feb 2022 19:39:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6cc7ee6c96e110fb553a963091caccb5d86b21e544eaa942b6c0790d4278c681`  
		Last Modified: Tue, 08 Feb 2022 19:40:48 GMT  
		Size: 66.1 MB (66145238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:fadcb4baca649109a8625d85ea703ae24c8b53da551bc2124d3f5fbc06b547ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9de6068deba3e5af8e83805b27dfc79d1e4728948d781f9eda038e8e84912374
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **473.8 MB (473797024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37cca01d65d7d629d2f44cf3d2ac822fd1fecd185fbf0e00ceaaea97842450c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:39:46 GMT
ADD file:0dcd3603971e922307b1605e2f1d589bc5f4c8bc61afc2f0aefa817d58bd6071 in / 
# Tue, 08 Feb 2022 19:39:47 GMT
CMD ["/bin/bash"]
# Tue, 08 Feb 2022 19:40:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-cc7e5469c58d5d340a4834dfcb1b4f5cd38df8115a8622b945b52156d73005e2.tar.gz"  && echo "356327ddb540b40c52a2a4a6392991c4fb8a6b15c8f6a0bca616a7751d776175  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6cc7ee6c96e110fb553a963091caccb5d86b21e544eaa942b6c0790d4278c681`  
		Last Modified: Tue, 08 Feb 2022 19:40:48 GMT  
		Size: 66.1 MB (66145238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12d51930db801eff88ca3450938771be2dc3af5155289546b3b8c372ecc0506`  
		Last Modified: Tue, 08 Feb 2022 19:41:19 GMT  
		Size: 407.7 MB (407651786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:3807816d350446a722cfc8cf366e163ebf566a52a333d87372b77320a5d7eb4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:a4cfc190f7c549bc8a3f260a8f3af45ddeae63fb10ccad70f914d411aec1e431
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62237845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab2a8d1dc5555599378fc9c5a5661470b0151ed10e3d663a8fbf0b09d6e3d09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9a75e593b5ca191b5ca33df38a76dae3a64ef1c5166a202cd8aa3896c8ebd36e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63816961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70fe3a7e5673d1977cf1600b59c9e91d75769aea7bff0abfd978fe809a9f8c21`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 02:54:31 GMT
ADD file:d8fe7ad66f762a8aad81401877fc5d61f1a4b58eac91f47145e6e443aa3ac8ee in / 
# Fri, 04 Mar 2022 02:54:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:12990ee66856745f12f3a508d82e3d48a09d0378d91aaca8ca153c3819e7a686`  
		Last Modified: Thu, 03 Mar 2022 02:21:31 GMT  
		Size: 63.8 MB (63816961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:c1ee9fc091e36d67cbe79f8acc9c56c133d8a8f0fcfdd327b2ccdab85bd088b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c2f6a88e3f9cb6221b13a2d961456a081975b936580387b6933cfff6e664af9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.4 MB (485371765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8932d75666cadda98036af5cd135cad7a648d26fc9b62458558ca3b2a56a435`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 23:40:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-86059ff059c15219c13900625367028ea52b1d95d6f6515947fe04983baf9add.tar.gz"  && echo "7cbab49134e393024873c4c8ad4937d84c8b7ed316b4d6260ae6b425cdd89e91  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df40d5f106fd4ab71023a3b15de586ad3165bbec356559856b77c24ad4d33883`  
		Last Modified: Fri, 04 Feb 2022 23:42:04 GMT  
		Size: 423.1 MB (423133920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2896d84d7d4d35a3b2107ee151860013ff99c1b84fe61ee1dc6200724c51e84e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.9 MB (486930828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc9dae5a26f2292aff8c56adebc728b2a363264201f58e30e964116af4c4832`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 02:54:31 GMT
ADD file:d8fe7ad66f762a8aad81401877fc5d61f1a4b58eac91f47145e6e443aa3ac8ee in / 
# Fri, 04 Mar 2022 02:54:32 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 02:54:54 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-743baa7c60c3c54741d5e55ae3430a659604633fb03e9616435ba83760e96755.tar.gz"  && echo "a2d893e0aae7d4bbe63bc587b4df87ae9ba7f2de8a15de13e766f74031044843  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:12990ee66856745f12f3a508d82e3d48a09d0378d91aaca8ca153c3819e7a686`  
		Last Modified: Thu, 03 Mar 2022 02:21:31 GMT  
		Size: 63.8 MB (63816961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88df431ce701ae5994531d21801baa8d60ebb952c1675cee8006761b12e1bb3`  
		Last Modified: Fri, 04 Mar 2022 02:56:21 GMT  
		Size: 423.1 MB (423113867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
