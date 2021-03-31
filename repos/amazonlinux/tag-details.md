<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20210326.0`](#amazonlinux20202103260)
-	[`amazonlinux:2.0.20210326.0-with-sources`](#amazonlinux20202103260-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20210319.0`](#amazonlinux2018030202103190)
-	[`amazonlinux:2018.03.0.20210319.0-with-sources`](#amazonlinux2018030202103190-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:3938c216b45dbf699264ccc2fd44841bb9e3ddec08b06ad1e5b0f5efa8efb91d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e87eddd9673f8c9572c9d8fdc62fd3623d327f31cd244a8e2b618148d3f08e65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62237383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97e9a24da3a72d938cbfa3d81ae8946866d23a95c6192c6e457f6e96246eb19c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:50 GMT
ADD file:da200ac5c51ffde7abae35c82ed6e30c690882ff1f9820d4cf473bb4040ae106 in / 
# Tue, 30 Mar 2021 21:59:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e48d2aca327e0da277489942827d8ab487cdbeffd3edf30bc49ddc61bed05f2f`  
		Last Modified: Tue, 30 Mar 2021 22:01:33 GMT  
		Size: 62.2 MB (62237383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:2a3bab7e020e521e70ae7b4a287d4e1100f7afd4dcaf3150074a6efc85e0b328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:55c9c7ea173f7a807040710a03fcff5bbee34bcc96ab4fee9bb247eb507acde8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449100342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71907c2cf3d74fea02b3d1f947c42c09b5738882cbe5af66b43ca764a18a6016`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:50 GMT
ADD file:da200ac5c51ffde7abae35c82ed6e30c690882ff1f9820d4cf473bb4040ae106 in / 
# Tue, 30 Mar 2021 21:59:51 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 22:00:06 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-dc5d92c927a9f79aab7658e5c05df877dd40282d7bf9b4b11a5eb11b225cb7ad.tar.gz"  && echo "03509f1ca8f0593cf761a9fda3dc71baf0f45752a0d8908a04ccd9937bd1ddfc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e48d2aca327e0da277489942827d8ab487cdbeffd3edf30bc49ddc61bed05f2f`  
		Last Modified: Tue, 30 Mar 2021 22:01:33 GMT  
		Size: 62.2 MB (62237383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9ab6a3693e0cf7dee1138b844daf28d5d474449b158560dcd916c6dd189fa`  
		Last Modified: Tue, 30 Mar 2021 22:02:05 GMT  
		Size: 386.9 MB (386862959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:06380711d6a8ac0b6989f7e2a4419e560796791d9c7c843753a719c73552dc30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:bfc3ba0cc5604df7e13d85e39a2a27a1dc93885f24184423524adf50a4ecd916
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61946585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c0b9bec08e6887cb8bf67884fcb5cc62bfa0fec17a732278ac18309d9a3c47`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:951ba8af32f239fac96f15a85302ecc868b9f88d209d1ae5563e0e27010664ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63660038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebea3c905ab61bc6c3666b7c8ae0bd44611982872f8b11ca01e0dc7877768c15`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:e65e726f83310347d83d7ffab3375e29bba9b4d2e3316dc22bf9f70776d4b4d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6a8ca270cc7529a3da4123ea10c0ee61bfd59b0e4a0db0928d05d4a45470b51b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542821098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc5900d56f8f33395ceaaba7e68666dae13a14d1a516ee4c6a1b084b4060662`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:59:38 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2bae5111d32ce9495afda9ddcd94ec2757b716e7f208b5b45ea710dc754d3ec7.tar.gz"  && echo "10bf5fa5b0b0b808615283d2de7209c58c1521c81a4953383fea0c38e1b93998  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38882999dcccafe0e4f06565dae85913942fcb9b250a3858b64618e1ef7264a1`  
		Last Modified: Tue, 30 Mar 2021 22:01:05 GMT  
		Size: 480.9 MB (480874513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:86e35f42983fda1d7e6e62e6c9073f684a444c516f66fcecbc6d60ff261ef17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544534564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a0528e0069c1ed55daa082c5603b43018e3dce5c1286aa57cd143804c753f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 22:00:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2bae5111d32ce9495afda9ddcd94ec2757b716e7f208b5b45ea710dc754d3ec7.tar.gz"  && echo "10bf5fa5b0b0b808615283d2de7209c58c1521c81a4953383fea0c38e1b93998  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9e8ca57ca152eedd246bdea5ab367dbe81d57c888320293b11d62a4aff4116`  
		Last Modified: Tue, 30 Mar 2021 22:02:12 GMT  
		Size: 480.9 MB (480874526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20210326.0`

```console
$ docker pull amazonlinux@sha256:06380711d6a8ac0b6989f7e2a4419e560796791d9c7c843753a719c73552dc30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20210326.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:bfc3ba0cc5604df7e13d85e39a2a27a1dc93885f24184423524adf50a4ecd916
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61946585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c0b9bec08e6887cb8bf67884fcb5cc62bfa0fec17a732278ac18309d9a3c47`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20210326.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:951ba8af32f239fac96f15a85302ecc868b9f88d209d1ae5563e0e27010664ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63660038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebea3c905ab61bc6c3666b7c8ae0bd44611982872f8b11ca01e0dc7877768c15`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20210326.0-with-sources`

```console
$ docker pull amazonlinux@sha256:e65e726f83310347d83d7ffab3375e29bba9b4d2e3316dc22bf9f70776d4b4d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20210326.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6a8ca270cc7529a3da4123ea10c0ee61bfd59b0e4a0db0928d05d4a45470b51b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542821098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc5900d56f8f33395ceaaba7e68666dae13a14d1a516ee4c6a1b084b4060662`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:59:38 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2bae5111d32ce9495afda9ddcd94ec2757b716e7f208b5b45ea710dc754d3ec7.tar.gz"  && echo "10bf5fa5b0b0b808615283d2de7209c58c1521c81a4953383fea0c38e1b93998  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38882999dcccafe0e4f06565dae85913942fcb9b250a3858b64618e1ef7264a1`  
		Last Modified: Tue, 30 Mar 2021 22:01:05 GMT  
		Size: 480.9 MB (480874513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20210326.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:86e35f42983fda1d7e6e62e6c9073f684a444c516f66fcecbc6d60ff261ef17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544534564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a0528e0069c1ed55daa082c5603b43018e3dce5c1286aa57cd143804c753f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 22:00:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2bae5111d32ce9495afda9ddcd94ec2757b716e7f208b5b45ea710dc754d3ec7.tar.gz"  && echo "10bf5fa5b0b0b808615283d2de7209c58c1521c81a4953383fea0c38e1b93998  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9e8ca57ca152eedd246bdea5ab367dbe81d57c888320293b11d62a4aff4116`  
		Last Modified: Tue, 30 Mar 2021 22:02:12 GMT  
		Size: 480.9 MB (480874526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:3938c216b45dbf699264ccc2fd44841bb9e3ddec08b06ad1e5b0f5efa8efb91d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e87eddd9673f8c9572c9d8fdc62fd3623d327f31cd244a8e2b618148d3f08e65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62237383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97e9a24da3a72d938cbfa3d81ae8946866d23a95c6192c6e457f6e96246eb19c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:50 GMT
ADD file:da200ac5c51ffde7abae35c82ed6e30c690882ff1f9820d4cf473bb4040ae106 in / 
# Tue, 30 Mar 2021 21:59:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e48d2aca327e0da277489942827d8ab487cdbeffd3edf30bc49ddc61bed05f2f`  
		Last Modified: Tue, 30 Mar 2021 22:01:33 GMT  
		Size: 62.2 MB (62237383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:2a3bab7e020e521e70ae7b4a287d4e1100f7afd4dcaf3150074a6efc85e0b328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:55c9c7ea173f7a807040710a03fcff5bbee34bcc96ab4fee9bb247eb507acde8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449100342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71907c2cf3d74fea02b3d1f947c42c09b5738882cbe5af66b43ca764a18a6016`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:50 GMT
ADD file:da200ac5c51ffde7abae35c82ed6e30c690882ff1f9820d4cf473bb4040ae106 in / 
# Tue, 30 Mar 2021 21:59:51 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 22:00:06 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-dc5d92c927a9f79aab7658e5c05df877dd40282d7bf9b4b11a5eb11b225cb7ad.tar.gz"  && echo "03509f1ca8f0593cf761a9fda3dc71baf0f45752a0d8908a04ccd9937bd1ddfc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e48d2aca327e0da277489942827d8ab487cdbeffd3edf30bc49ddc61bed05f2f`  
		Last Modified: Tue, 30 Mar 2021 22:01:33 GMT  
		Size: 62.2 MB (62237383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9ab6a3693e0cf7dee1138b844daf28d5d474449b158560dcd916c6dd189fa`  
		Last Modified: Tue, 30 Mar 2021 22:02:05 GMT  
		Size: 386.9 MB (386862959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20210319.0`

```console
$ docker pull amazonlinux@sha256:3938c216b45dbf699264ccc2fd44841bb9e3ddec08b06ad1e5b0f5efa8efb91d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20210319.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e87eddd9673f8c9572c9d8fdc62fd3623d327f31cd244a8e2b618148d3f08e65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62237383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97e9a24da3a72d938cbfa3d81ae8946866d23a95c6192c6e457f6e96246eb19c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:50 GMT
ADD file:da200ac5c51ffde7abae35c82ed6e30c690882ff1f9820d4cf473bb4040ae106 in / 
# Tue, 30 Mar 2021 21:59:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e48d2aca327e0da277489942827d8ab487cdbeffd3edf30bc49ddc61bed05f2f`  
		Last Modified: Tue, 30 Mar 2021 22:01:33 GMT  
		Size: 62.2 MB (62237383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20210319.0-with-sources`

```console
$ docker pull amazonlinux@sha256:2a3bab7e020e521e70ae7b4a287d4e1100f7afd4dcaf3150074a6efc85e0b328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20210319.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:55c9c7ea173f7a807040710a03fcff5bbee34bcc96ab4fee9bb247eb507acde8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449100342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71907c2cf3d74fea02b3d1f947c42c09b5738882cbe5af66b43ca764a18a6016`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:50 GMT
ADD file:da200ac5c51ffde7abae35c82ed6e30c690882ff1f9820d4cf473bb4040ae106 in / 
# Tue, 30 Mar 2021 21:59:51 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 22:00:06 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-dc5d92c927a9f79aab7658e5c05df877dd40282d7bf9b4b11a5eb11b225cb7ad.tar.gz"  && echo "03509f1ca8f0593cf761a9fda3dc71baf0f45752a0d8908a04ccd9937bd1ddfc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e48d2aca327e0da277489942827d8ab487cdbeffd3edf30bc49ddc61bed05f2f`  
		Last Modified: Tue, 30 Mar 2021 22:01:33 GMT  
		Size: 62.2 MB (62237383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9ab6a3693e0cf7dee1138b844daf28d5d474449b158560dcd916c6dd189fa`  
		Last Modified: Tue, 30 Mar 2021 22:02:05 GMT  
		Size: 386.9 MB (386862959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:06380711d6a8ac0b6989f7e2a4419e560796791d9c7c843753a719c73552dc30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:bfc3ba0cc5604df7e13d85e39a2a27a1dc93885f24184423524adf50a4ecd916
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61946585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c0b9bec08e6887cb8bf67884fcb5cc62bfa0fec17a732278ac18309d9a3c47`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:951ba8af32f239fac96f15a85302ecc868b9f88d209d1ae5563e0e27010664ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63660038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebea3c905ab61bc6c3666b7c8ae0bd44611982872f8b11ca01e0dc7877768c15`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:e65e726f83310347d83d7ffab3375e29bba9b4d2e3316dc22bf9f70776d4b4d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6a8ca270cc7529a3da4123ea10c0ee61bfd59b0e4a0db0928d05d4a45470b51b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542821098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc5900d56f8f33395ceaaba7e68666dae13a14d1a516ee4c6a1b084b4060662`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:59:38 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2bae5111d32ce9495afda9ddcd94ec2757b716e7f208b5b45ea710dc754d3ec7.tar.gz"  && echo "10bf5fa5b0b0b808615283d2de7209c58c1521c81a4953383fea0c38e1b93998  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38882999dcccafe0e4f06565dae85913942fcb9b250a3858b64618e1ef7264a1`  
		Last Modified: Tue, 30 Mar 2021 22:01:05 GMT  
		Size: 480.9 MB (480874513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:86e35f42983fda1d7e6e62e6c9073f684a444c516f66fcecbc6d60ff261ef17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544534564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a0528e0069c1ed55daa082c5603b43018e3dce5c1286aa57cd143804c753f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 22:00:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2bae5111d32ce9495afda9ddcd94ec2757b716e7f208b5b45ea710dc754d3ec7.tar.gz"  && echo "10bf5fa5b0b0b808615283d2de7209c58c1521c81a4953383fea0c38e1b93998  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9e8ca57ca152eedd246bdea5ab367dbe81d57c888320293b11d62a4aff4116`  
		Last Modified: Tue, 30 Mar 2021 22:02:12 GMT  
		Size: 480.9 MB (480874526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
