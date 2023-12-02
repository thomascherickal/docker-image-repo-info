<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:22.04`](#ubuntu2204)
-	[`ubuntu:23.04`](#ubuntu2304)
-	[`ubuntu:23.10`](#ubuntu2310)
-	[`ubuntu:24.04`](#ubuntu2404)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20231128`](#ubuntufocal-20231128)
-	[`ubuntu:jammy`](#ubuntujammy)
-	[`ubuntu:jammy-20231128`](#ubuntujammy-20231128)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:lunar`](#ubuntulunar)
-	[`ubuntu:lunar-20231128`](#ubuntulunar-20231128)
-	[`ubuntu:mantic`](#ubuntumantic)
-	[`ubuntu:mantic-20231128`](#ubuntumantic-20231128)
-	[`ubuntu:noble`](#ubuntunoble)
-	[`ubuntu:noble-20231126.1`](#ubuntunoble-202311261)
-	[`ubuntu:rolling`](#ubunturolling)

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:379b13f42b4e34bb00adb1d322ffead668231536563dc3ad2840180d8191c968
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:20.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:fe8a36445d3d850960d6a24554f2cf4e19d82ba1e611e3e8713bd7b76989623d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27512563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83a4bf3bb050e11e0f3bfdcfaff38eeb1dd851b7a362d930cd590dd97b3b1687`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:06e174da2c1a4cd683a888d933a235407a02f2d98fedb49c34601b293fc5e36e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23612914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eba8b8e77a0ca1c3d8315507ef4e67d817fb199a4cdbc603a0e06fb1b9f78ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a50255c0017d09ab86514148fe36d006a4ad9a46633b82efd4b0233a9c9082e8`  
		Last Modified: Tue, 03 Oct 2023 11:16:56 GMT  
		Size: 23.6 MB (23612914 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:074f14759aac23ee1f3ec318fbc1baa83f309ff78ad4448d63f79d2c8bea24c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25975507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51abb690a3439f2dc40cd5546d184a849ecba847491d2acbaebaec01d90196db`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:647745abc179283618fc640158b3a0c0cdd76b6d8e68feb4d96c4174451f2c3f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59af7d4768482e1b3e0f3bda4f41accb3b4d7ef0e41b65bf07fdd4cfde97f80b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:22:52 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:22:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:22:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:22:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:22:55 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Tue, 28 Nov 2023 05:22:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:efac268f6ae0690e6212150a83c96d2063c29df1b9514da029d061f1c5d2a483`  
		Last Modified: Tue, 28 Nov 2023 05:37:38 GMT  
		Size: 32.1 MB (32075384 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:e3a8fd652ab4f3349c1c1e872ce5dc8f904ee5e702da67a052de21ba1a73bdfc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26363432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2100e7bf53362df619b569b29c7edd960f4091de1b47ad8838c16444b53b0d5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:20:48 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:20:50 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Tue, 28 Nov 2023 05:20:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1baa125247957ef5c6754c3e8f1d9b1a6a073bc38c8f3f5a37d3bf31b377f6c0`  
		Last Modified: Tue, 28 Nov 2023 05:37:46 GMT  
		Size: 26.4 MB (26363432 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.04`

```console
$ docker pull ubuntu@sha256:e72750c6564f1911cf2bc6b43f56f266f72d259c09b9fa3bcfc8d0182a466893
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:22.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:149d67e29f765f4db62aa52161009e99e389544e25a8f43c8c89d4a445a7ca37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29547417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6548eacb0639263e9d8abfee48f8ac8b327102a05335b67572f715c580a968e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5e8117c0bd28aecad06f7e76d4d3b64734d59c1a0a44541d18060cd8fba30c50`  
		Last Modified: Fri, 01 Dec 2023 08:21:32 GMT  
		Size: 29.5 MB (29547417 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:212b9f426e7be12bf9a80b65e1a14fc39e319cff3a7857772b21c02f1eaff610
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26629612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3f9d425ffe4e459ab4cfc7b6f32c504d3f86b0fcb2a1b58d7646ab045ca4c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4091a3a7d6aa711dc0e0bbacfd3546df44ca257c300de1ad00fbdc95e218f7bd`  
		Last Modified: Thu, 05 Oct 2023 07:43:39 GMT  
		Size: 26.6 MB (26629612 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:5b5a3f7bd48cdcd8ff523361ae281a4a645b1d7889b5a15856ea540e68fba5c4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27357622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031631b933269c0c43a31cb8444745bf85c032d8166276b40e428843c8f54472`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:32ba3a3141d26dce5dc8f42b11b36e32f5986433d380291ba7f98b143af3fc46`  
		Last Modified: Fri, 01 Dec 2023 08:21:38 GMT  
		Size: 27.4 MB (27357622 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b3822149d5c0170039f6f39fc0fda06c2467e4472378b9850bad1792b83e46d5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34528110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25984a1694332640432648189383e67e9677a3e39d9a3b6831e8aada68a2708`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5314902d38478222f7d8dabbc907136e36fc9e8ea9b40b24a6b7085a981ac37c`  
		Last Modified: Fri, 01 Dec 2023 08:22:04 GMT  
		Size: 34.5 MB (34528110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:f41668699eb7c917d00f9cd97fdebe746eb34e6331a74c7995370bafd938b048
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28026463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b4b5d0bbf65145807bbe5d2845ca5ace09a6117b31b4a08b6895c8b33df360`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 08:11:20 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:11:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:11:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:11:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:11:22 GMT
ADD file:1e0a0e74040ce284db152e44fa004b927dfe7ed6482ff2b6541b73de409f38e8 in / 
# Fri, 01 Dec 2023 08:11:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b3ec46dd4bd918c0959c5eb4c7186c3d99e420988ebc621684d9077697bb5a62`  
		Last Modified: Fri, 01 Dec 2023 08:22:10 GMT  
		Size: 28.0 MB (28026463 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.04`

```console
$ docker pull ubuntu@sha256:861c743b5b8529d608d9e9561b04d633cb7dd85abeea0c9e65a54a8279630a67
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:23.04` - linux; amd64

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

### `ubuntu:23.04` - linux; arm variant v7

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

### `ubuntu:23.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:15db3e6b59a9119916cd858d52e6d4cef718c02c781dce5cf0fe5d03d933b73c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26079900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438c28bcdb9f7216366ebe5113f796f5404a28dea1790f34929e1251264e45a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:09:50 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:09:50 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:09:53 GMT
ADD file:6859e1ffc351c0e88484a54fa40a0e572765d4c34180b05901ea0adab3a5928b in / 
# Tue, 28 Nov 2023 09:09:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d8df4a5e885db4891759c9d9cfc2e43aee3f9aabf9527d938bb46d115e03e8da`  
		Last Modified: Tue, 28 Nov 2023 09:27:30 GMT  
		Size: 26.1 MB (26079900 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:c28fa7ea101bb0a00eff5a308adc23ab2e38233fb5d774159312e3c3a76c8117
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30917966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e62d935d40f82192cbff6f4484a55808f2768c86a03a58d529a523394d24c12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:18:09 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:18:10 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:18:12 GMT
ADD file:6b3f0585aa120c4ab6a2a030727088bedc6e7d88a01d65c847d77f311637589f in / 
# Tue, 28 Nov 2023 09:18:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:560944132ff1df4504e996c465ce940bd939a402ada0807793d05ca35535070c`  
		Last Modified: Tue, 28 Nov 2023 09:27:55 GMT  
		Size: 30.9 MB (30917966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:b9e4e416dbed67b9ddc739e89ef6352e80636153335eda2083a5f8e2895b1a27
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25705524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ffbdfac8172ad59a8598c19128ed08f06dfd85348b13a614aa85ff9d67a093`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:17:26 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:17:26 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:17:28 GMT
ADD file:34e95cddd67480da1b7990b0957bd24393bc65dc923e9af86031a3b55ee0d3c8 in / 
# Tue, 28 Nov 2023 09:17:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f1590276a0ea31f1d9c79822d84f64652790d6ba51de9ecdee58adc2e3a6ecdd`  
		Last Modified: Tue, 28 Nov 2023 09:28:01 GMT  
		Size: 25.7 MB (25705524 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.10`

```console
$ docker pull ubuntu@sha256:354b2187c7f828ffb2d7e3676139a49cc390d9a63c5f17f61d650df2b7c366bd
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:23.10` - linux; amd64

```console
$ docker pull ubuntu@sha256:8d093e0651575a6437cc4a3d561f892a345d263aeac6156ef378fe6a4ccabd4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27273553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a94112583ff9c6d0a7b67348fc3b0ee5bbf104a86a9e24585c9ad1028fd25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:54:17 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:54:19 GMT
ADD file:5430e0b4ea856c760b6e2b88e8c2cd2d49704ed2f3c53ae34c10750a608d40ec in / 
# Thu, 30 Nov 2023 17:54:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:767829bcf202e4fa7e777f29d390307e29ac437f131685a1ff1293d44705ca23`  
		Last Modified: Thu, 30 Nov 2023 18:06:39 GMT  
		Size: 27.3 MB (27273553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2a465a4c4831c57977b6646e481f504061294f1bf1ae1b99fb5d93c67b8a471a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25201383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc753c284b47a7a5ff3ec2e926551ba95dc6c9072415649cb13a9cdff503dc04`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8761b0d436cd2e1ff47496b7cc353cf0b49347ffc92b070c31a5cf5431041614`  
		Last Modified: Wed, 11 Oct 2023 18:18:00 GMT  
		Size: 25.2 MB (25201383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:694c2aa053066101c5f29e909d4baaea478ac50e499d452f510c10e961ebb42f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26391312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382e20053971e462c74b86d6dd56f440693ddf596f0fb4989a9ef87ffb1bd5a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:41:07 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:41:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:41:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:41:07 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:41:09 GMT
ADD file:973e000ef2f95dfa48695815ebd7027db718c9fe80260271e43ee06fddfd073b in / 
# Thu, 30 Nov 2023 17:41:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b227d7805fb6cba5d091f0565054ae9ed1e13a6e2df91de4cfb41f70e208da31`  
		Last Modified: Thu, 30 Nov 2023 18:06:46 GMT  
		Size: 26.4 MB (26391312 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:22c4449e6ef2d40adecaf8ecc4df1bd80a701c12f89f29f15245189cd3da22b1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31346558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eab81e5b01a3726fd0cdbe70cf8d42317086e71ef61ad68667b29af27db455b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:57:33 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:57:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:57:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:57:34 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:57:37 GMT
ADD file:d08e45288fbc31570a3a92ae480bf6ac3ed8e4900b3260d56a51ce024818b6fe in / 
# Thu, 30 Nov 2023 17:57:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:86fa66fe8d0305c6369ae9bf03d1677c1d99b5cefbef6dd550617a300956d5b6`  
		Last Modified: Thu, 30 Nov 2023 18:06:59 GMT  
		Size: 31.3 MB (31346558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:f9bd1296086163c80f76427fb987a4ecf6799b490c724fc0bea92e66d60620cf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27094013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4bd2cee374af30258d9d818b2ef084ef72674c8a1304bc94b177dc70da33166`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:42:50 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:42:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:42:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:42:51 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:42:53 GMT
ADD file:63283c7c5d335fa063fe3da82fa78d45ed5af9327a2d154bad18a8711485db77 in / 
# Thu, 30 Nov 2023 17:42:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5ab01e9ae41fd34fc412118be6d5e21f82290394cf86ba09cd54207fa341e2d9`  
		Last Modified: Thu, 30 Nov 2023 18:07:13 GMT  
		Size: 27.1 MB (27094013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:24.04`

```console
$ docker pull ubuntu@sha256:60b647f056b54ebce877c6dfcab95f512f0b22624e94b1e1878c83e0337db45e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:24.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef2b3c979842614a9537785f2dcc5e93a977fa50dc567c42a7d4f5ea6470fec0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27213697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf276bdd215773746bde9489a88d063b98584b8a650272c037da7be94941a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:09:34 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:09:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:09:35 GMT
ADD file:b2f5aa693e38f0ebe3e4d26ded8f957b4eb6f75c8360340cfcdeee25bf1b1b40 in / 
# Mon, 27 Nov 2023 11:09:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:62a1d607dcd86fd912d7d1448a129970b9c35f5506fbc48f8fea327ec9706b14`  
		Last Modified: Mon, 27 Nov 2023 11:15:40 GMT  
		Size: 27.2 MB (27213697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:24.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:cef62b26f726dd229d5169a3dd6c43a6d4f779753ad0bb7ec79767612eca6d07
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26374487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a9ca3da4a89ce3b696e991e2746ef3fd43ba45e0f865e10826a5ffa412ec80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 10:59:44 GMT
ARG RELEASE
# Mon, 27 Nov 2023 10:59:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 10:59:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 10:59:44 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 10:59:45 GMT
ADD file:92c5394029d3289245a20d89db9042438c196e87f86d2c2b38ef039a94e34ea1 in / 
# Mon, 27 Nov 2023 10:59:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:280505470bcff1adb1835bdfe9c6a43d01e8f619dfc2149dfdf782f2e3586f6f`  
		Last Modified: Mon, 27 Nov 2023 11:15:48 GMT  
		Size: 26.4 MB (26374487 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:24.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:7507a6b5347931e91ccbf64eccb1d47d9b1a3c8c731b370efd21fbc28c08bfb5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31316257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de3a97de9876c2336ea46851c0df7a2d9ad45c60022dfbff95d5d6e75ccefca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 10:59:52 GMT
ARG RELEASE
# Mon, 27 Nov 2023 10:59:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 10:59:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 10:59:53 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 10:59:55 GMT
ADD file:63fd35cafc829797c017809779c1ff420497005f85c88df5d033722104683537 in / 
# Mon, 27 Nov 2023 10:59:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5bb3f3c327d75c33efbc824eb228df818cdf339da3fdd25997cbb0e8e84093ba`  
		Last Modified: Mon, 27 Nov 2023 11:16:00 GMT  
		Size: 31.3 MB (31316257 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:24.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:02b206da5e7735063f201ecce4b1fd4d43e2c624e9abafde928a7097cef935c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27193420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2bcb51370031c182472d927c17f5f86bb7994d65bb928427c271ffa6141f5b7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:01:31 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:01:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:01:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:01:31 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:01:33 GMT
ADD file:c05030a894e86ddc5d70ff8a2d6332f1d879fa59044c55b03f4bff46b334e1bb in / 
# Mon, 27 Nov 2023 11:01:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5dc2945941767d28b766b0e98aae2c27161db418c3e6dfa4323fc53ab51b8cfc`  
		Last Modified: Mon, 27 Nov 2023 11:16:06 GMT  
		Size: 27.2 MB (27193420 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:e75813741b2b9106a87c91f4a1dc11afb2b71e2ee78c898a0e982b9ccf973e57
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:devel` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef2b3c979842614a9537785f2dcc5e93a977fa50dc567c42a7d4f5ea6470fec0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27213697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf276bdd215773746bde9489a88d063b98584b8a650272c037da7be94941a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:09:34 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:09:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:09:35 GMT
ADD file:b2f5aa693e38f0ebe3e4d26ded8f957b4eb6f75c8360340cfcdeee25bf1b1b40 in / 
# Mon, 27 Nov 2023 11:09:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:62a1d607dcd86fd912d7d1448a129970b9c35f5506fbc48f8fea327ec9706b14`  
		Last Modified: Mon, 27 Nov 2023 11:15:40 GMT  
		Size: 27.2 MB (27213697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:832381cafc44879857f084dd780d246e2afc077bb9f97cc76d02665b50a7b51b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25244973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e05e891c9b4d59dea3e056be161095328b7b723250ac89b69e4178a45e894ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:05:03 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:05:08 GMT
ADD file:512405a66f1049a7237c67d9d5776db7f41d5991eceec535260f4d3b7f19e65d in / 
# Tue, 26 Sep 2023 05:05:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:956aaffe9fe2861fc716bca41f30a50ff2eb645844bc74edb8b90428a5ef3637`  
		Last Modified: Tue, 26 Sep 2023 05:34:08 GMT  
		Size: 25.2 MB (25244973 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:cef62b26f726dd229d5169a3dd6c43a6d4f779753ad0bb7ec79767612eca6d07
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26374487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a9ca3da4a89ce3b696e991e2746ef3fd43ba45e0f865e10826a5ffa412ec80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 10:59:44 GMT
ARG RELEASE
# Mon, 27 Nov 2023 10:59:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 10:59:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 10:59:44 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 10:59:45 GMT
ADD file:92c5394029d3289245a20d89db9042438c196e87f86d2c2b38ef039a94e34ea1 in / 
# Mon, 27 Nov 2023 10:59:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:280505470bcff1adb1835bdfe9c6a43d01e8f619dfc2149dfdf782f2e3586f6f`  
		Last Modified: Mon, 27 Nov 2023 11:15:48 GMT  
		Size: 26.4 MB (26374487 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:7507a6b5347931e91ccbf64eccb1d47d9b1a3c8c731b370efd21fbc28c08bfb5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31316257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de3a97de9876c2336ea46851c0df7a2d9ad45c60022dfbff95d5d6e75ccefca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 10:59:52 GMT
ARG RELEASE
# Mon, 27 Nov 2023 10:59:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 10:59:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 10:59:53 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 10:59:55 GMT
ADD file:63fd35cafc829797c017809779c1ff420497005f85c88df5d033722104683537 in / 
# Mon, 27 Nov 2023 10:59:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5bb3f3c327d75c33efbc824eb228df818cdf339da3fdd25997cbb0e8e84093ba`  
		Last Modified: Mon, 27 Nov 2023 11:16:00 GMT  
		Size: 31.3 MB (31316257 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:02b206da5e7735063f201ecce4b1fd4d43e2c624e9abafde928a7097cef935c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27193420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2bcb51370031c182472d927c17f5f86bb7994d65bb928427c271ffa6141f5b7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:01:31 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:01:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:01:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:01:31 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:01:33 GMT
ADD file:c05030a894e86ddc5d70ff8a2d6332f1d879fa59044c55b03f4bff46b334e1bb in / 
# Mon, 27 Nov 2023 11:01:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5dc2945941767d28b766b0e98aae2c27161db418c3e6dfa4323fc53ab51b8cfc`  
		Last Modified: Mon, 27 Nov 2023 11:16:06 GMT  
		Size: 27.2 MB (27193420 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:379b13f42b4e34bb00adb1d322ffead668231536563dc3ad2840180d8191c968
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:focal` - linux; amd64

```console
$ docker pull ubuntu@sha256:fe8a36445d3d850960d6a24554f2cf4e19d82ba1e611e3e8713bd7b76989623d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27512563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83a4bf3bb050e11e0f3bfdcfaff38eeb1dd851b7a362d930cd590dd97b3b1687`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:06e174da2c1a4cd683a888d933a235407a02f2d98fedb49c34601b293fc5e36e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23612914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eba8b8e77a0ca1c3d8315507ef4e67d817fb199a4cdbc603a0e06fb1b9f78ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a50255c0017d09ab86514148fe36d006a4ad9a46633b82efd4b0233a9c9082e8`  
		Last Modified: Tue, 03 Oct 2023 11:16:56 GMT  
		Size: 23.6 MB (23612914 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:074f14759aac23ee1f3ec318fbc1baa83f309ff78ad4448d63f79d2c8bea24c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25975507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51abb690a3439f2dc40cd5546d184a849ecba847491d2acbaebaec01d90196db`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:647745abc179283618fc640158b3a0c0cdd76b6d8e68feb4d96c4174451f2c3f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59af7d4768482e1b3e0f3bda4f41accb3b4d7ef0e41b65bf07fdd4cfde97f80b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:22:52 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:22:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:22:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:22:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:22:55 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Tue, 28 Nov 2023 05:22:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:efac268f6ae0690e6212150a83c96d2063c29df1b9514da029d061f1c5d2a483`  
		Last Modified: Tue, 28 Nov 2023 05:37:38 GMT  
		Size: 32.1 MB (32075384 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:e3a8fd652ab4f3349c1c1e872ce5dc8f904ee5e702da67a052de21ba1a73bdfc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26363432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2100e7bf53362df619b569b29c7edd960f4091de1b47ad8838c16444b53b0d5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:20:48 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:20:50 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Tue, 28 Nov 2023 05:20:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1baa125247957ef5c6754c3e8f1d9b1a6a073bc38c8f3f5a37d3bf31b377f6c0`  
		Last Modified: Tue, 28 Nov 2023 05:37:46 GMT  
		Size: 26.4 MB (26363432 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal-20231128`

```console
$ docker pull ubuntu@sha256:f5163780840b94495b9c095ee4e42765a20277dfc37270e8db43b226180df6e3
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:focal-20231128` - linux; amd64

```console
$ docker pull ubuntu@sha256:fe8a36445d3d850960d6a24554f2cf4e19d82ba1e611e3e8713bd7b76989623d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27512563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83a4bf3bb050e11e0f3bfdcfaff38eeb1dd851b7a362d930cd590dd97b3b1687`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20231128` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:074f14759aac23ee1f3ec318fbc1baa83f309ff78ad4448d63f79d2c8bea24c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25975507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51abb690a3439f2dc40cd5546d184a849ecba847491d2acbaebaec01d90196db`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20231128` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:647745abc179283618fc640158b3a0c0cdd76b6d8e68feb4d96c4174451f2c3f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59af7d4768482e1b3e0f3bda4f41accb3b4d7ef0e41b65bf07fdd4cfde97f80b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:22:52 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:22:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:22:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:22:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:22:55 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Tue, 28 Nov 2023 05:22:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:efac268f6ae0690e6212150a83c96d2063c29df1b9514da029d061f1c5d2a483`  
		Last Modified: Tue, 28 Nov 2023 05:37:38 GMT  
		Size: 32.1 MB (32075384 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20231128` - linux; s390x

```console
$ docker pull ubuntu@sha256:e3a8fd652ab4f3349c1c1e872ce5dc8f904ee5e702da67a052de21ba1a73bdfc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26363432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2100e7bf53362df619b569b29c7edd960f4091de1b47ad8838c16444b53b0d5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:20:48 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:20:50 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Tue, 28 Nov 2023 05:20:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1baa125247957ef5c6754c3e8f1d9b1a6a073bc38c8f3f5a37d3bf31b377f6c0`  
		Last Modified: Tue, 28 Nov 2023 05:37:46 GMT  
		Size: 26.4 MB (26363432 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy`

```console
$ docker pull ubuntu@sha256:e72750c6564f1911cf2bc6b43f56f266f72d259c09b9fa3bcfc8d0182a466893
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:jammy` - linux; amd64

```console
$ docker pull ubuntu@sha256:149d67e29f765f4db62aa52161009e99e389544e25a8f43c8c89d4a445a7ca37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29547417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6548eacb0639263e9d8abfee48f8ac8b327102a05335b67572f715c580a968e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5e8117c0bd28aecad06f7e76d4d3b64734d59c1a0a44541d18060cd8fba30c50`  
		Last Modified: Fri, 01 Dec 2023 08:21:32 GMT  
		Size: 29.5 MB (29547417 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:212b9f426e7be12bf9a80b65e1a14fc39e319cff3a7857772b21c02f1eaff610
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26629612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3f9d425ffe4e459ab4cfc7b6f32c504d3f86b0fcb2a1b58d7646ab045ca4c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4091a3a7d6aa711dc0e0bbacfd3546df44ca257c300de1ad00fbdc95e218f7bd`  
		Last Modified: Thu, 05 Oct 2023 07:43:39 GMT  
		Size: 26.6 MB (26629612 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:5b5a3f7bd48cdcd8ff523361ae281a4a645b1d7889b5a15856ea540e68fba5c4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27357622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031631b933269c0c43a31cb8444745bf85c032d8166276b40e428843c8f54472`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:32ba3a3141d26dce5dc8f42b11b36e32f5986433d380291ba7f98b143af3fc46`  
		Last Modified: Fri, 01 Dec 2023 08:21:38 GMT  
		Size: 27.4 MB (27357622 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b3822149d5c0170039f6f39fc0fda06c2467e4472378b9850bad1792b83e46d5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34528110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25984a1694332640432648189383e67e9677a3e39d9a3b6831e8aada68a2708`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5314902d38478222f7d8dabbc907136e36fc9e8ea9b40b24a6b7085a981ac37c`  
		Last Modified: Fri, 01 Dec 2023 08:22:04 GMT  
		Size: 34.5 MB (34528110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; s390x

```console
$ docker pull ubuntu@sha256:f41668699eb7c917d00f9cd97fdebe746eb34e6331a74c7995370bafd938b048
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28026463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b4b5d0bbf65145807bbe5d2845ca5ace09a6117b31b4a08b6895c8b33df360`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 08:11:20 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:11:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:11:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:11:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:11:22 GMT
ADD file:1e0a0e74040ce284db152e44fa004b927dfe7ed6482ff2b6541b73de409f38e8 in / 
# Fri, 01 Dec 2023 08:11:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b3ec46dd4bd918c0959c5eb4c7186c3d99e420988ebc621684d9077697bb5a62`  
		Last Modified: Fri, 01 Dec 2023 08:22:10 GMT  
		Size: 28.0 MB (28026463 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy-20231128`

```console
$ docker pull ubuntu@sha256:1d507191f366f57bc6870f9ec229141efe8204af453983a4812b06b0f79e45af
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:jammy-20231128` - linux; amd64

```console
$ docker pull ubuntu@sha256:149d67e29f765f4db62aa52161009e99e389544e25a8f43c8c89d4a445a7ca37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29547417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6548eacb0639263e9d8abfee48f8ac8b327102a05335b67572f715c580a968e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5e8117c0bd28aecad06f7e76d4d3b64734d59c1a0a44541d18060cd8fba30c50`  
		Last Modified: Fri, 01 Dec 2023 08:21:32 GMT  
		Size: 29.5 MB (29547417 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy-20231128` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:5b5a3f7bd48cdcd8ff523361ae281a4a645b1d7889b5a15856ea540e68fba5c4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27357622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031631b933269c0c43a31cb8444745bf85c032d8166276b40e428843c8f54472`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:32ba3a3141d26dce5dc8f42b11b36e32f5986433d380291ba7f98b143af3fc46`  
		Last Modified: Fri, 01 Dec 2023 08:21:38 GMT  
		Size: 27.4 MB (27357622 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy-20231128` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b3822149d5c0170039f6f39fc0fda06c2467e4472378b9850bad1792b83e46d5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34528110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25984a1694332640432648189383e67e9677a3e39d9a3b6831e8aada68a2708`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5314902d38478222f7d8dabbc907136e36fc9e8ea9b40b24a6b7085a981ac37c`  
		Last Modified: Fri, 01 Dec 2023 08:22:04 GMT  
		Size: 34.5 MB (34528110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy-20231128` - linux; s390x

```console
$ docker pull ubuntu@sha256:f41668699eb7c917d00f9cd97fdebe746eb34e6331a74c7995370bafd938b048
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28026463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b4b5d0bbf65145807bbe5d2845ca5ace09a6117b31b4a08b6895c8b33df360`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 08:11:20 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:11:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:11:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:11:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:11:22 GMT
ADD file:1e0a0e74040ce284db152e44fa004b927dfe7ed6482ff2b6541b73de409f38e8 in / 
# Fri, 01 Dec 2023 08:11:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b3ec46dd4bd918c0959c5eb4c7186c3d99e420988ebc621684d9077697bb5a62`  
		Last Modified: Fri, 01 Dec 2023 08:22:10 GMT  
		Size: 28.0 MB (28026463 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:e72750c6564f1911cf2bc6b43f56f266f72d259c09b9fa3bcfc8d0182a466893
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:latest` - linux; amd64

```console
$ docker pull ubuntu@sha256:149d67e29f765f4db62aa52161009e99e389544e25a8f43c8c89d4a445a7ca37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29547417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6548eacb0639263e9d8abfee48f8ac8b327102a05335b67572f715c580a968e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5e8117c0bd28aecad06f7e76d4d3b64734d59c1a0a44541d18060cd8fba30c50`  
		Last Modified: Fri, 01 Dec 2023 08:21:32 GMT  
		Size: 29.5 MB (29547417 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:212b9f426e7be12bf9a80b65e1a14fc39e319cff3a7857772b21c02f1eaff610
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26629612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3f9d425ffe4e459ab4cfc7b6f32c504d3f86b0fcb2a1b58d7646ab045ca4c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4091a3a7d6aa711dc0e0bbacfd3546df44ca257c300de1ad00fbdc95e218f7bd`  
		Last Modified: Thu, 05 Oct 2023 07:43:39 GMT  
		Size: 26.6 MB (26629612 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:5b5a3f7bd48cdcd8ff523361ae281a4a645b1d7889b5a15856ea540e68fba5c4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27357622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031631b933269c0c43a31cb8444745bf85c032d8166276b40e428843c8f54472`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:32ba3a3141d26dce5dc8f42b11b36e32f5986433d380291ba7f98b143af3fc46`  
		Last Modified: Fri, 01 Dec 2023 08:21:38 GMT  
		Size: 27.4 MB (27357622 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b3822149d5c0170039f6f39fc0fda06c2467e4472378b9850bad1792b83e46d5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34528110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25984a1694332640432648189383e67e9677a3e39d9a3b6831e8aada68a2708`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5314902d38478222f7d8dabbc907136e36fc9e8ea9b40b24a6b7085a981ac37c`  
		Last Modified: Fri, 01 Dec 2023 08:22:04 GMT  
		Size: 34.5 MB (34528110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:f41668699eb7c917d00f9cd97fdebe746eb34e6331a74c7995370bafd938b048
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28026463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b4b5d0bbf65145807bbe5d2845ca5ace09a6117b31b4a08b6895c8b33df360`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 08:11:20 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:11:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:11:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:11:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:11:22 GMT
ADD file:1e0a0e74040ce284db152e44fa004b927dfe7ed6482ff2b6541b73de409f38e8 in / 
# Fri, 01 Dec 2023 08:11:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b3ec46dd4bd918c0959c5eb4c7186c3d99e420988ebc621684d9077697bb5a62`  
		Last Modified: Fri, 01 Dec 2023 08:22:10 GMT  
		Size: 28.0 MB (28026463 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar`

```console
$ docker pull ubuntu@sha256:861c743b5b8529d608d9e9561b04d633cb7dd85abeea0c9e65a54a8279630a67
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
$ docker pull ubuntu@sha256:15db3e6b59a9119916cd858d52e6d4cef718c02c781dce5cf0fe5d03d933b73c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26079900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438c28bcdb9f7216366ebe5113f796f5404a28dea1790f34929e1251264e45a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:09:50 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:09:50 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:09:53 GMT
ADD file:6859e1ffc351c0e88484a54fa40a0e572765d4c34180b05901ea0adab3a5928b in / 
# Tue, 28 Nov 2023 09:09:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d8df4a5e885db4891759c9d9cfc2e43aee3f9aabf9527d938bb46d115e03e8da`  
		Last Modified: Tue, 28 Nov 2023 09:27:30 GMT  
		Size: 26.1 MB (26079900 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:c28fa7ea101bb0a00eff5a308adc23ab2e38233fb5d774159312e3c3a76c8117
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30917966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e62d935d40f82192cbff6f4484a55808f2768c86a03a58d529a523394d24c12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:18:09 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:18:10 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:18:12 GMT
ADD file:6b3f0585aa120c4ab6a2a030727088bedc6e7d88a01d65c847d77f311637589f in / 
# Tue, 28 Nov 2023 09:18:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:560944132ff1df4504e996c465ce940bd939a402ada0807793d05ca35535070c`  
		Last Modified: Tue, 28 Nov 2023 09:27:55 GMT  
		Size: 30.9 MB (30917966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; s390x

```console
$ docker pull ubuntu@sha256:b9e4e416dbed67b9ddc739e89ef6352e80636153335eda2083a5f8e2895b1a27
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25705524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ffbdfac8172ad59a8598c19128ed08f06dfd85348b13a614aa85ff9d67a093`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:17:26 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:17:26 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:17:28 GMT
ADD file:34e95cddd67480da1b7990b0957bd24393bc65dc923e9af86031a3b55ee0d3c8 in / 
# Tue, 28 Nov 2023 09:17:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f1590276a0ea31f1d9c79822d84f64652790d6ba51de9ecdee58adc2e3a6ecdd`  
		Last Modified: Tue, 28 Nov 2023 09:28:01 GMT  
		Size: 25.7 MB (25705524 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar-20231128`

```console
$ docker pull ubuntu@sha256:ed20292dfaf21c0010ed6540bfe4cc394502aa843209b46296480ae4643c492b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:lunar-20231128` - linux; amd64

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

### `ubuntu:lunar-20231128` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:15db3e6b59a9119916cd858d52e6d4cef718c02c781dce5cf0fe5d03d933b73c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26079900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438c28bcdb9f7216366ebe5113f796f5404a28dea1790f34929e1251264e45a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:09:50 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:09:50 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:09:53 GMT
ADD file:6859e1ffc351c0e88484a54fa40a0e572765d4c34180b05901ea0adab3a5928b in / 
# Tue, 28 Nov 2023 09:09:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d8df4a5e885db4891759c9d9cfc2e43aee3f9aabf9527d938bb46d115e03e8da`  
		Last Modified: Tue, 28 Nov 2023 09:27:30 GMT  
		Size: 26.1 MB (26079900 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20231128` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:c28fa7ea101bb0a00eff5a308adc23ab2e38233fb5d774159312e3c3a76c8117
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30917966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e62d935d40f82192cbff6f4484a55808f2768c86a03a58d529a523394d24c12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:18:09 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:18:10 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:18:12 GMT
ADD file:6b3f0585aa120c4ab6a2a030727088bedc6e7d88a01d65c847d77f311637589f in / 
# Tue, 28 Nov 2023 09:18:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:560944132ff1df4504e996c465ce940bd939a402ada0807793d05ca35535070c`  
		Last Modified: Tue, 28 Nov 2023 09:27:55 GMT  
		Size: 30.9 MB (30917966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20231128` - linux; s390x

```console
$ docker pull ubuntu@sha256:b9e4e416dbed67b9ddc739e89ef6352e80636153335eda2083a5f8e2895b1a27
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25705524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ffbdfac8172ad59a8598c19128ed08f06dfd85348b13a614aa85ff9d67a093`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:17:26 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:17:26 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:17:28 GMT
ADD file:34e95cddd67480da1b7990b0957bd24393bc65dc923e9af86031a3b55ee0d3c8 in / 
# Tue, 28 Nov 2023 09:17:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f1590276a0ea31f1d9c79822d84f64652790d6ba51de9ecdee58adc2e3a6ecdd`  
		Last Modified: Tue, 28 Nov 2023 09:28:01 GMT  
		Size: 25.7 MB (25705524 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:mantic`

```console
$ docker pull ubuntu@sha256:354b2187c7f828ffb2d7e3676139a49cc390d9a63c5f17f61d650df2b7c366bd
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:mantic` - linux; amd64

```console
$ docker pull ubuntu@sha256:8d093e0651575a6437cc4a3d561f892a345d263aeac6156ef378fe6a4ccabd4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27273553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a94112583ff9c6d0a7b67348fc3b0ee5bbf104a86a9e24585c9ad1028fd25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:54:17 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:54:19 GMT
ADD file:5430e0b4ea856c760b6e2b88e8c2cd2d49704ed2f3c53ae34c10750a608d40ec in / 
# Thu, 30 Nov 2023 17:54:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:767829bcf202e4fa7e777f29d390307e29ac437f131685a1ff1293d44705ca23`  
		Last Modified: Thu, 30 Nov 2023 18:06:39 GMT  
		Size: 27.3 MB (27273553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2a465a4c4831c57977b6646e481f504061294f1bf1ae1b99fb5d93c67b8a471a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25201383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc753c284b47a7a5ff3ec2e926551ba95dc6c9072415649cb13a9cdff503dc04`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8761b0d436cd2e1ff47496b7cc353cf0b49347ffc92b070c31a5cf5431041614`  
		Last Modified: Wed, 11 Oct 2023 18:18:00 GMT  
		Size: 25.2 MB (25201383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:694c2aa053066101c5f29e909d4baaea478ac50e499d452f510c10e961ebb42f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26391312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382e20053971e462c74b86d6dd56f440693ddf596f0fb4989a9ef87ffb1bd5a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:41:07 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:41:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:41:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:41:07 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:41:09 GMT
ADD file:973e000ef2f95dfa48695815ebd7027db718c9fe80260271e43ee06fddfd073b in / 
# Thu, 30 Nov 2023 17:41:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b227d7805fb6cba5d091f0565054ae9ed1e13a6e2df91de4cfb41f70e208da31`  
		Last Modified: Thu, 30 Nov 2023 18:06:46 GMT  
		Size: 26.4 MB (26391312 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:22c4449e6ef2d40adecaf8ecc4df1bd80a701c12f89f29f15245189cd3da22b1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31346558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eab81e5b01a3726fd0cdbe70cf8d42317086e71ef61ad68667b29af27db455b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:57:33 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:57:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:57:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:57:34 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:57:37 GMT
ADD file:d08e45288fbc31570a3a92ae480bf6ac3ed8e4900b3260d56a51ce024818b6fe in / 
# Thu, 30 Nov 2023 17:57:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:86fa66fe8d0305c6369ae9bf03d1677c1d99b5cefbef6dd550617a300956d5b6`  
		Last Modified: Thu, 30 Nov 2023 18:06:59 GMT  
		Size: 31.3 MB (31346558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; s390x

```console
$ docker pull ubuntu@sha256:f9bd1296086163c80f76427fb987a4ecf6799b490c724fc0bea92e66d60620cf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27094013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4bd2cee374af30258d9d818b2ef084ef72674c8a1304bc94b177dc70da33166`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:42:50 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:42:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:42:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:42:51 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:42:53 GMT
ADD file:63283c7c5d335fa063fe3da82fa78d45ed5af9327a2d154bad18a8711485db77 in / 
# Thu, 30 Nov 2023 17:42:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5ab01e9ae41fd34fc412118be6d5e21f82290394cf86ba09cd54207fa341e2d9`  
		Last Modified: Thu, 30 Nov 2023 18:07:13 GMT  
		Size: 27.1 MB (27094013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:mantic-20231128`

```console
$ docker pull ubuntu@sha256:1de9ba765001777dcc9ab13070e15edc08a1c346dc21ad65383b805872dde885
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:mantic-20231128` - linux; amd64

```console
$ docker pull ubuntu@sha256:8d093e0651575a6437cc4a3d561f892a345d263aeac6156ef378fe6a4ccabd4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27273553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a94112583ff9c6d0a7b67348fc3b0ee5bbf104a86a9e24585c9ad1028fd25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:54:17 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:54:19 GMT
ADD file:5430e0b4ea856c760b6e2b88e8c2cd2d49704ed2f3c53ae34c10750a608d40ec in / 
# Thu, 30 Nov 2023 17:54:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:767829bcf202e4fa7e777f29d390307e29ac437f131685a1ff1293d44705ca23`  
		Last Modified: Thu, 30 Nov 2023 18:06:39 GMT  
		Size: 27.3 MB (27273553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic-20231128` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:694c2aa053066101c5f29e909d4baaea478ac50e499d452f510c10e961ebb42f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26391312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382e20053971e462c74b86d6dd56f440693ddf596f0fb4989a9ef87ffb1bd5a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:41:07 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:41:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:41:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:41:07 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:41:09 GMT
ADD file:973e000ef2f95dfa48695815ebd7027db718c9fe80260271e43ee06fddfd073b in / 
# Thu, 30 Nov 2023 17:41:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b227d7805fb6cba5d091f0565054ae9ed1e13a6e2df91de4cfb41f70e208da31`  
		Last Modified: Thu, 30 Nov 2023 18:06:46 GMT  
		Size: 26.4 MB (26391312 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic-20231128` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:22c4449e6ef2d40adecaf8ecc4df1bd80a701c12f89f29f15245189cd3da22b1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31346558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eab81e5b01a3726fd0cdbe70cf8d42317086e71ef61ad68667b29af27db455b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:57:33 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:57:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:57:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:57:34 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:57:37 GMT
ADD file:d08e45288fbc31570a3a92ae480bf6ac3ed8e4900b3260d56a51ce024818b6fe in / 
# Thu, 30 Nov 2023 17:57:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:86fa66fe8d0305c6369ae9bf03d1677c1d99b5cefbef6dd550617a300956d5b6`  
		Last Modified: Thu, 30 Nov 2023 18:06:59 GMT  
		Size: 31.3 MB (31346558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic-20231128` - linux; s390x

```console
$ docker pull ubuntu@sha256:f9bd1296086163c80f76427fb987a4ecf6799b490c724fc0bea92e66d60620cf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27094013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4bd2cee374af30258d9d818b2ef084ef72674c8a1304bc94b177dc70da33166`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:42:50 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:42:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:42:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:42:51 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:42:53 GMT
ADD file:63283c7c5d335fa063fe3da82fa78d45ed5af9327a2d154bad18a8711485db77 in / 
# Thu, 30 Nov 2023 17:42:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5ab01e9ae41fd34fc412118be6d5e21f82290394cf86ba09cd54207fa341e2d9`  
		Last Modified: Thu, 30 Nov 2023 18:07:13 GMT  
		Size: 27.1 MB (27094013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:noble`

```console
$ docker pull ubuntu@sha256:60b647f056b54ebce877c6dfcab95f512f0b22624e94b1e1878c83e0337db45e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:noble` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef2b3c979842614a9537785f2dcc5e93a977fa50dc567c42a7d4f5ea6470fec0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27213697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf276bdd215773746bde9489a88d063b98584b8a650272c037da7be94941a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:09:34 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:09:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:09:35 GMT
ADD file:b2f5aa693e38f0ebe3e4d26ded8f957b4eb6f75c8360340cfcdeee25bf1b1b40 in / 
# Mon, 27 Nov 2023 11:09:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:62a1d607dcd86fd912d7d1448a129970b9c35f5506fbc48f8fea327ec9706b14`  
		Last Modified: Mon, 27 Nov 2023 11:15:40 GMT  
		Size: 27.2 MB (27213697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:noble` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:cef62b26f726dd229d5169a3dd6c43a6d4f779753ad0bb7ec79767612eca6d07
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26374487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a9ca3da4a89ce3b696e991e2746ef3fd43ba45e0f865e10826a5ffa412ec80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 10:59:44 GMT
ARG RELEASE
# Mon, 27 Nov 2023 10:59:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 10:59:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 10:59:44 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 10:59:45 GMT
ADD file:92c5394029d3289245a20d89db9042438c196e87f86d2c2b38ef039a94e34ea1 in / 
# Mon, 27 Nov 2023 10:59:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:280505470bcff1adb1835bdfe9c6a43d01e8f619dfc2149dfdf782f2e3586f6f`  
		Last Modified: Mon, 27 Nov 2023 11:15:48 GMT  
		Size: 26.4 MB (26374487 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:noble` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:7507a6b5347931e91ccbf64eccb1d47d9b1a3c8c731b370efd21fbc28c08bfb5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31316257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de3a97de9876c2336ea46851c0df7a2d9ad45c60022dfbff95d5d6e75ccefca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 10:59:52 GMT
ARG RELEASE
# Mon, 27 Nov 2023 10:59:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 10:59:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 10:59:53 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 10:59:55 GMT
ADD file:63fd35cafc829797c017809779c1ff420497005f85c88df5d033722104683537 in / 
# Mon, 27 Nov 2023 10:59:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5bb3f3c327d75c33efbc824eb228df818cdf339da3fdd25997cbb0e8e84093ba`  
		Last Modified: Mon, 27 Nov 2023 11:16:00 GMT  
		Size: 31.3 MB (31316257 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:noble` - linux; s390x

```console
$ docker pull ubuntu@sha256:02b206da5e7735063f201ecce4b1fd4d43e2c624e9abafde928a7097cef935c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27193420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2bcb51370031c182472d927c17f5f86bb7994d65bb928427c271ffa6141f5b7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:01:31 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:01:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:01:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:01:31 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:01:33 GMT
ADD file:c05030a894e86ddc5d70ff8a2d6332f1d879fa59044c55b03f4bff46b334e1bb in / 
# Mon, 27 Nov 2023 11:01:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5dc2945941767d28b766b0e98aae2c27161db418c3e6dfa4323fc53ab51b8cfc`  
		Last Modified: Mon, 27 Nov 2023 11:16:06 GMT  
		Size: 27.2 MB (27193420 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:noble-20231126.1`

```console
$ docker pull ubuntu@sha256:60b647f056b54ebce877c6dfcab95f512f0b22624e94b1e1878c83e0337db45e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:noble-20231126.1` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef2b3c979842614a9537785f2dcc5e93a977fa50dc567c42a7d4f5ea6470fec0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27213697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf276bdd215773746bde9489a88d063b98584b8a650272c037da7be94941a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:09:34 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:09:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:09:35 GMT
ADD file:b2f5aa693e38f0ebe3e4d26ded8f957b4eb6f75c8360340cfcdeee25bf1b1b40 in / 
# Mon, 27 Nov 2023 11:09:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:62a1d607dcd86fd912d7d1448a129970b9c35f5506fbc48f8fea327ec9706b14`  
		Last Modified: Mon, 27 Nov 2023 11:15:40 GMT  
		Size: 27.2 MB (27213697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:noble-20231126.1` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:cef62b26f726dd229d5169a3dd6c43a6d4f779753ad0bb7ec79767612eca6d07
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26374487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a9ca3da4a89ce3b696e991e2746ef3fd43ba45e0f865e10826a5ffa412ec80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 10:59:44 GMT
ARG RELEASE
# Mon, 27 Nov 2023 10:59:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 10:59:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 10:59:44 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 10:59:45 GMT
ADD file:92c5394029d3289245a20d89db9042438c196e87f86d2c2b38ef039a94e34ea1 in / 
# Mon, 27 Nov 2023 10:59:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:280505470bcff1adb1835bdfe9c6a43d01e8f619dfc2149dfdf782f2e3586f6f`  
		Last Modified: Mon, 27 Nov 2023 11:15:48 GMT  
		Size: 26.4 MB (26374487 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:noble-20231126.1` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:7507a6b5347931e91ccbf64eccb1d47d9b1a3c8c731b370efd21fbc28c08bfb5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31316257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de3a97de9876c2336ea46851c0df7a2d9ad45c60022dfbff95d5d6e75ccefca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 10:59:52 GMT
ARG RELEASE
# Mon, 27 Nov 2023 10:59:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 10:59:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 10:59:53 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 10:59:55 GMT
ADD file:63fd35cafc829797c017809779c1ff420497005f85c88df5d033722104683537 in / 
# Mon, 27 Nov 2023 10:59:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5bb3f3c327d75c33efbc824eb228df818cdf339da3fdd25997cbb0e8e84093ba`  
		Last Modified: Mon, 27 Nov 2023 11:16:00 GMT  
		Size: 31.3 MB (31316257 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:noble-20231126.1` - linux; s390x

```console
$ docker pull ubuntu@sha256:02b206da5e7735063f201ecce4b1fd4d43e2c624e9abafde928a7097cef935c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27193420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2bcb51370031c182472d927c17f5f86bb7994d65bb928427c271ffa6141f5b7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:01:31 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:01:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:01:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:01:31 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:01:33 GMT
ADD file:c05030a894e86ddc5d70ff8a2d6332f1d879fa59044c55b03f4bff46b334e1bb in / 
# Mon, 27 Nov 2023 11:01:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5dc2945941767d28b766b0e98aae2c27161db418c3e6dfa4323fc53ab51b8cfc`  
		Last Modified: Mon, 27 Nov 2023 11:16:06 GMT  
		Size: 27.2 MB (27193420 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:354b2187c7f828ffb2d7e3676139a49cc390d9a63c5f17f61d650df2b7c366bd
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:rolling` - linux; amd64

```console
$ docker pull ubuntu@sha256:8d093e0651575a6437cc4a3d561f892a345d263aeac6156ef378fe6a4ccabd4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27273553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a94112583ff9c6d0a7b67348fc3b0ee5bbf104a86a9e24585c9ad1028fd25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:54:17 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:54:19 GMT
ADD file:5430e0b4ea856c760b6e2b88e8c2cd2d49704ed2f3c53ae34c10750a608d40ec in / 
# Thu, 30 Nov 2023 17:54:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:767829bcf202e4fa7e777f29d390307e29ac437f131685a1ff1293d44705ca23`  
		Last Modified: Thu, 30 Nov 2023 18:06:39 GMT  
		Size: 27.3 MB (27273553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2a465a4c4831c57977b6646e481f504061294f1bf1ae1b99fb5d93c67b8a471a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25201383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc753c284b47a7a5ff3ec2e926551ba95dc6c9072415649cb13a9cdff503dc04`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8761b0d436cd2e1ff47496b7cc353cf0b49347ffc92b070c31a5cf5431041614`  
		Last Modified: Wed, 11 Oct 2023 18:18:00 GMT  
		Size: 25.2 MB (25201383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:694c2aa053066101c5f29e909d4baaea478ac50e499d452f510c10e961ebb42f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26391312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382e20053971e462c74b86d6dd56f440693ddf596f0fb4989a9ef87ffb1bd5a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:41:07 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:41:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:41:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:41:07 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:41:09 GMT
ADD file:973e000ef2f95dfa48695815ebd7027db718c9fe80260271e43ee06fddfd073b in / 
# Thu, 30 Nov 2023 17:41:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b227d7805fb6cba5d091f0565054ae9ed1e13a6e2df91de4cfb41f70e208da31`  
		Last Modified: Thu, 30 Nov 2023 18:06:46 GMT  
		Size: 26.4 MB (26391312 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:22c4449e6ef2d40adecaf8ecc4df1bd80a701c12f89f29f15245189cd3da22b1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31346558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eab81e5b01a3726fd0cdbe70cf8d42317086e71ef61ad68667b29af27db455b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:57:33 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:57:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:57:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:57:34 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:57:37 GMT
ADD file:d08e45288fbc31570a3a92ae480bf6ac3ed8e4900b3260d56a51ce024818b6fe in / 
# Thu, 30 Nov 2023 17:57:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:86fa66fe8d0305c6369ae9bf03d1677c1d99b5cefbef6dd550617a300956d5b6`  
		Last Modified: Thu, 30 Nov 2023 18:06:59 GMT  
		Size: 31.3 MB (31346558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:f9bd1296086163c80f76427fb987a4ecf6799b490c724fc0bea92e66d60620cf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27094013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4bd2cee374af30258d9d818b2ef084ef72674c8a1304bc94b177dc70da33166`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:42:50 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:42:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:42:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:42:51 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:42:53 GMT
ADD file:63283c7c5d335fa063fe3da82fa78d45ed5af9327a2d154bad18a8711485db77 in / 
# Thu, 30 Nov 2023 17:42:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5ab01e9ae41fd34fc412118be6d5e21f82290394cf86ba09cd54207fa341e2d9`  
		Last Modified: Thu, 30 Nov 2023 18:07:13 GMT  
		Size: 27.1 MB (27094013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
