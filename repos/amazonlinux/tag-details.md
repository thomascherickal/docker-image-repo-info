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
-	[`amazonlinux:2018.03.0.20220315.0`](#amazonlinux2018030202203150)
-	[`amazonlinux:2018.03.0.20220315.0-with-sources`](#amazonlinux2018030202203150-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20220315.0`](#amazonlinux20220202203150)
-	[`amazonlinux:2022.0.20220315.0-with-sources`](#amazonlinux20220202203150-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:6d6d23596b807105d3aa54ceda05fef7f08ab8bcd48cd6bec6f216111c2e26f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6b88dfac47108b50d5f76fe09cfcbcc16c06e1ea8b97c60ff4041f8a3da00282
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62371377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b51c1998f54dfd2111136ee5fb8c322fed50b421aed9c334a3d47028757503`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 19 Mar 2022 00:00:30 GMT
ADD file:0740e257922976a4807eb5e0e8b2137d2187c581e04757bc6396b012c2984877 in / 
# Sat, 19 Mar 2022 00:00:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6a2af4276da118f47f6d59faaf739ac8ad6b76230fe4e9e881f931f89f5fe99d`  
		Last Modified: Sat, 19 Mar 2022 00:01:39 GMT  
		Size: 62.4 MB (62371377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:cab807063eba14c13141f4ca54c68b85b13466402ac0aa3b103fddd9aa71b07e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:61dd738d5d2d0e86bf529be79608e492643297824b2528559b9356b76699b013
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515016086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36c0893271a92f18800485ea04292041280f69c87a1a4c15d98fba808bd1ed14`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 19 Mar 2022 00:00:30 GMT
ADD file:0740e257922976a4807eb5e0e8b2137d2187c581e04757bc6396b012c2984877 in / 
# Sat, 19 Mar 2022 00:00:31 GMT
CMD ["/bin/bash"]
# Sat, 19 Mar 2022 00:00:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1955409f03009ae852836cca134addda0273353334d33438c74060317a23bd38.tar.gz"  && echo "3d9d1fa76eb7d2d554881174fd0f92549d482d99b6f60822dd59173789b14ddc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6a2af4276da118f47f6d59faaf739ac8ad6b76230fe4e9e881f931f89f5fe99d`  
		Last Modified: Sat, 19 Mar 2022 00:01:39 GMT  
		Size: 62.4 MB (62371377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298f23d3684e32a3c17a32933ec4af8f46adeddc4abcf14615c8bb052dedf445`  
		Last Modified: Sat, 19 Mar 2022 00:02:14 GMT  
		Size: 452.6 MB (452644709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:b33b787cdb0e82495d2dc115745f68c7cd8d2585d9d83812fdc183ad39d1b753
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6fa3c5cd2dc7efbe15a2f1d888e8791819023b0d21ae4de3f8014b6b7cf2be10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62205270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aa63ff55c40363d84978d0bd4f41d56d7d4bf4b33a7ea1f30d94b6a0dce6323`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:26:26 GMT
ADD file:4e47205cb284668bcfa38b8efbacd331b3fca78d6893a1ca037e00f6f3612643 in / 
# Fri, 18 Mar 2022 05:26:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:20e1cc2336fb3a7a833ea690a50980a547ab8eaf90797eccd05c4dffe60d7f2a`  
		Last Modified: Wed, 16 Mar 2022 17:46:01 GMT  
		Size: 62.2 MB (62205270 bytes)  
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
$ docker pull amazonlinux@sha256:21693ea27108e5514cd3fce013a53ea08b32e2ad6dd9d3263f38bf9c3bab6e21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:482a94c2fbb091d98d5f458dad127758f4774d6c850386b8e9f637099fa92463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.3 MB (485327027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4553ac9cb419bbc8bf2268c081472d5ef9ae180c2f978ef628deed7ca6fa414`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:26:26 GMT
ADD file:4e47205cb284668bcfa38b8efbacd331b3fca78d6893a1ca037e00f6f3612643 in / 
# Fri, 18 Mar 2022 05:26:27 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 05:26:52 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-3c9668ec048dfa6db814960c8f21d657525398c311820322e74a0cd5c740a565.tar.gz"  && echo "28f895ddb81eab8d861e7f1adc7c54a47146dc14956644e699d4eb9ead29f515  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:20e1cc2336fb3a7a833ea690a50980a547ab8eaf90797eccd05c4dffe60d7f2a`  
		Last Modified: Wed, 16 Mar 2022 17:46:01 GMT  
		Size: 62.2 MB (62205270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a49cb7dc0d9e4a04a4e0043db8324496b140ebf112a0615b6975552ed5e9f9a`  
		Last Modified: Fri, 18 Mar 2022 05:28:47 GMT  
		Size: 423.1 MB (423121757 bytes)  
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
$ docker pull amazonlinux@sha256:b33b787cdb0e82495d2dc115745f68c7cd8d2585d9d83812fdc183ad39d1b753
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220316.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6fa3c5cd2dc7efbe15a2f1d888e8791819023b0d21ae4de3f8014b6b7cf2be10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62205270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aa63ff55c40363d84978d0bd4f41d56d7d4bf4b33a7ea1f30d94b6a0dce6323`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:26:26 GMT
ADD file:4e47205cb284668bcfa38b8efbacd331b3fca78d6893a1ca037e00f6f3612643 in / 
# Fri, 18 Mar 2022 05:26:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:20e1cc2336fb3a7a833ea690a50980a547ab8eaf90797eccd05c4dffe60d7f2a`  
		Last Modified: Wed, 16 Mar 2022 17:46:01 GMT  
		Size: 62.2 MB (62205270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull amazonlinux@sha256:21693ea27108e5514cd3fce013a53ea08b32e2ad6dd9d3263f38bf9c3bab6e21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220316.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:482a94c2fbb091d98d5f458dad127758f4774d6c850386b8e9f637099fa92463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.3 MB (485327027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4553ac9cb419bbc8bf2268c081472d5ef9ae180c2f978ef628deed7ca6fa414`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:26:26 GMT
ADD file:4e47205cb284668bcfa38b8efbacd331b3fca78d6893a1ca037e00f6f3612643 in / 
# Fri, 18 Mar 2022 05:26:27 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 05:26:52 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-3c9668ec048dfa6db814960c8f21d657525398c311820322e74a0cd5c740a565.tar.gz"  && echo "28f895ddb81eab8d861e7f1adc7c54a47146dc14956644e699d4eb9ead29f515  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:20e1cc2336fb3a7a833ea690a50980a547ab8eaf90797eccd05c4dffe60d7f2a`  
		Last Modified: Wed, 16 Mar 2022 17:46:01 GMT  
		Size: 62.2 MB (62205270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a49cb7dc0d9e4a04a4e0043db8324496b140ebf112a0615b6975552ed5e9f9a`  
		Last Modified: Fri, 18 Mar 2022 05:28:47 GMT  
		Size: 423.1 MB (423121757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull amazonlinux@sha256:6d6d23596b807105d3aa54ceda05fef7f08ab8bcd48cd6bec6f216111c2e26f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6b88dfac47108b50d5f76fe09cfcbcc16c06e1ea8b97c60ff4041f8a3da00282
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62371377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b51c1998f54dfd2111136ee5fb8c322fed50b421aed9c334a3d47028757503`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 19 Mar 2022 00:00:30 GMT
ADD file:0740e257922976a4807eb5e0e8b2137d2187c581e04757bc6396b012c2984877 in / 
# Sat, 19 Mar 2022 00:00:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6a2af4276da118f47f6d59faaf739ac8ad6b76230fe4e9e881f931f89f5fe99d`  
		Last Modified: Sat, 19 Mar 2022 00:01:39 GMT  
		Size: 62.4 MB (62371377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:cab807063eba14c13141f4ca54c68b85b13466402ac0aa3b103fddd9aa71b07e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:61dd738d5d2d0e86bf529be79608e492643297824b2528559b9356b76699b013
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515016086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36c0893271a92f18800485ea04292041280f69c87a1a4c15d98fba808bd1ed14`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 19 Mar 2022 00:00:30 GMT
ADD file:0740e257922976a4807eb5e0e8b2137d2187c581e04757bc6396b012c2984877 in / 
# Sat, 19 Mar 2022 00:00:31 GMT
CMD ["/bin/bash"]
# Sat, 19 Mar 2022 00:00:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1955409f03009ae852836cca134addda0273353334d33438c74060317a23bd38.tar.gz"  && echo "3d9d1fa76eb7d2d554881174fd0f92549d482d99b6f60822dd59173789b14ddc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6a2af4276da118f47f6d59faaf739ac8ad6b76230fe4e9e881f931f89f5fe99d`  
		Last Modified: Sat, 19 Mar 2022 00:01:39 GMT  
		Size: 62.4 MB (62371377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298f23d3684e32a3c17a32933ec4af8f46adeddc4abcf14615c8bb052dedf445`  
		Last Modified: Sat, 19 Mar 2022 00:02:14 GMT  
		Size: 452.6 MB (452644709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220315.0`

```console
$ docker pull amazonlinux@sha256:6d6d23596b807105d3aa54ceda05fef7f08ab8bcd48cd6bec6f216111c2e26f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220315.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6b88dfac47108b50d5f76fe09cfcbcc16c06e1ea8b97c60ff4041f8a3da00282
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62371377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b51c1998f54dfd2111136ee5fb8c322fed50b421aed9c334a3d47028757503`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 19 Mar 2022 00:00:30 GMT
ADD file:0740e257922976a4807eb5e0e8b2137d2187c581e04757bc6396b012c2984877 in / 
# Sat, 19 Mar 2022 00:00:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6a2af4276da118f47f6d59faaf739ac8ad6b76230fe4e9e881f931f89f5fe99d`  
		Last Modified: Sat, 19 Mar 2022 00:01:39 GMT  
		Size: 62.4 MB (62371377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220315.0-with-sources`

```console
$ docker pull amazonlinux@sha256:cab807063eba14c13141f4ca54c68b85b13466402ac0aa3b103fddd9aa71b07e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220315.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:61dd738d5d2d0e86bf529be79608e492643297824b2528559b9356b76699b013
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515016086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36c0893271a92f18800485ea04292041280f69c87a1a4c15d98fba808bd1ed14`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 19 Mar 2022 00:00:30 GMT
ADD file:0740e257922976a4807eb5e0e8b2137d2187c581e04757bc6396b012c2984877 in / 
# Sat, 19 Mar 2022 00:00:31 GMT
CMD ["/bin/bash"]
# Sat, 19 Mar 2022 00:00:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1955409f03009ae852836cca134addda0273353334d33438c74060317a23bd38.tar.gz"  && echo "3d9d1fa76eb7d2d554881174fd0f92549d482d99b6f60822dd59173789b14ddc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6a2af4276da118f47f6d59faaf739ac8ad6b76230fe4e9e881f931f89f5fe99d`  
		Last Modified: Sat, 19 Mar 2022 00:01:39 GMT  
		Size: 62.4 MB (62371377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298f23d3684e32a3c17a32933ec4af8f46adeddc4abcf14615c8bb052dedf445`  
		Last Modified: Sat, 19 Mar 2022 00:02:14 GMT  
		Size: 452.6 MB (452644709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:b43e6145a7c17c628533cf743fe1555eb0766f91067ba13546d32fb832dd0a85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c74e77c670519cd69e3f5ce3fa714c02c582a40d786dd7e97113e717e7655e4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70551902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:596c538642b7e6e4555a5995097d5b9d754a024d98026531b8b8398ffd920296`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 22:06:49 GMT
ADD file:0e00ccd2daf7fcbf2c4b6c87fc4c7426cb4744220d4688380b712b0a10b1ce17 in / 
# Wed, 30 Mar 2022 22:06:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:51621d34d545ca53a75f5f765d89feed132eed23e837845dab564cd60d3c4a8d`  
		Last Modified: Wed, 30 Mar 2022 22:07:49 GMT  
		Size: 70.6 MB (70551902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:dde8762c9c365a36934cb4f000ed611c19e52b8c5e32ea0d51a4672029ecdbf8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69106021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afd7915f681cff0714f53daa5fdacc9983b5e0e06b2c0bac438e6421724843c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 18:25:19 GMT
ADD file:b4343bb7616f343b9a7343c7512a69010bd7f36e2c2e218e0eea2f57382746cf in / 
# Wed, 30 Mar 2022 18:25:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1539c116c8b0d4e18a17732583c333362ac930b6eb4be2833fff8a8ab2ea6b8b`  
		Last Modified: Wed, 30 Mar 2022 18:26:53 GMT  
		Size: 69.1 MB (69106021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:c7b999c4dafbef559f121d77f919a775db13ddcea68a31d846b4d3e9ef317469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2fb367b85dcc2797239921217f62d98c66b4e614609ae8130d85ea12fa2be3cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.1 MB (489146951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8572b53c2976082cbb5f61cdd5677e4d8f173f835f7f46f692f85743b824f0c1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 22:06:49 GMT
ADD file:0e00ccd2daf7fcbf2c4b6c87fc4c7426cb4744220d4688380b712b0a10b1ce17 in / 
# Wed, 30 Mar 2022 22:06:49 GMT
CMD ["/bin/bash"]
# Wed, 30 Mar 2022 22:07:13 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-feddddadaa0ca95e9807903d234b2e9192782e81abe4ae95c969d9acf5d1a223.tar.gz"  && echo "a2450fe78ed3b89a144721743a282fcb5041783247ae040872007c08d36a83e1  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:51621d34d545ca53a75f5f765d89feed132eed23e837845dab564cd60d3c4a8d`  
		Last Modified: Wed, 30 Mar 2022 22:07:49 GMT  
		Size: 70.6 MB (70551902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4592a6a3eb2786610fec5f2359858c714b4968d2e854cde2a0adedbc33b2cf`  
		Last Modified: Wed, 30 Mar 2022 22:08:17 GMT  
		Size: 418.6 MB (418595049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:e2dd86254b03868c5c0566669f828081a230149217b93dedce7902ae792d910f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.7 MB (487701029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15709e43976d58175cbdcb7b62bb8d5a6a1b1618c7ba82580e570e92909e68`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 18:25:19 GMT
ADD file:b4343bb7616f343b9a7343c7512a69010bd7f36e2c2e218e0eea2f57382746cf in / 
# Wed, 30 Mar 2022 18:25:20 GMT
CMD ["/bin/bash"]
# Wed, 30 Mar 2022 18:26:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-feddddadaa0ca95e9807903d234b2e9192782e81abe4ae95c969d9acf5d1a223.tar.gz"  && echo "a2450fe78ed3b89a144721743a282fcb5041783247ae040872007c08d36a83e1  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:1539c116c8b0d4e18a17732583c333362ac930b6eb4be2833fff8a8ab2ea6b8b`  
		Last Modified: Wed, 30 Mar 2022 18:26:53 GMT  
		Size: 69.1 MB (69106021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51ff1c75bc99c531f890a7b86060bf09ced222193f634e9f1b029ae55afb22c`  
		Last Modified: Wed, 30 Mar 2022 18:27:28 GMT  
		Size: 418.6 MB (418595008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220315.0`

```console
$ docker pull amazonlinux@sha256:b43e6145a7c17c628533cf743fe1555eb0766f91067ba13546d32fb832dd0a85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220315.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c74e77c670519cd69e3f5ce3fa714c02c582a40d786dd7e97113e717e7655e4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70551902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:596c538642b7e6e4555a5995097d5b9d754a024d98026531b8b8398ffd920296`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 22:06:49 GMT
ADD file:0e00ccd2daf7fcbf2c4b6c87fc4c7426cb4744220d4688380b712b0a10b1ce17 in / 
# Wed, 30 Mar 2022 22:06:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:51621d34d545ca53a75f5f765d89feed132eed23e837845dab564cd60d3c4a8d`  
		Last Modified: Wed, 30 Mar 2022 22:07:49 GMT  
		Size: 70.6 MB (70551902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220315.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:dde8762c9c365a36934cb4f000ed611c19e52b8c5e32ea0d51a4672029ecdbf8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69106021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afd7915f681cff0714f53daa5fdacc9983b5e0e06b2c0bac438e6421724843c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 18:25:19 GMT
ADD file:b4343bb7616f343b9a7343c7512a69010bd7f36e2c2e218e0eea2f57382746cf in / 
# Wed, 30 Mar 2022 18:25:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1539c116c8b0d4e18a17732583c333362ac930b6eb4be2833fff8a8ab2ea6b8b`  
		Last Modified: Wed, 30 Mar 2022 18:26:53 GMT  
		Size: 69.1 MB (69106021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220315.0-with-sources`

```console
$ docker pull amazonlinux@sha256:c7b999c4dafbef559f121d77f919a775db13ddcea68a31d846b4d3e9ef317469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220315.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2fb367b85dcc2797239921217f62d98c66b4e614609ae8130d85ea12fa2be3cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.1 MB (489146951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8572b53c2976082cbb5f61cdd5677e4d8f173f835f7f46f692f85743b824f0c1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 22:06:49 GMT
ADD file:0e00ccd2daf7fcbf2c4b6c87fc4c7426cb4744220d4688380b712b0a10b1ce17 in / 
# Wed, 30 Mar 2022 22:06:49 GMT
CMD ["/bin/bash"]
# Wed, 30 Mar 2022 22:07:13 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-feddddadaa0ca95e9807903d234b2e9192782e81abe4ae95c969d9acf5d1a223.tar.gz"  && echo "a2450fe78ed3b89a144721743a282fcb5041783247ae040872007c08d36a83e1  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:51621d34d545ca53a75f5f765d89feed132eed23e837845dab564cd60d3c4a8d`  
		Last Modified: Wed, 30 Mar 2022 22:07:49 GMT  
		Size: 70.6 MB (70551902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4592a6a3eb2786610fec5f2359858c714b4968d2e854cde2a0adedbc33b2cf`  
		Last Modified: Wed, 30 Mar 2022 22:08:17 GMT  
		Size: 418.6 MB (418595049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220315.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:e2dd86254b03868c5c0566669f828081a230149217b93dedce7902ae792d910f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.7 MB (487701029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15709e43976d58175cbdcb7b62bb8d5a6a1b1618c7ba82580e570e92909e68`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 18:25:19 GMT
ADD file:b4343bb7616f343b9a7343c7512a69010bd7f36e2c2e218e0eea2f57382746cf in / 
# Wed, 30 Mar 2022 18:25:20 GMT
CMD ["/bin/bash"]
# Wed, 30 Mar 2022 18:26:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-feddddadaa0ca95e9807903d234b2e9192782e81abe4ae95c969d9acf5d1a223.tar.gz"  && echo "a2450fe78ed3b89a144721743a282fcb5041783247ae040872007c08d36a83e1  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:1539c116c8b0d4e18a17732583c333362ac930b6eb4be2833fff8a8ab2ea6b8b`  
		Last Modified: Wed, 30 Mar 2022 18:26:53 GMT  
		Size: 69.1 MB (69106021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51ff1c75bc99c531f890a7b86060bf09ced222193f634e9f1b029ae55afb22c`  
		Last Modified: Wed, 30 Mar 2022 18:27:28 GMT  
		Size: 418.6 MB (418595008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:b43e6145a7c17c628533cf743fe1555eb0766f91067ba13546d32fb832dd0a85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c74e77c670519cd69e3f5ce3fa714c02c582a40d786dd7e97113e717e7655e4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70551902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:596c538642b7e6e4555a5995097d5b9d754a024d98026531b8b8398ffd920296`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 22:06:49 GMT
ADD file:0e00ccd2daf7fcbf2c4b6c87fc4c7426cb4744220d4688380b712b0a10b1ce17 in / 
# Wed, 30 Mar 2022 22:06:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:51621d34d545ca53a75f5f765d89feed132eed23e837845dab564cd60d3c4a8d`  
		Last Modified: Wed, 30 Mar 2022 22:07:49 GMT  
		Size: 70.6 MB (70551902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:dde8762c9c365a36934cb4f000ed611c19e52b8c5e32ea0d51a4672029ecdbf8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69106021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afd7915f681cff0714f53daa5fdacc9983b5e0e06b2c0bac438e6421724843c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 18:25:19 GMT
ADD file:b4343bb7616f343b9a7343c7512a69010bd7f36e2c2e218e0eea2f57382746cf in / 
# Wed, 30 Mar 2022 18:25:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1539c116c8b0d4e18a17732583c333362ac930b6eb4be2833fff8a8ab2ea6b8b`  
		Last Modified: Wed, 30 Mar 2022 18:26:53 GMT  
		Size: 69.1 MB (69106021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:c7b999c4dafbef559f121d77f919a775db13ddcea68a31d846b4d3e9ef317469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2fb367b85dcc2797239921217f62d98c66b4e614609ae8130d85ea12fa2be3cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.1 MB (489146951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8572b53c2976082cbb5f61cdd5677e4d8f173f835f7f46f692f85743b824f0c1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 22:06:49 GMT
ADD file:0e00ccd2daf7fcbf2c4b6c87fc4c7426cb4744220d4688380b712b0a10b1ce17 in / 
# Wed, 30 Mar 2022 22:06:49 GMT
CMD ["/bin/bash"]
# Wed, 30 Mar 2022 22:07:13 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-feddddadaa0ca95e9807903d234b2e9192782e81abe4ae95c969d9acf5d1a223.tar.gz"  && echo "a2450fe78ed3b89a144721743a282fcb5041783247ae040872007c08d36a83e1  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:51621d34d545ca53a75f5f765d89feed132eed23e837845dab564cd60d3c4a8d`  
		Last Modified: Wed, 30 Mar 2022 22:07:49 GMT  
		Size: 70.6 MB (70551902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4592a6a3eb2786610fec5f2359858c714b4968d2e854cde2a0adedbc33b2cf`  
		Last Modified: Wed, 30 Mar 2022 22:08:17 GMT  
		Size: 418.6 MB (418595049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:e2dd86254b03868c5c0566669f828081a230149217b93dedce7902ae792d910f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.7 MB (487701029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15709e43976d58175cbdcb7b62bb8d5a6a1b1618c7ba82580e570e92909e68`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 18:25:19 GMT
ADD file:b4343bb7616f343b9a7343c7512a69010bd7f36e2c2e218e0eea2f57382746cf in / 
# Wed, 30 Mar 2022 18:25:20 GMT
CMD ["/bin/bash"]
# Wed, 30 Mar 2022 18:26:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-feddddadaa0ca95e9807903d234b2e9192782e81abe4ae95c969d9acf5d1a223.tar.gz"  && echo "a2450fe78ed3b89a144721743a282fcb5041783247ae040872007c08d36a83e1  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:1539c116c8b0d4e18a17732583c333362ac930b6eb4be2833fff8a8ab2ea6b8b`  
		Last Modified: Wed, 30 Mar 2022 18:26:53 GMT  
		Size: 69.1 MB (69106021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51ff1c75bc99c531f890a7b86060bf09ced222193f634e9f1b029ae55afb22c`  
		Last Modified: Wed, 30 Mar 2022 18:27:28 GMT  
		Size: 418.6 MB (418595008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:b33b787cdb0e82495d2dc115745f68c7cd8d2585d9d83812fdc183ad39d1b753
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6fa3c5cd2dc7efbe15a2f1d888e8791819023b0d21ae4de3f8014b6b7cf2be10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62205270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aa63ff55c40363d84978d0bd4f41d56d7d4bf4b33a7ea1f30d94b6a0dce6323`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:26:26 GMT
ADD file:4e47205cb284668bcfa38b8efbacd331b3fca78d6893a1ca037e00f6f3612643 in / 
# Fri, 18 Mar 2022 05:26:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:20e1cc2336fb3a7a833ea690a50980a547ab8eaf90797eccd05c4dffe60d7f2a`  
		Last Modified: Wed, 16 Mar 2022 17:46:01 GMT  
		Size: 62.2 MB (62205270 bytes)  
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
$ docker pull amazonlinux@sha256:21693ea27108e5514cd3fce013a53ea08b32e2ad6dd9d3263f38bf9c3bab6e21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:482a94c2fbb091d98d5f458dad127758f4774d6c850386b8e9f637099fa92463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.3 MB (485327027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4553ac9cb419bbc8bf2268c081472d5ef9ae180c2f978ef628deed7ca6fa414`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:26:26 GMT
ADD file:4e47205cb284668bcfa38b8efbacd331b3fca78d6893a1ca037e00f6f3612643 in / 
# Fri, 18 Mar 2022 05:26:27 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 05:26:52 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-3c9668ec048dfa6db814960c8f21d657525398c311820322e74a0cd5c740a565.tar.gz"  && echo "28f895ddb81eab8d861e7f1adc7c54a47146dc14956644e699d4eb9ead29f515  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:20e1cc2336fb3a7a833ea690a50980a547ab8eaf90797eccd05c4dffe60d7f2a`  
		Last Modified: Wed, 16 Mar 2022 17:46:01 GMT  
		Size: 62.2 MB (62205270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a49cb7dc0d9e4a04a4e0043db8324496b140ebf112a0615b6975552ed5e9f9a`  
		Last Modified: Fri, 18 Mar 2022 05:28:47 GMT  
		Size: 423.1 MB (423121757 bytes)  
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
