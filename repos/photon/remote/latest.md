## `photon:latest`

```console
$ docker pull photon@sha256:050f0399f9b1d2ddfa12eb0393c22584bdb7ba3a1251e1ba0aa4ff2d8727fece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:27849bc9798e4715b3cde3f32ae24e2585a05a94de7d65c12186b236ed716b94
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15198877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df2d28329f8119d944f17d2720cd231cebf14e6e3a9ef61ccb742a645a275133`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 07 Aug 2020 23:38:02 GMT
ADD file:4b24bfeacaff2ff4e3d8f2d94f15f5e70018f36fad278b5c0b2c45490982c86c in / 
# Fri, 07 Aug 2020 23:38:02 GMT
LABEL name=Photon OS x86_64/3.0 Base Image vendor=VMware build-date=20200807
# Fri, 07 Aug 2020 23:38:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d8975294146ee8d6e70795ae0b464e89b1ce252532676e4fb3704b146b58d7f9`  
		Last Modified: Fri, 07 Aug 2020 23:38:41 GMT  
		Size: 15.2 MB (15198877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:dd1b61361a20402166c9028274813c89d8ba7fbe12f62a3ed2897c9fc187782e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (12985878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9e69351fd8dcb2c612ca9b64077ccb75797911ee281024c306ba10e379b3eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 14 Aug 2020 23:48:05 GMT
ADD file:7d4f60dd1e522af618a283eb3db5236fb9be72d0eb10a554d67a6a7d3e5ea8f4 in / 
# Fri, 14 Aug 2020 23:48:06 GMT
LABEL name=Photon OS aarch64/3.0 Base Image vendor=VMware build-date=20200814
# Fri, 14 Aug 2020 23:48:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:874a83eab31334d9f462133cb047cc5cf1d6a9912054eb76c1915812d13a6f8a`  
		Last Modified: Fri, 14 Aug 2020 23:48:25 GMT  
		Size: 13.0 MB (12985878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
