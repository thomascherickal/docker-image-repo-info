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
-	[`amazonlinux:2018.03.0.20211015.1`](#amazonlinux2018030202110151)
-	[`amazonlinux:2018.03.0.20211015.1-with-sources`](#amazonlinux2018030202110151-with-sources)
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
$ docker pull amazonlinux@sha256:05c170879b6dec01ee51dd380d4d63cfb9ba59e738a03531c7ab5923515af3b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:05295e83275444cae0e55601f6a545b548fd3e03e8ef9a4ab9c38a52071519b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61976108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d99c40d6547efd6328851315f5bcf7e6a8e0a96c200583a445fc0cdcd2146b81`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 22:19:45 GMT
ADD file:7aef897e53c30ca977c42dd7692208abbd381b7d2e7e07a91d929f3f0ac4ea5c in / 
# Thu, 21 Oct 2021 22:19:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5263c4cb36ce7acd05658a221ec502b376a281d7a6075ad09beb23ac02a7668c`  
		Last Modified: Wed, 20 Oct 2021 18:03:24 GMT  
		Size: 62.0 MB (61976108 bytes)  
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
$ docker pull amazonlinux@sha256:ee2c1690c911d75f55b7f3b9023e3c78e48eb8b45b504da402b71acd04ab96b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7270588a2f1d44b6515784c67c8887f7ae83def17069edd48910f555d7eda296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.0 MB (543036131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acec5c4453b5b9e508505dc7ed855169c8df9f295df44f0cb767a4fa5d8ee71`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 22:19:45 GMT
ADD file:7aef897e53c30ca977c42dd7692208abbd381b7d2e7e07a91d929f3f0ac4ea5c in / 
# Thu, 21 Oct 2021 22:19:46 GMT
CMD ["/bin/bash"]
# Thu, 21 Oct 2021 22:20:07 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e9fd3b1031f9a7540f8249e5d30e6439633e1eb09f394919e35ac5017ec18c93.tar.gz"  && echo "08179d9c712a9a7f501377be8ec5e1f7c229343a5bec655c93db62c623831c7c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:5263c4cb36ce7acd05658a221ec502b376a281d7a6075ad09beb23ac02a7668c`  
		Last Modified: Wed, 20 Oct 2021 18:03:24 GMT  
		Size: 62.0 MB (61976108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9dd65b340056c10ece74bbe3f53f0a1ec019751a8d9b835573cac406fda501`  
		Last Modified: Thu, 21 Oct 2021 22:21:05 GMT  
		Size: 481.1 MB (481060023 bytes)  
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
$ docker pull amazonlinux@sha256:05c170879b6dec01ee51dd380d4d63cfb9ba59e738a03531c7ab5923515af3b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20211005.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:05295e83275444cae0e55601f6a545b548fd3e03e8ef9a4ab9c38a52071519b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61976108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d99c40d6547efd6328851315f5bcf7e6a8e0a96c200583a445fc0cdcd2146b81`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 22:19:45 GMT
ADD file:7aef897e53c30ca977c42dd7692208abbd381b7d2e7e07a91d929f3f0ac4ea5c in / 
# Thu, 21 Oct 2021 22:19:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5263c4cb36ce7acd05658a221ec502b376a281d7a6075ad09beb23ac02a7668c`  
		Last Modified: Wed, 20 Oct 2021 18:03:24 GMT  
		Size: 62.0 MB (61976108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull amazonlinux@sha256:ee2c1690c911d75f55b7f3b9023e3c78e48eb8b45b504da402b71acd04ab96b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20211005.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7270588a2f1d44b6515784c67c8887f7ae83def17069edd48910f555d7eda296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.0 MB (543036131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acec5c4453b5b9e508505dc7ed855169c8df9f295df44f0cb767a4fa5d8ee71`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 22:19:45 GMT
ADD file:7aef897e53c30ca977c42dd7692208abbd381b7d2e7e07a91d929f3f0ac4ea5c in / 
# Thu, 21 Oct 2021 22:19:46 GMT
CMD ["/bin/bash"]
# Thu, 21 Oct 2021 22:20:07 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e9fd3b1031f9a7540f8249e5d30e6439633e1eb09f394919e35ac5017ec18c93.tar.gz"  && echo "08179d9c712a9a7f501377be8ec5e1f7c229343a5bec655c93db62c623831c7c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:5263c4cb36ce7acd05658a221ec502b376a281d7a6075ad09beb23ac02a7668c`  
		Last Modified: Wed, 20 Oct 2021 18:03:24 GMT  
		Size: 62.0 MB (61976108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9dd65b340056c10ece74bbe3f53f0a1ec019751a8d9b835573cac406fda501`  
		Last Modified: Thu, 21 Oct 2021 22:21:05 GMT  
		Size: 481.1 MB (481060023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `amazonlinux:2018.03.0.20211015.1`

**does not exist** (yet?)

## `amazonlinux:2018.03.0.20211015.1-with-sources`

**does not exist** (yet?)

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:05c170879b6dec01ee51dd380d4d63cfb9ba59e738a03531c7ab5923515af3b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:05295e83275444cae0e55601f6a545b548fd3e03e8ef9a4ab9c38a52071519b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61976108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d99c40d6547efd6328851315f5bcf7e6a8e0a96c200583a445fc0cdcd2146b81`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 22:19:45 GMT
ADD file:7aef897e53c30ca977c42dd7692208abbd381b7d2e7e07a91d929f3f0ac4ea5c in / 
# Thu, 21 Oct 2021 22:19:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5263c4cb36ce7acd05658a221ec502b376a281d7a6075ad09beb23ac02a7668c`  
		Last Modified: Wed, 20 Oct 2021 18:03:24 GMT  
		Size: 62.0 MB (61976108 bytes)  
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
$ docker pull amazonlinux@sha256:ee2c1690c911d75f55b7f3b9023e3c78e48eb8b45b504da402b71acd04ab96b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7270588a2f1d44b6515784c67c8887f7ae83def17069edd48910f555d7eda296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.0 MB (543036131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acec5c4453b5b9e508505dc7ed855169c8df9f295df44f0cb767a4fa5d8ee71`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 22:19:45 GMT
ADD file:7aef897e53c30ca977c42dd7692208abbd381b7d2e7e07a91d929f3f0ac4ea5c in / 
# Thu, 21 Oct 2021 22:19:46 GMT
CMD ["/bin/bash"]
# Thu, 21 Oct 2021 22:20:07 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e9fd3b1031f9a7540f8249e5d30e6439633e1eb09f394919e35ac5017ec18c93.tar.gz"  && echo "08179d9c712a9a7f501377be8ec5e1f7c229343a5bec655c93db62c623831c7c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:5263c4cb36ce7acd05658a221ec502b376a281d7a6075ad09beb23ac02a7668c`  
		Last Modified: Wed, 20 Oct 2021 18:03:24 GMT  
		Size: 62.0 MB (61976108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9dd65b340056c10ece74bbe3f53f0a1ec019751a8d9b835573cac406fda501`  
		Last Modified: Thu, 21 Oct 2021 22:21:05 GMT  
		Size: 481.1 MB (481060023 bytes)  
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
