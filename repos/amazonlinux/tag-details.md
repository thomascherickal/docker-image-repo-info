<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20211223.0`](#amazonlinux20202112230)
-	[`amazonlinux:2.0.20211223.0-with-sources`](#amazonlinux20202112230-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20220119.1`](#amazonlinux2018030202201191)
-	[`amazonlinux:2018.03.0.20220119.1-with-sources`](#amazonlinux2018030202201191-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:07602b51b89bd986c01777ebf06af227541337c0483395cc550e14c1cb0204ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9739ed1453449dac5824684cb1189478978dece8ac856560f96c55101a57710a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62408287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7cbfc406b7ed062fb9c08cfcad0a8dc85028c1420e7a3bf65c9bd0f083f796`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:40 GMT
ADD file:b40f5b5df3c73d89ec477953753f29f16b9ebd38006d73c41b1468302e274d6f in / 
# Thu, 02 Dec 2021 23:20:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6ce5a5560ab28234e783487f84e4b59ecf9cdd051947c044d6b557746ded7630`  
		Last Modified: Thu, 02 Dec 2021 23:22:29 GMT  
		Size: 62.4 MB (62408287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:d4d921a4a191944d7e028f22efa418f978ae39d9b6d451b6d19f8fc1cdbaeab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:da16df68ae7f6ce6fad4123e255ba51d0917030f796e1ef4086a3deaf51e8101
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515029612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa111552ce92b077f0e226fd14d250252ec4643eead06a1010743c65016ee472`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:40 GMT
ADD file:b40f5b5df3c73d89ec477953753f29f16b9ebd38006d73c41b1468302e274d6f in / 
# Thu, 02 Dec 2021 23:20:40 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 23:21:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d9420f93e86b4ae7e03c24f0e4f98c3c9ea9a63b39646e47c86b1dbadc8bdec5.tar.gz"  && echo "c30aa8fe6299b9787f1287c9b7508bad1f31a056d26cf106d87670b6fe99c16f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6ce5a5560ab28234e783487f84e4b59ecf9cdd051947c044d6b557746ded7630`  
		Last Modified: Thu, 02 Dec 2021 23:22:29 GMT  
		Size: 62.4 MB (62408287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309de403a6353bf47267c55cbbfd3ce20772653b054e31dd83b30bc40380451e`  
		Last Modified: Thu, 02 Dec 2021 23:22:59 GMT  
		Size: 452.6 MB (452621325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:ffc013f79b36a2c0352b444f5322ff43de25152a8ac1ad0fa473e90f1cbedcbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9c4e7b374a7a9253764876520d867ba1f5bfddeed82b029b5054cce0f71faf20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62212074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30156a0e4f040d255f30a8bf0b28540fce965398fe1c13ab29a7292e411dfde7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:20:04 GMT
ADD file:618cac8c5b6f6ff56ce221df12002d34997bcc996a0af3200b58db07d68be275 in / 
# Wed, 12 Jan 2022 02:20:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3a461b3ae562f8b6cf015b4c480a21b630a874f7fec851457680159226c81632`  
		Last Modified: Mon, 10 Jan 2022 23:29:44 GMT  
		Size: 62.2 MB (62212074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:b072eb708b1a43ebfab7745a2ed7e189722632c774efddcc03c963b0b69e6d5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63836908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:377da0386f50f197de2aef131c3df2a761d075a487cf6bbc4338ccf2916c24fe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:39:41 GMT
ADD file:afc90ca87d61fdaef5c9d192a5151ab745ac8b8ea4d7544c2dfdd66bdb3b7993 in / 
# Wed, 12 Jan 2022 02:39:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b2e274b2b0f90c3d6329566163244a0f2e6d97e4c010c62133388ac89652105f`  
		Last Modified: Wed, 12 Jan 2022 02:41:56 GMT  
		Size: 63.8 MB (63836908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:88401a082ea5ed7c7f52bae11a93ac1b21e6be238e1e015c8d1125c81eb025ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c09b199271ac2123d756575757bd922c47ce5a694f9db2918d60b8e091875875
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.2 MB (485180055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369eae5a9f20304404ae63efff50e98c2b4a2180a939d85b710cffcb8a1640c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:20:04 GMT
ADD file:618cac8c5b6f6ff56ce221df12002d34997bcc996a0af3200b58db07d68be275 in / 
# Wed, 12 Jan 2022 02:20:04 GMT
CMD ["/bin/bash"]
# Wed, 12 Jan 2022 02:23:00 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7aacabcecad2264904d2033d4072bf9e9b01b2723fb3de24f8df40bdfc2d34f7.tar.gz"  && echo "eba78093a05bb779050f6f4b93732638f4e1c21fb83c321416e0756efa88a089  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3a461b3ae562f8b6cf015b4c480a21b630a874f7fec851457680159226c81632`  
		Last Modified: Mon, 10 Jan 2022 23:29:44 GMT  
		Size: 62.2 MB (62212074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f95733a61d793aea825bb1d8d9524d99118ee03b09038bff8da69f10cc6cd8`  
		Last Modified: Wed, 12 Jan 2022 02:24:10 GMT  
		Size: 423.0 MB (422967981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ad5d2555741764f400b006e21873f1d966bef7a06905709b08d884ca5046dc82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.8 MB (486804859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69dcd260e7799a7e5ad30046fd6a56a731b92f7603c7eadff3195f6a9f5ae419`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:39:41 GMT
ADD file:afc90ca87d61fdaef5c9d192a5151ab745ac8b8ea4d7544c2dfdd66bdb3b7993 in / 
# Wed, 12 Jan 2022 02:39:43 GMT
CMD ["/bin/bash"]
# Wed, 12 Jan 2022 02:41:20 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7aacabcecad2264904d2033d4072bf9e9b01b2723fb3de24f8df40bdfc2d34f7.tar.gz"  && echo "eba78093a05bb779050f6f4b93732638f4e1c21fb83c321416e0756efa88a089  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:b2e274b2b0f90c3d6329566163244a0f2e6d97e4c010c62133388ac89652105f`  
		Last Modified: Wed, 12 Jan 2022 02:41:56 GMT  
		Size: 63.8 MB (63836908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f335cb87be6e36244e570c6194cee7b36f34f1af6d0f2c4a2c61430b67b7071`  
		Last Modified: Wed, 12 Jan 2022 02:42:43 GMT  
		Size: 423.0 MB (422967951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20211223.0`

```console
$ docker pull amazonlinux@sha256:ffc013f79b36a2c0352b444f5322ff43de25152a8ac1ad0fa473e90f1cbedcbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20211223.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9c4e7b374a7a9253764876520d867ba1f5bfddeed82b029b5054cce0f71faf20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62212074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30156a0e4f040d255f30a8bf0b28540fce965398fe1c13ab29a7292e411dfde7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:20:04 GMT
ADD file:618cac8c5b6f6ff56ce221df12002d34997bcc996a0af3200b58db07d68be275 in / 
# Wed, 12 Jan 2022 02:20:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3a461b3ae562f8b6cf015b4c480a21b630a874f7fec851457680159226c81632`  
		Last Modified: Mon, 10 Jan 2022 23:29:44 GMT  
		Size: 62.2 MB (62212074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20211223.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:b072eb708b1a43ebfab7745a2ed7e189722632c774efddcc03c963b0b69e6d5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63836908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:377da0386f50f197de2aef131c3df2a761d075a487cf6bbc4338ccf2916c24fe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:39:41 GMT
ADD file:afc90ca87d61fdaef5c9d192a5151ab745ac8b8ea4d7544c2dfdd66bdb3b7993 in / 
# Wed, 12 Jan 2022 02:39:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b2e274b2b0f90c3d6329566163244a0f2e6d97e4c010c62133388ac89652105f`  
		Last Modified: Wed, 12 Jan 2022 02:41:56 GMT  
		Size: 63.8 MB (63836908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20211223.0-with-sources`

```console
$ docker pull amazonlinux@sha256:88401a082ea5ed7c7f52bae11a93ac1b21e6be238e1e015c8d1125c81eb025ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20211223.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c09b199271ac2123d756575757bd922c47ce5a694f9db2918d60b8e091875875
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.2 MB (485180055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369eae5a9f20304404ae63efff50e98c2b4a2180a939d85b710cffcb8a1640c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:20:04 GMT
ADD file:618cac8c5b6f6ff56ce221df12002d34997bcc996a0af3200b58db07d68be275 in / 
# Wed, 12 Jan 2022 02:20:04 GMT
CMD ["/bin/bash"]
# Wed, 12 Jan 2022 02:23:00 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7aacabcecad2264904d2033d4072bf9e9b01b2723fb3de24f8df40bdfc2d34f7.tar.gz"  && echo "eba78093a05bb779050f6f4b93732638f4e1c21fb83c321416e0756efa88a089  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3a461b3ae562f8b6cf015b4c480a21b630a874f7fec851457680159226c81632`  
		Last Modified: Mon, 10 Jan 2022 23:29:44 GMT  
		Size: 62.2 MB (62212074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f95733a61d793aea825bb1d8d9524d99118ee03b09038bff8da69f10cc6cd8`  
		Last Modified: Wed, 12 Jan 2022 02:24:10 GMT  
		Size: 423.0 MB (422967981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20211223.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ad5d2555741764f400b006e21873f1d966bef7a06905709b08d884ca5046dc82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.8 MB (486804859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69dcd260e7799a7e5ad30046fd6a56a731b92f7603c7eadff3195f6a9f5ae419`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:39:41 GMT
ADD file:afc90ca87d61fdaef5c9d192a5151ab745ac8b8ea4d7544c2dfdd66bdb3b7993 in / 
# Wed, 12 Jan 2022 02:39:43 GMT
CMD ["/bin/bash"]
# Wed, 12 Jan 2022 02:41:20 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7aacabcecad2264904d2033d4072bf9e9b01b2723fb3de24f8df40bdfc2d34f7.tar.gz"  && echo "eba78093a05bb779050f6f4b93732638f4e1c21fb83c321416e0756efa88a089  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:b2e274b2b0f90c3d6329566163244a0f2e6d97e4c010c62133388ac89652105f`  
		Last Modified: Wed, 12 Jan 2022 02:41:56 GMT  
		Size: 63.8 MB (63836908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f335cb87be6e36244e570c6194cee7b36f34f1af6d0f2c4a2c61430b67b7071`  
		Last Modified: Wed, 12 Jan 2022 02:42:43 GMT  
		Size: 423.0 MB (422967951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:07602b51b89bd986c01777ebf06af227541337c0483395cc550e14c1cb0204ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9739ed1453449dac5824684cb1189478978dece8ac856560f96c55101a57710a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62408287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7cbfc406b7ed062fb9c08cfcad0a8dc85028c1420e7a3bf65c9bd0f083f796`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:40 GMT
ADD file:b40f5b5df3c73d89ec477953753f29f16b9ebd38006d73c41b1468302e274d6f in / 
# Thu, 02 Dec 2021 23:20:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6ce5a5560ab28234e783487f84e4b59ecf9cdd051947c044d6b557746ded7630`  
		Last Modified: Thu, 02 Dec 2021 23:22:29 GMT  
		Size: 62.4 MB (62408287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:d4d921a4a191944d7e028f22efa418f978ae39d9b6d451b6d19f8fc1cdbaeab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:da16df68ae7f6ce6fad4123e255ba51d0917030f796e1ef4086a3deaf51e8101
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515029612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa111552ce92b077f0e226fd14d250252ec4643eead06a1010743c65016ee472`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:40 GMT
ADD file:b40f5b5df3c73d89ec477953753f29f16b9ebd38006d73c41b1468302e274d6f in / 
# Thu, 02 Dec 2021 23:20:40 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 23:21:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d9420f93e86b4ae7e03c24f0e4f98c3c9ea9a63b39646e47c86b1dbadc8bdec5.tar.gz"  && echo "c30aa8fe6299b9787f1287c9b7508bad1f31a056d26cf106d87670b6fe99c16f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6ce5a5560ab28234e783487f84e4b59ecf9cdd051947c044d6b557746ded7630`  
		Last Modified: Thu, 02 Dec 2021 23:22:29 GMT  
		Size: 62.4 MB (62408287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309de403a6353bf47267c55cbbfd3ce20772653b054e31dd83b30bc40380451e`  
		Last Modified: Thu, 02 Dec 2021 23:22:59 GMT  
		Size: 452.6 MB (452621325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220119.1`

**does not exist** (yet?)

## `amazonlinux:2018.03.0.20220119.1-with-sources`

**does not exist** (yet?)

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:ffc013f79b36a2c0352b444f5322ff43de25152a8ac1ad0fa473e90f1cbedcbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9c4e7b374a7a9253764876520d867ba1f5bfddeed82b029b5054cce0f71faf20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62212074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30156a0e4f040d255f30a8bf0b28540fce965398fe1c13ab29a7292e411dfde7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:20:04 GMT
ADD file:618cac8c5b6f6ff56ce221df12002d34997bcc996a0af3200b58db07d68be275 in / 
# Wed, 12 Jan 2022 02:20:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3a461b3ae562f8b6cf015b4c480a21b630a874f7fec851457680159226c81632`  
		Last Modified: Mon, 10 Jan 2022 23:29:44 GMT  
		Size: 62.2 MB (62212074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:b072eb708b1a43ebfab7745a2ed7e189722632c774efddcc03c963b0b69e6d5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63836908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:377da0386f50f197de2aef131c3df2a761d075a487cf6bbc4338ccf2916c24fe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:39:41 GMT
ADD file:afc90ca87d61fdaef5c9d192a5151ab745ac8b8ea4d7544c2dfdd66bdb3b7993 in / 
# Wed, 12 Jan 2022 02:39:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b2e274b2b0f90c3d6329566163244a0f2e6d97e4c010c62133388ac89652105f`  
		Last Modified: Wed, 12 Jan 2022 02:41:56 GMT  
		Size: 63.8 MB (63836908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:88401a082ea5ed7c7f52bae11a93ac1b21e6be238e1e015c8d1125c81eb025ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c09b199271ac2123d756575757bd922c47ce5a694f9db2918d60b8e091875875
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.2 MB (485180055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369eae5a9f20304404ae63efff50e98c2b4a2180a939d85b710cffcb8a1640c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:20:04 GMT
ADD file:618cac8c5b6f6ff56ce221df12002d34997bcc996a0af3200b58db07d68be275 in / 
# Wed, 12 Jan 2022 02:20:04 GMT
CMD ["/bin/bash"]
# Wed, 12 Jan 2022 02:23:00 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7aacabcecad2264904d2033d4072bf9e9b01b2723fb3de24f8df40bdfc2d34f7.tar.gz"  && echo "eba78093a05bb779050f6f4b93732638f4e1c21fb83c321416e0756efa88a089  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3a461b3ae562f8b6cf015b4c480a21b630a874f7fec851457680159226c81632`  
		Last Modified: Mon, 10 Jan 2022 23:29:44 GMT  
		Size: 62.2 MB (62212074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f95733a61d793aea825bb1d8d9524d99118ee03b09038bff8da69f10cc6cd8`  
		Last Modified: Wed, 12 Jan 2022 02:24:10 GMT  
		Size: 423.0 MB (422967981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ad5d2555741764f400b006e21873f1d966bef7a06905709b08d884ca5046dc82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.8 MB (486804859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69dcd260e7799a7e5ad30046fd6a56a731b92f7603c7eadff3195f6a9f5ae419`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jan 2022 02:39:41 GMT
ADD file:afc90ca87d61fdaef5c9d192a5151ab745ac8b8ea4d7544c2dfdd66bdb3b7993 in / 
# Wed, 12 Jan 2022 02:39:43 GMT
CMD ["/bin/bash"]
# Wed, 12 Jan 2022 02:41:20 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7aacabcecad2264904d2033d4072bf9e9b01b2723fb3de24f8df40bdfc2d34f7.tar.gz"  && echo "eba78093a05bb779050f6f4b93732638f4e1c21fb83c321416e0756efa88a089  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:b2e274b2b0f90c3d6329566163244a0f2e6d97e4c010c62133388ac89652105f`  
		Last Modified: Wed, 12 Jan 2022 02:41:56 GMT  
		Size: 63.8 MB (63836908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f335cb87be6e36244e570c6194cee7b36f34f1af6d0f2c4a2c61430b67b7071`  
		Last Modified: Wed, 12 Jan 2022 02:42:43 GMT  
		Size: 423.0 MB (422967951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
