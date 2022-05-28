## `debian:stretch-backports`

```console
$ docker pull debian@sha256:c0390cfd91b55fe899a24a6565d7136b2de736ccccc308da1a800dafa0e653df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:1d0d6a315702bbd04d7da0305d4e90cb3f3ff7117d28adab876cbc6e23e234b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45429951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9735d893832716ec19e17c01b7d4687da681124c98160c2eb59bf75bdc80f187`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:22:13 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed6fc7d0b0f5abd867a03201070060f2d9e97b495be20fb62696ecfd5370e88`  
		Last Modified: Sat, 28 May 2022 01:28:55 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:fb1c1235d76db690bb01da68e0402ca5d2c1ed4d111f797b75060437b46dc8a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44123080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715afcefe509b51f1e36c84c71c4a541020ec08dadc41a8f6e96a95229aa69d2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:55:33 GMT
ADD file:95b054735b431afab54d50818bab5058e711871345ec62ca3036290e76c5002c in / 
# Wed, 11 May 2022 00:55:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 00:55:49 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:342be1c547ac3ac45aaed473477b6660f99f4de775e90a96d72de9ed5e557bd3`  
		Last Modified: Wed, 11 May 2022 01:13:02 GMT  
		Size: 44.1 MB (44122855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ac31a33faf1aa82d100c86ae2e3d30c0445c941b3e76de60751dd34a71f405`  
		Last Modified: Wed, 11 May 2022 01:13:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:9e7fa538dd6e7159df38a14d4605d43dd37aec9abefa680b8a2b00cd0617b628
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42151005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0770c300e06e44ea384bf758a6ab1d3ea36481c312de3867f6718e314dd100a8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:05:16 GMT
ADD file:f859825c79355490a08b5fd55799cc3eb1643e21abfeebe59a3a4b08e54e3f7f in / 
# Sat, 28 May 2022 01:05:17 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:05:32 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ae3d55ab33f9bf9aa2c47629e66da1c4e679da10d83c29941f39b04140996e4b`  
		Last Modified: Sat, 28 May 2022 01:21:38 GMT  
		Size: 42.2 MB (42150781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34e492b50671ebe5997ea3a6d53fcc53fc84f71d310916f9df435e0db9ab3ba`  
		Last Modified: Sat, 28 May 2022 01:21:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:5fc7f02950bd21fcdc3a88e7acab2306525943384a4208f8db27dfdb9fbb27a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43213095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0054cf0cb32b0c8d8bcf67c5a8ea640379c6d22a6f9217ce6691c051d88448c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:42:45 GMT
ADD file:93d675ee0bc32a88dc4d6c0872276c4678dc31f0b6eb8b936cb823f191bc07f0 in / 
# Sat, 28 May 2022 00:42:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:42:53 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:de7fc2a3b80bcd193de687188fc9051c8be6c61ec81fec3aeae61c079f71e69e`  
		Last Modified: Sat, 28 May 2022 00:51:21 GMT  
		Size: 43.2 MB (43212871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f8a23087310eaa4a40fcd38862b1bb74716d13e50bdc96cf59508e10d4b42e`  
		Last Modified: Sat, 28 May 2022 00:51:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:45ab1f34d75df566bdf559aee28e1ea5b0a3c7dae9a5f491d36ec230cfca0c28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46150422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0672210f2f1369953379f550b600ea341f9e4c1367281d62ae9dc43c1309086c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:41:50 GMT
ADD file:1a448f874e606582cb67d9369c97c83c78f2327fde8089b8cb6aaf476dc51935 in / 
# Sat, 28 May 2022 00:41:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:41:58 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:99b3b0cea6c21e2e36bc4c198a72e5aa3b3ab76d26c2c63d9b0c2b0add554135`  
		Last Modified: Sat, 28 May 2022 00:50:28 GMT  
		Size: 46.2 MB (46150199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75f8839e7ceac50b1a339bbdb13213aaa13cc24fe0d1e6e17d9cb66b86b33dd`  
		Last Modified: Sat, 28 May 2022 00:50:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
