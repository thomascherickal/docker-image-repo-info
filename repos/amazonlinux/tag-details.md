<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20220316.0`](#amazonlinux20202203160)
-	[`amazonlinux:2.0.20220316.0-with-sources`](#amazonlinux20202203160-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20220209.0`](#amazonlinux2018030202202090)
-	[`amazonlinux:2018.03.0.20220209.0-with-sources`](#amazonlinux2018030202202090-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20220308.1`](#amazonlinux20220202203081)
-	[`amazonlinux:2022.0.20220308.1-with-sources`](#amazonlinux20220202203081-with-sources)
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
$ docker pull amazonlinux@sha256:ac28662b06b98d9ab5c9c6ad9a7bb8203b0ce8d26dc35f4986a8f56a810bbab6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:cb1abbf3ad67f51bc30a7fef0ddec5d1008907807f95c8bb9e7b30b0dad348bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62239296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6862f029c6f5f62e2f903686d840cdecbbec6554e23b8cc19f0d18ef72e21c42`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 04:17:58 GMT
ADD file:6e25b6e9b3976f8d699ddf69117d5af30565798c52f777c8b4b99e38aca8523f in / 
# Fri, 04 Mar 2022 04:17:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bda57ff2d0d885374555b8bf3f1aaa48d5f044446a24a98acedbef6acc0b727e`  
		Last Modified: Thu, 03 Mar 2022 02:21:35 GMT  
		Size: 62.2 MB (62239296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f3585a47bc028e750f37684bbf67de38d2c5ae102b8742405c4fa2364647863a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63828887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba048c8ea90cafeac8f911ba460a0a6924d8d056a9caf220a8628458a5f6ba77`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:36:59 GMT
ADD file:2b2d809ac07187a252399bb24721c7a295cf5fa71ef4e526ea56bb8d1bf77fd0 in / 
# Fri, 18 Mar 2022 00:37:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:16a64fa775cc87d32953ff0ed81775d6ea6b725a7946b4260298cc1ec4b5b32b`  
		Last Modified: Thu, 17 Mar 2022 02:22:32 GMT  
		Size: 63.8 MB (63828887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:999665d9a2213ea2bf8093cd9cefcc6d7978438730e1a080c8682c801096757f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3567d9d9eeeeac94ddbd2c08b4ebe9c003a415d4adfb30a4c982f3418d425a36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.4 MB (485353196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e954a7af0320b059d91c2fa85155e202c6b2267be94efa101212fa30328abf78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 04:17:58 GMT
ADD file:6e25b6e9b3976f8d699ddf69117d5af30565798c52f777c8b4b99e38aca8523f in / 
# Fri, 04 Mar 2022 04:17:59 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 04:18:26 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-743baa7c60c3c54741d5e55ae3430a659604633fb03e9616435ba83760e96755.tar.gz"  && echo "a2d893e0aae7d4bbe63bc587b4df87ae9ba7f2de8a15de13e766f74031044843  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:bda57ff2d0d885374555b8bf3f1aaa48d5f044446a24a98acedbef6acc0b727e`  
		Last Modified: Thu, 03 Mar 2022 02:21:35 GMT  
		Size: 62.2 MB (62239296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfc84eae14a8f5517f777f3df3cc60ac8cf33a648d677bc33fab552696f8869`  
		Last Modified: Fri, 04 Mar 2022 04:19:56 GMT  
		Size: 423.1 MB (423113900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:eb66bea13e8eb8b6402f2396470190f5201029f1740f7571511d66fdd157dcdd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.0 MB (486950607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2615f7bdf3f4ddc681610c299da2d5c5c1dfb862ccb4e2f3c5ff0558c98ff73f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:36:59 GMT
ADD file:2b2d809ac07187a252399bb24721c7a295cf5fa71ef4e526ea56bb8d1bf77fd0 in / 
# Fri, 18 Mar 2022 00:37:00 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 00:37:23 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-3c9668ec048dfa6db814960c8f21d657525398c311820322e74a0cd5c740a565.tar.gz"  && echo "28f895ddb81eab8d861e7f1adc7c54a47146dc14956644e699d4eb9ead29f515  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:16a64fa775cc87d32953ff0ed81775d6ea6b725a7946b4260298cc1ec4b5b32b`  
		Last Modified: Thu, 17 Mar 2022 02:22:32 GMT  
		Size: 63.8 MB (63828887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd7a9d9c15edb2f1e103b9fc3acb6251a5ee9d252dae649c8d9c61b88973b5`  
		Last Modified: Fri, 18 Mar 2022 00:39:16 GMT  
		Size: 423.1 MB (423121720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220316.0`

```console
$ docker pull amazonlinux@sha256:d134bc41890ec409edd54d188d558a874dee2d9eac420267cdfa2a788151db18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220316.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f3585a47bc028e750f37684bbf67de38d2c5ae102b8742405c4fa2364647863a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63828887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba048c8ea90cafeac8f911ba460a0a6924d8d056a9caf220a8628458a5f6ba77`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:36:59 GMT
ADD file:2b2d809ac07187a252399bb24721c7a295cf5fa71ef4e526ea56bb8d1bf77fd0 in / 
# Fri, 18 Mar 2022 00:37:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:16a64fa775cc87d32953ff0ed81775d6ea6b725a7946b4260298cc1ec4b5b32b`  
		Last Modified: Thu, 17 Mar 2022 02:22:32 GMT  
		Size: 63.8 MB (63828887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220316.0-with-sources`

```console
$ docker pull amazonlinux@sha256:91d76019d6e536ca35374808184636a61287032fb3a468509ba4cd6519ccf54c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220316.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:eb66bea13e8eb8b6402f2396470190f5201029f1740f7571511d66fdd157dcdd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.0 MB (486950607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2615f7bdf3f4ddc681610c299da2d5c5c1dfb862ccb4e2f3c5ff0558c98ff73f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:36:59 GMT
ADD file:2b2d809ac07187a252399bb24721c7a295cf5fa71ef4e526ea56bb8d1bf77fd0 in / 
# Fri, 18 Mar 2022 00:37:00 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 00:37:23 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-3c9668ec048dfa6db814960c8f21d657525398c311820322e74a0cd5c740a565.tar.gz"  && echo "28f895ddb81eab8d861e7f1adc7c54a47146dc14956644e699d4eb9ead29f515  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:16a64fa775cc87d32953ff0ed81775d6ea6b725a7946b4260298cc1ec4b5b32b`  
		Last Modified: Thu, 17 Mar 2022 02:22:32 GMT  
		Size: 63.8 MB (63828887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd7a9d9c15edb2f1e103b9fc3acb6251a5ee9d252dae649c8d9c61b88973b5`  
		Last Modified: Fri, 18 Mar 2022 00:39:16 GMT  
		Size: 423.1 MB (423121720 bytes)  
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
$ docker pull amazonlinux@sha256:f051e1bb1df1df299422bdfc53b5f579c32f18c4941bc51a4055f1db735ff140
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
$ docker pull amazonlinux@sha256:72f24f745e7d92730a1d833c0e2d62a5cf2b34de0c28751361185695a94958b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66181332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f05e07b335cebb522b1bf5d9bc24b6f3c7ce7058ee0d7e24db511662441d01e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:37:34 GMT
ADD file:0a3f467739b6b34c1677c74456d43d60dd73758c7cea9f5299bf964ac83a6f07 in / 
# Fri, 18 Mar 2022 00:37:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8879502b9714388f162c398379c27a6290a8532d379327519640e91d05ac5b15`  
		Last Modified: Fri, 18 Mar 2022 00:39:40 GMT  
		Size: 66.2 MB (66181332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:182ddd498eb7659524a3a6b2d1f4a90d49270c8bdf877d5e9466163072ac70e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9d70c6acb55094f295cb8b5a825f196fdf6e21ccb871820c521f7b451cc85279
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **475.0 MB (475044841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c50a5ed22d2d8eacb5b113a93756909e390d9b515b4c812f7654bdec1aac97`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:19:55 GMT
ADD file:a17c7e0c1674512d1358af2a8ecd7d3ab42c3f853ca0d502a0a5ccf61e7cc1ae in / 
# Tue, 08 Feb 2022 19:19:56 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 04:18:59 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-cc7e5469c58d5d340a4834dfcb1b4f5cd38df8115a8622b945b52156d73005e2.tar.gz"  && echo "356327ddb540b40c52a2a4a6392991c4fb8a6b15c8f6a0bca616a7751d776175  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7bc2af7bb0f9d7bc2dd4e52e139b26d5ec36138f2349163c565b89eb4c5dcc6f`  
		Last Modified: Tue, 08 Feb 2022 19:20:49 GMT  
		Size: 67.4 MB (67393012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ec3e1a9e03dfb694ffaf58eda23ce244264e78f40f7876a54a3c178823663a`  
		Last Modified: Fri, 04 Mar 2022 04:20:27 GMT  
		Size: 407.7 MB (407651829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:efa82a440427284fb42c3bb04f8b6883d1d25256b94825dedc674a5dbd4bf666
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **473.7 MB (473701235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:766f7a9f1488c64f9e231d75c17a96d6c7861535370a772aa719bf6f9d439a06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:37:34 GMT
ADD file:0a3f467739b6b34c1677c74456d43d60dd73758c7cea9f5299bf964ac83a6f07 in / 
# Fri, 18 Mar 2022 00:37:35 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 00:37:58 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-fa0d04ab17f6ae9cb1de39ab5dad52c2e6d9fb369f43679b2f6a0c9e5d12c284.tar.gz"  && echo "35ebd0b74ac0b0422bf72c99f18fd2a38f226202adf6ee9271c52cf2ea7d3df0  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8879502b9714388f162c398379c27a6290a8532d379327519640e91d05ac5b15`  
		Last Modified: Fri, 18 Mar 2022 00:39:40 GMT  
		Size: 66.2 MB (66181332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72833236772f911f636d1b918822c9a8ebd9cd41307464819b9beb9a35f16870`  
		Last Modified: Fri, 18 Mar 2022 00:40:21 GMT  
		Size: 407.5 MB (407519903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220308.1`

```console
$ docker pull amazonlinux@sha256:cae55d1c3e12f594974e61f4d67d28f1ef8c1c27ff00c9bbbac53fa9f406dc02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220308.1` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:72f24f745e7d92730a1d833c0e2d62a5cf2b34de0c28751361185695a94958b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66181332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f05e07b335cebb522b1bf5d9bc24b6f3c7ce7058ee0d7e24db511662441d01e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:37:34 GMT
ADD file:0a3f467739b6b34c1677c74456d43d60dd73758c7cea9f5299bf964ac83a6f07 in / 
# Fri, 18 Mar 2022 00:37:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8879502b9714388f162c398379c27a6290a8532d379327519640e91d05ac5b15`  
		Last Modified: Fri, 18 Mar 2022 00:39:40 GMT  
		Size: 66.2 MB (66181332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220308.1-with-sources`

```console
$ docker pull amazonlinux@sha256:b2dd99d7265fbbb7d8fc44cced2e507d5e3fdb0897207a66ed249015ccc5d1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220308.1-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:efa82a440427284fb42c3bb04f8b6883d1d25256b94825dedc674a5dbd4bf666
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **473.7 MB (473701235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:766f7a9f1488c64f9e231d75c17a96d6c7861535370a772aa719bf6f9d439a06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:37:34 GMT
ADD file:0a3f467739b6b34c1677c74456d43d60dd73758c7cea9f5299bf964ac83a6f07 in / 
# Fri, 18 Mar 2022 00:37:35 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 00:37:58 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-fa0d04ab17f6ae9cb1de39ab5dad52c2e6d9fb369f43679b2f6a0c9e5d12c284.tar.gz"  && echo "35ebd0b74ac0b0422bf72c99f18fd2a38f226202adf6ee9271c52cf2ea7d3df0  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8879502b9714388f162c398379c27a6290a8532d379327519640e91d05ac5b15`  
		Last Modified: Fri, 18 Mar 2022 00:39:40 GMT  
		Size: 66.2 MB (66181332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72833236772f911f636d1b918822c9a8ebd9cd41307464819b9beb9a35f16870`  
		Last Modified: Fri, 18 Mar 2022 00:40:21 GMT  
		Size: 407.5 MB (407519903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:f051e1bb1df1df299422bdfc53b5f579c32f18c4941bc51a4055f1db735ff140
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
$ docker pull amazonlinux@sha256:72f24f745e7d92730a1d833c0e2d62a5cf2b34de0c28751361185695a94958b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66181332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f05e07b335cebb522b1bf5d9bc24b6f3c7ce7058ee0d7e24db511662441d01e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:37:34 GMT
ADD file:0a3f467739b6b34c1677c74456d43d60dd73758c7cea9f5299bf964ac83a6f07 in / 
# Fri, 18 Mar 2022 00:37:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8879502b9714388f162c398379c27a6290a8532d379327519640e91d05ac5b15`  
		Last Modified: Fri, 18 Mar 2022 00:39:40 GMT  
		Size: 66.2 MB (66181332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:182ddd498eb7659524a3a6b2d1f4a90d49270c8bdf877d5e9466163072ac70e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9d70c6acb55094f295cb8b5a825f196fdf6e21ccb871820c521f7b451cc85279
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **475.0 MB (475044841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c50a5ed22d2d8eacb5b113a93756909e390d9b515b4c812f7654bdec1aac97`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:19:55 GMT
ADD file:a17c7e0c1674512d1358af2a8ecd7d3ab42c3f853ca0d502a0a5ccf61e7cc1ae in / 
# Tue, 08 Feb 2022 19:19:56 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 04:18:59 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-cc7e5469c58d5d340a4834dfcb1b4f5cd38df8115a8622b945b52156d73005e2.tar.gz"  && echo "356327ddb540b40c52a2a4a6392991c4fb8a6b15c8f6a0bca616a7751d776175  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7bc2af7bb0f9d7bc2dd4e52e139b26d5ec36138f2349163c565b89eb4c5dcc6f`  
		Last Modified: Tue, 08 Feb 2022 19:20:49 GMT  
		Size: 67.4 MB (67393012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ec3e1a9e03dfb694ffaf58eda23ce244264e78f40f7876a54a3c178823663a`  
		Last Modified: Fri, 04 Mar 2022 04:20:27 GMT  
		Size: 407.7 MB (407651829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:efa82a440427284fb42c3bb04f8b6883d1d25256b94825dedc674a5dbd4bf666
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **473.7 MB (473701235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:766f7a9f1488c64f9e231d75c17a96d6c7861535370a772aa719bf6f9d439a06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:37:34 GMT
ADD file:0a3f467739b6b34c1677c74456d43d60dd73758c7cea9f5299bf964ac83a6f07 in / 
# Fri, 18 Mar 2022 00:37:35 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 00:37:58 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-fa0d04ab17f6ae9cb1de39ab5dad52c2e6d9fb369f43679b2f6a0c9e5d12c284.tar.gz"  && echo "35ebd0b74ac0b0422bf72c99f18fd2a38f226202adf6ee9271c52cf2ea7d3df0  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8879502b9714388f162c398379c27a6290a8532d379327519640e91d05ac5b15`  
		Last Modified: Fri, 18 Mar 2022 00:39:40 GMT  
		Size: 66.2 MB (66181332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72833236772f911f636d1b918822c9a8ebd9cd41307464819b9beb9a35f16870`  
		Last Modified: Fri, 18 Mar 2022 00:40:21 GMT  
		Size: 407.5 MB (407519903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:ac28662b06b98d9ab5c9c6ad9a7bb8203b0ce8d26dc35f4986a8f56a810bbab6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:cb1abbf3ad67f51bc30a7fef0ddec5d1008907807f95c8bb9e7b30b0dad348bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62239296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6862f029c6f5f62e2f903686d840cdecbbec6554e23b8cc19f0d18ef72e21c42`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 04:17:58 GMT
ADD file:6e25b6e9b3976f8d699ddf69117d5af30565798c52f777c8b4b99e38aca8523f in / 
# Fri, 04 Mar 2022 04:17:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bda57ff2d0d885374555b8bf3f1aaa48d5f044446a24a98acedbef6acc0b727e`  
		Last Modified: Thu, 03 Mar 2022 02:21:35 GMT  
		Size: 62.2 MB (62239296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f3585a47bc028e750f37684bbf67de38d2c5ae102b8742405c4fa2364647863a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63828887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba048c8ea90cafeac8f911ba460a0a6924d8d056a9caf220a8628458a5f6ba77`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:36:59 GMT
ADD file:2b2d809ac07187a252399bb24721c7a295cf5fa71ef4e526ea56bb8d1bf77fd0 in / 
# Fri, 18 Mar 2022 00:37:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:16a64fa775cc87d32953ff0ed81775d6ea6b725a7946b4260298cc1ec4b5b32b`  
		Last Modified: Thu, 17 Mar 2022 02:22:32 GMT  
		Size: 63.8 MB (63828887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:999665d9a2213ea2bf8093cd9cefcc6d7978438730e1a080c8682c801096757f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3567d9d9eeeeac94ddbd2c08b4ebe9c003a415d4adfb30a4c982f3418d425a36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.4 MB (485353196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e954a7af0320b059d91c2fa85155e202c6b2267be94efa101212fa30328abf78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 04:17:58 GMT
ADD file:6e25b6e9b3976f8d699ddf69117d5af30565798c52f777c8b4b99e38aca8523f in / 
# Fri, 04 Mar 2022 04:17:59 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 04:18:26 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-743baa7c60c3c54741d5e55ae3430a659604633fb03e9616435ba83760e96755.tar.gz"  && echo "a2d893e0aae7d4bbe63bc587b4df87ae9ba7f2de8a15de13e766f74031044843  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:bda57ff2d0d885374555b8bf3f1aaa48d5f044446a24a98acedbef6acc0b727e`  
		Last Modified: Thu, 03 Mar 2022 02:21:35 GMT  
		Size: 62.2 MB (62239296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfc84eae14a8f5517f777f3df3cc60ac8cf33a648d677bc33fab552696f8869`  
		Last Modified: Fri, 04 Mar 2022 04:19:56 GMT  
		Size: 423.1 MB (423113900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:eb66bea13e8eb8b6402f2396470190f5201029f1740f7571511d66fdd157dcdd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.0 MB (486950607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2615f7bdf3f4ddc681610c299da2d5c5c1dfb862ccb4e2f3c5ff0558c98ff73f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:36:59 GMT
ADD file:2b2d809ac07187a252399bb24721c7a295cf5fa71ef4e526ea56bb8d1bf77fd0 in / 
# Fri, 18 Mar 2022 00:37:00 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 00:37:23 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-3c9668ec048dfa6db814960c8f21d657525398c311820322e74a0cd5c740a565.tar.gz"  && echo "28f895ddb81eab8d861e7f1adc7c54a47146dc14956644e699d4eb9ead29f515  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:16a64fa775cc87d32953ff0ed81775d6ea6b725a7946b4260298cc1ec4b5b32b`  
		Last Modified: Thu, 17 Mar 2022 02:22:32 GMT  
		Size: 63.8 MB (63828887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd7a9d9c15edb2f1e103b9fc3acb6251a5ee9d252dae649c8d9c61b88973b5`  
		Last Modified: Fri, 18 Mar 2022 00:39:16 GMT  
		Size: 423.1 MB (423121720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
