<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230122.0.120412`](#archlinuxbase-202301220120412)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230122.0.120412`](#archlinuxbase-devel-202301220120412)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:345144f4b0aea995de5738475fc36785c133304a25bcb0d374ca03c3f0660573
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:e7fb3b7f2840a68d9dd07ad5741dd9a773fde63d870c568978dba329d01d172b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141925942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a72a6159a613919ca30f6811174598bae7c50f89d5803a5df66780d57590c5`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 17 Jan 2023 20:20:15 GMT
COPY dir:c42d1863a8894c21ad7df2ef8e80841e1d4ee7bc52129bb6c42421257045c0f0 in / 
# Tue, 17 Jan 2023 20:20:16 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 17 Jan 2023 20:20:17 GMT
ENV LANG=C.UTF-8
# Tue, 17 Jan 2023 20:20:17 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:24f427444b18bd52922792c35a34d27186ebb645bda49bc594dbb7369c0696aa`  
		Last Modified: Tue, 17 Jan 2023 20:21:58 GMT  
		Size: 141.9 MB (141917994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee5bd4dd5b9171bcd78eb3169a8d65d0cc0700b0d41bcc3b61711b00da2ee69`  
		Last Modified: Tue, 17 Jan 2023 20:21:37 GMT  
		Size: 7.9 KB (7948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230122.0.120412`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:3c83e1f50048816af25445a8bedf1fe32970744a504154214cbfe64b48a93677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:d363f036cbbe40976a3b5883712fa56637a7245c24eca278d9afe71d64a93aea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.3 MB (243275732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35a14990e418befb73692b1ec51a76ae3c34197dd0567a0722b0aa020cac7395`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 17 Jan 2023 20:21:14 GMT
COPY dir:c3807cae7579da7832d9d3bc75212b97fc1966cec9bf93ecd82d62c2e02358ae in / 
# Tue, 17 Jan 2023 20:21:17 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 17 Jan 2023 20:21:17 GMT
ENV LANG=C.UTF-8
# Tue, 17 Jan 2023 20:21:17 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:25026b95ecab1e6bf51e54bd471db73dcc64fd0a13e8ecc9b691e01039afb119`  
		Last Modified: Tue, 17 Jan 2023 20:22:44 GMT  
		Size: 243.3 MB (243267105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13727ffa379b51b5a4f7002874399fa5cf02574e6ad79fb9d45076b5f8441e6`  
		Last Modified: Tue, 17 Jan 2023 20:22:09 GMT  
		Size: 8.6 KB (8627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230122.0.120412`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:345144f4b0aea995de5738475fc36785c133304a25bcb0d374ca03c3f0660573
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:e7fb3b7f2840a68d9dd07ad5741dd9a773fde63d870c568978dba329d01d172b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141925942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a72a6159a613919ca30f6811174598bae7c50f89d5803a5df66780d57590c5`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 17 Jan 2023 20:20:15 GMT
COPY dir:c42d1863a8894c21ad7df2ef8e80841e1d4ee7bc52129bb6c42421257045c0f0 in / 
# Tue, 17 Jan 2023 20:20:16 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 17 Jan 2023 20:20:17 GMT
ENV LANG=C.UTF-8
# Tue, 17 Jan 2023 20:20:17 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:24f427444b18bd52922792c35a34d27186ebb645bda49bc594dbb7369c0696aa`  
		Last Modified: Tue, 17 Jan 2023 20:21:58 GMT  
		Size: 141.9 MB (141917994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee5bd4dd5b9171bcd78eb3169a8d65d0cc0700b0d41bcc3b61711b00da2ee69`  
		Last Modified: Tue, 17 Jan 2023 20:21:37 GMT  
		Size: 7.9 KB (7948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
