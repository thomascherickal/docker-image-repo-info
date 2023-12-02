## `ubuntu:lunar`

```console
$ docker pull ubuntu@sha256:852d8cab9db2e8401402528f1d845d097e672fb28a09770aa0a4278a1911b70d
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:lunar` - linux; amd64

```console
$ docker pull ubuntu@sha256:ea1285dffce8a938ef356908d1be741da594310c8dced79b870d66808cb12b0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26886018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4cdeba72b994748f5eb1f525a70a9cc553b66037ec37e23645fbf3f0f5c160d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:02:17 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:02:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:02:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:02:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:02:19 GMT
ADD file:9627edfd854222fb9117755e0e89c54a01ba3477dffb8137693b12c586d970b8 in / 
# Tue, 28 Nov 2023 09:02:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6360b371721185fefbbad6763ab745900f1b2f7714570234473232dd575fc07f`  
		Last Modified: Tue, 28 Nov 2023 09:27:24 GMT  
		Size: 26.9 MB (26886018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:4dc1dd258d16171c6cd696ed5420402319d7cabe638b176b471495e94373f2a9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24629439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83502f31cce9655561356390e34e8d506e888f6ce4743a8400bfa765f6eedb8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:725335f54d3eb8903e713867d9f04db29fbc8835da3539fd3898faa22eaf016e`  
		Last Modified: Wed, 04 Oct 2023 12:33:24 GMT  
		Size: 24.6 MB (24629439 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:aa2be6baa498ab5862770bbc08cf00a058154cb257e41dca6ef8b7f7aebe22f8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26065969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4783be26912a96818aa1c9468ea8acb5eff2608697f62deff67048595a613145`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:23:52 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:23:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:23:53 GMT
ADD file:c9b1098bc90ac9b887c3bffdffbcff0c32f32e48df9a673041e3aa796296e69b in / 
# Wed, 04 Oct 2023 12:23:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:89e6336dd9e04a0993754adca328bf88d988540bb95cff284667037dd50f79eb`  
		Last Modified: Wed, 04 Oct 2023 12:33:17 GMT  
		Size: 26.1 MB (26065969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:2d697e1fc26340ae1a77a08397f53f978a6966d3c8a3cf195ee0870ca6e7dc2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30905941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6651a10a7ea6479a915882811fa23c286c9baabb6ea68a11e48c3235246b574e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:08:54 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:08:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:08:57 GMT
ADD file:24bc2f22a395e93a2ebbcfc45da8e5fc7f08e7c03cdc985c997300643d0310ec in / 
# Wed, 04 Oct 2023 12:08:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fafd77e1a2b2b77f4b648372d147a2d31af161695aa89bed56883733707bd39f`  
		Last Modified: Wed, 04 Oct 2023 12:33:31 GMT  
		Size: 30.9 MB (30905941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; s390x

```console
$ docker pull ubuntu@sha256:e54d7ce369ad0b993654f624153bbf76a3ef547ed0dc2e14ba0a60d199077b0e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25692995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab36c0e39cab522c65337f5bfeaaf36ce62c510ca07b09d17bea00fe80bfed55`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:26:55 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:26:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:26:57 GMT
ADD file:553d1c48ed98fa8bd575a7a645019079304c101dd6e06e82591a25440fe1a9b8 in / 
# Wed, 04 Oct 2023 12:26:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8333843c4e8c11c41362709d3852d288b9deee48dfdd0014810ce4d3ef224714`  
		Last Modified: Wed, 04 Oct 2023 12:33:37 GMT  
		Size: 25.7 MB (25692995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
