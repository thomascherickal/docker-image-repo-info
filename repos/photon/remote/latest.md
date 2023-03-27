## `photon:latest`

```console
$ docker pull photon@sha256:b05250c0910833a75fec1430ed7bbafd046ca8699eb3d350e0181bd2b41aae6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:2c9ad1739e409831bac3adc874e24cf749f07dd8cbb028699eb446b280d25217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16083195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acfe6fc63dcbb9175bf1a045f77030356aceb24fbd361be7dea4bcd78e599d63`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Mar 2023 18:21:13 GMT
ADD file:f7d25cf520073cd15407eebf5f523e5d53cdb5f8a9bc7c10090920cec8d0e39f in / 
# Mon, 27 Mar 2023 18:21:14 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20230325
# Mon, 27 Mar 2023 18:21:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:59695153de0d280efefe0b529aef9246b7ac4a44281b609b854dee3abefc2401`  
		Last Modified: Mon, 27 Mar 2023 18:21:38 GMT  
		Size: 16.1 MB (16083195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:96c77056fc16b3d881e73782364c62060f5290fb9c54598c41bb15cfc4f15f5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15169641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57db8be170d5302f4ff87d6ea224099dd552fb3eb107f773916720008b41fe08`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Mar 2023 18:47:47 GMT
ADD file:c053277abb1088e8402c9802aaa1d08f23b7937f0e8d0e98fa5a167e9312e153 in / 
# Mon, 27 Mar 2023 18:47:47 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20230325
# Mon, 27 Mar 2023 18:47:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ebd68509874a23c98f1fd9563c01d6f0b6321abf6f4729f673664b0422089c02`  
		Last Modified: Mon, 27 Mar 2023 18:48:07 GMT  
		Size: 15.2 MB (15169641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
