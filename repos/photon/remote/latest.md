## `photon:latest`

```console
$ docker pull photon@sha256:260937dd018a50bafe1019aa01e76f9b5b7ef5bccd949a4017ea2b10bca3c373
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:8ee367ebbd3db97c25aa068125d55113d939e3f03b2cf0f83c8369e3b1c06387
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15922832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e55630e7d59df4c258aa8700b388bbcf1a9a2e25fb2a0a36a31aaa32aec55341`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Jul 2023 00:18:30 GMT
ADD file:3bd2555c9f85633e2527f9bcbe2252361d384a9b08a5ba5b773820690443e731 in / 
# Tue, 25 Jul 2023 00:18:30 GMT
LABEL name=Photon OS x86_64/5.0 Base Image vendor=VMware build-date=20230722
# Tue, 25 Jul 2023 00:18:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dc32bc79d8e83d105f43c0e5b78651d32c07387cd04b3dbac4652382182f77f0`  
		Last Modified: Tue, 25 Jul 2023 00:18:56 GMT  
		Size: 15.9 MB (15922832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:b8dcd7c9081161a68a42635fe5620f054510e13f44145aab2644f4268b1feb44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14925945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6024ffa0db80a80bc651e22c6470818085c5c1c18ddf24bfac6bf911b6493b3c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 24 Jul 2023 22:07:32 GMT
ADD file:0a19e9073876672f760a6c11e34a17e34cd43fdaefdd0b9299275831a5c6ed46 in / 
# Mon, 24 Jul 2023 22:07:32 GMT
LABEL name=Photon OS aarch64/5.0 Base Image vendor=VMware build-date=20230722
# Mon, 24 Jul 2023 22:07:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dc75f982711b298db2c6a030ab58914ea755738657486225e12620524fc936ee`  
		Last Modified: Mon, 24 Jul 2023 22:07:53 GMT  
		Size: 14.9 MB (14925945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
