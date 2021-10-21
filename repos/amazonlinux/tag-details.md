<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20211005.0`](#amazonlinux20202110050)
-	[`amazonlinux:2.0.20211005.0-with-sources`](#amazonlinux20202110050-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20211001.0`](#amazonlinux2018030202110010)
-	[`amazonlinux:2018.03.0.20211001.0-with-sources`](#amazonlinux2018030202110010-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:cbe3e5bfec3dcbbf4c7a71431c09e02d23a3588dd5c5c3b83db0097843d7347d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:96d25afa5c49546d2711098e71492a6455cd3e30a84499993e695d44012d3bba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f814ccfcfaccf887e5050ce17689dbdacb9c07300c4490c290f11c301e9f6611`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:21:13 GMT
ADD file:858e35d9bdddc1da540b9c96cef665758539c4f98052911debbc4840456b6c3c in / 
# Fri, 01 Oct 2021 21:21:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:42e892c5bc2a48ee03d6c26e4ac8e04b6c00c867c736c85397c9b71cb97c84b6`  
		Last Modified: Fri, 01 Oct 2021 21:23:04 GMT  
		Size: 62.4 MB (62425413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:5e643a9f60f90d2fe2f0cbc272f316dd9f3e76197fa50325456f3187a0d6ca6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7f5b8b41668eaa316790cd331f5b39c7fab066464f04d0f57e53f54570547b93
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515026013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab8476254d46f7b199a6d38d15e0a83ccfc8326b756c3a99398bcfe0e2c6936`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:21:13 GMT
ADD file:858e35d9bdddc1da540b9c96cef665758539c4f98052911debbc4840456b6c3c in / 
# Fri, 01 Oct 2021 21:21:14 GMT
CMD ["/bin/bash"]
# Fri, 01 Oct 2021 21:21:42 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e273657ff7068db879e5243de5bdcf67bd9287fa16221f444ed1973a7085c77c.tar.gz"  && echo "7f5e1f7b4ed6b98122a5ca4e03e6aa30b1cb10e3e7aa5cd7a2a603a3b42f3c17  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:42e892c5bc2a48ee03d6c26e4ac8e04b6c00c867c736c85397c9b71cb97c84b6`  
		Last Modified: Fri, 01 Oct 2021 21:23:04 GMT  
		Size: 62.4 MB (62425413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa3edb9df8bffd61660f8cc726d814397887f54b03789d66a96b7fd9bbf407`  
		Last Modified: Fri, 01 Oct 2021 21:23:34 GMT  
		Size: 452.6 MB (452600600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:1c1548c73cdb64077c6eb073dc2d1e14d37581a75f2e3e02416855416991224f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:28091ca56cd22253c7a5e99cb581dacee6678181208e2a7799d573bf25d51a63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61952638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb66de99acf334abe43a4b0412d569e335c983cc924ab6dff5ceb5bcad911206`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:20:20 GMT
ADD file:21dc1ad70daefae1cf0e1b3e78fab06decda5cb9bc958d8a178adb3eddd1fb32 in / 
# Fri, 01 Oct 2021 21:20:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0728ce74490afacced1ac863ee989913071f97c52ab996e46cdd6b5369a2d63a`  
		Last Modified: Fri, 01 Oct 2021 10:54:14 GMT  
		Size: 62.0 MB (61952638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:cd1e1bf25bfaf6a4eea10910a02f6ecad68f1513e653e94dbc40aee4a063be73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63606878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e714a021005faa1f0ed7d86c5d1a9f01eb0a62dc16534cfae0782ab9441450c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 21:39:54 GMT
ADD file:d9148106dadecc4050f37ebf22ea9e7e56102619349368d1ce40d36f5e2fadd1 in / 
# Thu, 21 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e20b44047a77430ceb5678bf23278ca2841835a1b18a72adaace3d3a11c56031`  
		Last Modified: Thu, 21 Oct 2021 21:40:44 GMT  
		Size: 63.6 MB (63606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:9c60d0b0ed9c145c13877b5394d24504e120dbabd39a8e8be9f6806eb28174b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:166a07247bb683593f03a556aa010d3bc7273439f038eccee9b5cc0c48af3e17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.0 MB (543000923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f894820418645903e9eaf82e16f79a3234546d6984b9778f7a495e4373787ef0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:20:20 GMT
ADD file:21dc1ad70daefae1cf0e1b3e78fab06decda5cb9bc958d8a178adb3eddd1fb32 in / 
# Fri, 01 Oct 2021 21:20:20 GMT
CMD ["/bin/bash"]
# Fri, 01 Oct 2021 21:20:55 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9e2410667f949f30b61e785e22df92d79408ac9eca07635984070dda5b1f62b5.tar.gz"  && echo "38104879f82d48a1d2a52ceb37ad6275a2b26ab7596440d3ace779cc54d440fa  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0728ce74490afacced1ac863ee989913071f97c52ab996e46cdd6b5369a2d63a`  
		Last Modified: Fri, 01 Oct 2021 10:54:14 GMT  
		Size: 62.0 MB (61952638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310d2444e47af71010180a773ce686cc6dd57bc3285799bd0d06dbc6d567f827`  
		Last Modified: Fri, 01 Oct 2021 21:22:42 GMT  
		Size: 481.0 MB (481048285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:3eea61a0e363060aaf6efcc205010405838c6c927ac7335d9e7b719b52396dc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.7 MB (544666863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db7872fae8888e29da6789210a29c489ca95731ea6c681047c511583c9b815f6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 21:39:54 GMT
ADD file:d9148106dadecc4050f37ebf22ea9e7e56102619349368d1ce40d36f5e2fadd1 in / 
# Thu, 21 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
# Thu, 21 Oct 2021 21:40:15 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e9fd3b1031f9a7540f8249e5d30e6439633e1eb09f394919e35ac5017ec18c93.tar.gz"  && echo "08179d9c712a9a7f501377be8ec5e1f7c229343a5bec655c93db62c623831c7c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e20b44047a77430ceb5678bf23278ca2841835a1b18a72adaace3d3a11c56031`  
		Last Modified: Thu, 21 Oct 2021 21:40:44 GMT  
		Size: 63.6 MB (63606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0e87113240ad7af60957d04bccc7fd72a3ba5616639f468473384eb2c7c691`  
		Last Modified: Thu, 21 Oct 2021 21:41:29 GMT  
		Size: 481.1 MB (481059985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20211005.0`

```console
$ docker pull amazonlinux@sha256:62c7242ac429fe4f78098d41211c52576718af9bfebdedb371f700433141f604
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20211005.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:cd1e1bf25bfaf6a4eea10910a02f6ecad68f1513e653e94dbc40aee4a063be73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63606878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e714a021005faa1f0ed7d86c5d1a9f01eb0a62dc16534cfae0782ab9441450c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 21:39:54 GMT
ADD file:d9148106dadecc4050f37ebf22ea9e7e56102619349368d1ce40d36f5e2fadd1 in / 
# Thu, 21 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e20b44047a77430ceb5678bf23278ca2841835a1b18a72adaace3d3a11c56031`  
		Last Modified: Thu, 21 Oct 2021 21:40:44 GMT  
		Size: 63.6 MB (63606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20211005.0-with-sources`

```console
$ docker pull amazonlinux@sha256:15b7771479b7f11ec8a1b60bc3910c997d6bed75b1c3f7c9098b00c0f3e24f02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20211005.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:3eea61a0e363060aaf6efcc205010405838c6c927ac7335d9e7b719b52396dc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.7 MB (544666863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db7872fae8888e29da6789210a29c489ca95731ea6c681047c511583c9b815f6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 21:39:54 GMT
ADD file:d9148106dadecc4050f37ebf22ea9e7e56102619349368d1ce40d36f5e2fadd1 in / 
# Thu, 21 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
# Thu, 21 Oct 2021 21:40:15 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e9fd3b1031f9a7540f8249e5d30e6439633e1eb09f394919e35ac5017ec18c93.tar.gz"  && echo "08179d9c712a9a7f501377be8ec5e1f7c229343a5bec655c93db62c623831c7c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e20b44047a77430ceb5678bf23278ca2841835a1b18a72adaace3d3a11c56031`  
		Last Modified: Thu, 21 Oct 2021 21:40:44 GMT  
		Size: 63.6 MB (63606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0e87113240ad7af60957d04bccc7fd72a3ba5616639f468473384eb2c7c691`  
		Last Modified: Thu, 21 Oct 2021 21:41:29 GMT  
		Size: 481.1 MB (481059985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:cbe3e5bfec3dcbbf4c7a71431c09e02d23a3588dd5c5c3b83db0097843d7347d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:96d25afa5c49546d2711098e71492a6455cd3e30a84499993e695d44012d3bba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f814ccfcfaccf887e5050ce17689dbdacb9c07300c4490c290f11c301e9f6611`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:21:13 GMT
ADD file:858e35d9bdddc1da540b9c96cef665758539c4f98052911debbc4840456b6c3c in / 
# Fri, 01 Oct 2021 21:21:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:42e892c5bc2a48ee03d6c26e4ac8e04b6c00c867c736c85397c9b71cb97c84b6`  
		Last Modified: Fri, 01 Oct 2021 21:23:04 GMT  
		Size: 62.4 MB (62425413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:5e643a9f60f90d2fe2f0cbc272f316dd9f3e76197fa50325456f3187a0d6ca6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7f5b8b41668eaa316790cd331f5b39c7fab066464f04d0f57e53f54570547b93
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515026013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab8476254d46f7b199a6d38d15e0a83ccfc8326b756c3a99398bcfe0e2c6936`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:21:13 GMT
ADD file:858e35d9bdddc1da540b9c96cef665758539c4f98052911debbc4840456b6c3c in / 
# Fri, 01 Oct 2021 21:21:14 GMT
CMD ["/bin/bash"]
# Fri, 01 Oct 2021 21:21:42 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e273657ff7068db879e5243de5bdcf67bd9287fa16221f444ed1973a7085c77c.tar.gz"  && echo "7f5e1f7b4ed6b98122a5ca4e03e6aa30b1cb10e3e7aa5cd7a2a603a3b42f3c17  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:42e892c5bc2a48ee03d6c26e4ac8e04b6c00c867c736c85397c9b71cb97c84b6`  
		Last Modified: Fri, 01 Oct 2021 21:23:04 GMT  
		Size: 62.4 MB (62425413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa3edb9df8bffd61660f8cc726d814397887f54b03789d66a96b7fd9bbf407`  
		Last Modified: Fri, 01 Oct 2021 21:23:34 GMT  
		Size: 452.6 MB (452600600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20211001.0`

```console
$ docker pull amazonlinux@sha256:cbe3e5bfec3dcbbf4c7a71431c09e02d23a3588dd5c5c3b83db0097843d7347d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20211001.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:96d25afa5c49546d2711098e71492a6455cd3e30a84499993e695d44012d3bba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f814ccfcfaccf887e5050ce17689dbdacb9c07300c4490c290f11c301e9f6611`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:21:13 GMT
ADD file:858e35d9bdddc1da540b9c96cef665758539c4f98052911debbc4840456b6c3c in / 
# Fri, 01 Oct 2021 21:21:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:42e892c5bc2a48ee03d6c26e4ac8e04b6c00c867c736c85397c9b71cb97c84b6`  
		Last Modified: Fri, 01 Oct 2021 21:23:04 GMT  
		Size: 62.4 MB (62425413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20211001.0-with-sources`

```console
$ docker pull amazonlinux@sha256:5e643a9f60f90d2fe2f0cbc272f316dd9f3e76197fa50325456f3187a0d6ca6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20211001.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7f5b8b41668eaa316790cd331f5b39c7fab066464f04d0f57e53f54570547b93
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515026013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab8476254d46f7b199a6d38d15e0a83ccfc8326b756c3a99398bcfe0e2c6936`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:21:13 GMT
ADD file:858e35d9bdddc1da540b9c96cef665758539c4f98052911debbc4840456b6c3c in / 
# Fri, 01 Oct 2021 21:21:14 GMT
CMD ["/bin/bash"]
# Fri, 01 Oct 2021 21:21:42 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e273657ff7068db879e5243de5bdcf67bd9287fa16221f444ed1973a7085c77c.tar.gz"  && echo "7f5e1f7b4ed6b98122a5ca4e03e6aa30b1cb10e3e7aa5cd7a2a603a3b42f3c17  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:42e892c5bc2a48ee03d6c26e4ac8e04b6c00c867c736c85397c9b71cb97c84b6`  
		Last Modified: Fri, 01 Oct 2021 21:23:04 GMT  
		Size: 62.4 MB (62425413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa3edb9df8bffd61660f8cc726d814397887f54b03789d66a96b7fd9bbf407`  
		Last Modified: Fri, 01 Oct 2021 21:23:34 GMT  
		Size: 452.6 MB (452600600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:1c1548c73cdb64077c6eb073dc2d1e14d37581a75f2e3e02416855416991224f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:28091ca56cd22253c7a5e99cb581dacee6678181208e2a7799d573bf25d51a63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61952638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb66de99acf334abe43a4b0412d569e335c983cc924ab6dff5ceb5bcad911206`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:20:20 GMT
ADD file:21dc1ad70daefae1cf0e1b3e78fab06decda5cb9bc958d8a178adb3eddd1fb32 in / 
# Fri, 01 Oct 2021 21:20:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0728ce74490afacced1ac863ee989913071f97c52ab996e46cdd6b5369a2d63a`  
		Last Modified: Fri, 01 Oct 2021 10:54:14 GMT  
		Size: 62.0 MB (61952638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:cd1e1bf25bfaf6a4eea10910a02f6ecad68f1513e653e94dbc40aee4a063be73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63606878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e714a021005faa1f0ed7d86c5d1a9f01eb0a62dc16534cfae0782ab9441450c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 21:39:54 GMT
ADD file:d9148106dadecc4050f37ebf22ea9e7e56102619349368d1ce40d36f5e2fadd1 in / 
# Thu, 21 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e20b44047a77430ceb5678bf23278ca2841835a1b18a72adaace3d3a11c56031`  
		Last Modified: Thu, 21 Oct 2021 21:40:44 GMT  
		Size: 63.6 MB (63606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:9c60d0b0ed9c145c13877b5394d24504e120dbabd39a8e8be9f6806eb28174b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:166a07247bb683593f03a556aa010d3bc7273439f038eccee9b5cc0c48af3e17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.0 MB (543000923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f894820418645903e9eaf82e16f79a3234546d6984b9778f7a495e4373787ef0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:20:20 GMT
ADD file:21dc1ad70daefae1cf0e1b3e78fab06decda5cb9bc958d8a178adb3eddd1fb32 in / 
# Fri, 01 Oct 2021 21:20:20 GMT
CMD ["/bin/bash"]
# Fri, 01 Oct 2021 21:20:55 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9e2410667f949f30b61e785e22df92d79408ac9eca07635984070dda5b1f62b5.tar.gz"  && echo "38104879f82d48a1d2a52ceb37ad6275a2b26ab7596440d3ace779cc54d440fa  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0728ce74490afacced1ac863ee989913071f97c52ab996e46cdd6b5369a2d63a`  
		Last Modified: Fri, 01 Oct 2021 10:54:14 GMT  
		Size: 62.0 MB (61952638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310d2444e47af71010180a773ce686cc6dd57bc3285799bd0d06dbc6d567f827`  
		Last Modified: Fri, 01 Oct 2021 21:22:42 GMT  
		Size: 481.0 MB (481048285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:3eea61a0e363060aaf6efcc205010405838c6c927ac7335d9e7b719b52396dc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.7 MB (544666863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db7872fae8888e29da6789210a29c489ca95731ea6c681047c511583c9b815f6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 21:39:54 GMT
ADD file:d9148106dadecc4050f37ebf22ea9e7e56102619349368d1ce40d36f5e2fadd1 in / 
# Thu, 21 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
# Thu, 21 Oct 2021 21:40:15 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e9fd3b1031f9a7540f8249e5d30e6439633e1eb09f394919e35ac5017ec18c93.tar.gz"  && echo "08179d9c712a9a7f501377be8ec5e1f7c229343a5bec655c93db62c623831c7c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e20b44047a77430ceb5678bf23278ca2841835a1b18a72adaace3d3a11c56031`  
		Last Modified: Thu, 21 Oct 2021 21:40:44 GMT  
		Size: 63.6 MB (63606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0e87113240ad7af60957d04bccc7fd72a3ba5616639f468473384eb2c7c691`  
		Last Modified: Thu, 21 Oct 2021 21:41:29 GMT  
		Size: 481.1 MB (481059985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
