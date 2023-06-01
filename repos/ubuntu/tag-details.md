<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:18.04`](#ubuntu1804)
-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:22.04`](#ubuntu2204)
-	[`ubuntu:22.10`](#ubuntu2210)
-	[`ubuntu:23.04`](#ubuntu2304)
-	[`ubuntu:23.10`](#ubuntu2310)
-	[`ubuntu:bionic`](#ubuntubionic)
-	[`ubuntu:bionic-20230530`](#ubuntubionic-20230530)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20230412`](#ubuntufocal-20230412)
-	[`ubuntu:jammy`](#ubuntujammy)
-	[`ubuntu:jammy-20230522`](#ubuntujammy-20230522)
-	[`ubuntu:kinetic`](#ubuntukinetic)
-	[`ubuntu:kinetic-20230412`](#ubuntukinetic-20230412)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:lunar`](#ubuntulunar)
-	[`ubuntu:lunar-20230522`](#ubuntulunar-20230522)
-	[`ubuntu:mantic`](#ubuntumantic)
-	[`ubuntu:mantic-20230520`](#ubuntumantic-20230520)
-	[`ubuntu:rolling`](#ubunturolling)

## `ubuntu:18.04`

```console
$ docker pull ubuntu@sha256:14f1045816502e16fcbfc0b2a76747e9f5e40bc3899f8cfe20745abaafeaeab3
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:18.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:ffa418d98d4c763f2cba0d3b37e741c3d8b20dc6b60267e952e83fa466c83e9e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25689788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ba4bbc97fcec201c950799697650b5cd8e5de150322c4ec76e74e79f32522a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4e43cebf9258af1a3b1edd74432c71dcb190dea879f69291328e63a25dbf46b9`  
		Last Modified: Fri, 12 May 2023 10:04:36 GMT  
		Size: 25.7 MB (25689788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:18.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2852f36559cee4a83bf2a5102d91bde01826c2516fb9e78f3981775acf381292
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21397046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681870535343e99c778a531dd39e84779dbe994a1fe2c25861c52b492821046a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:03f27c2d942e1a5d45465a03e3dd48a5780a2267320eb05cf2a20a24315311d7`  
		Last Modified: Fri, 12 May 2023 10:04:49 GMT  
		Size: 21.4 MB (21397046 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:18.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:0723751a9fa8136b2eae5480865da9f5297dd3d33de90fef6a6ed1327e24e93c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22714573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9975d13233dc73c02ceeefb268a50537275756a8d449d57a953e23d75f3ba97c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:eade1387e79d6054aabd28e61e19e7f508c8b90dbfb315efd786c4bbf9105b82`  
		Last Modified: Fri, 12 May 2023 10:04:42 GMT  
		Size: 22.7 MB (22714573 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:18.04` - linux; 386

```console
$ docker pull ubuntu@sha256:6aff964c02b698a6b9a1f56d5a4f53a05d058156c90b21eb13f1d19ad6fe5a48
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26100600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c538b40d4e71fe0c64743ec5b5b6ee01c6bfb4bc066487fbbd612c6b55a72563`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:24:44 GMT
ARG RELEASE
# Fri, 12 May 2023 09:24:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:24:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:24:44 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:24:46 GMT
ADD file:400a181ec702fbfed9b51deb54f6c139365447e930201358981e10d21f6b672a in / 
# Fri, 12 May 2023 09:24:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1014939f0ab9331b59103a726ba635761885039c8e1224d8758703cb908c4535`  
		Last Modified: Fri, 12 May 2023 10:04:55 GMT  
		Size: 26.1 MB (26100600 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:18.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:a2ce16414f3148bd5374101b0eff84010b1b3a88125128574f12bb91d9443352
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29349033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:911c59e5d7f84bb1095d381c4097fcff5263242798611c0e244d53c8df470a94`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:21 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:21 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:23 GMT
ADD file:362fa5164fb227e6f3d45a41742ca485fc50dde3cfdc3fdc1f9233011d3d1b84 in / 
# Fri, 12 May 2023 09:26:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7160f00a7fc40c6d0afc65058cd21aed4420e3159a62aa78ac2e008c8719469e`  
		Last Modified: Fri, 12 May 2023 10:05:01 GMT  
		Size: 29.3 MB (29349033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:18.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:815ada59be008836670b1f63c1e828498f88b816bd474327a4ec07445a464a4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.7 MB (24749748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:160d661e1d9a24ed6f7968ea2da9b60bfa148a2176a853098bc0bf829315387d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:12 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:13 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:14 GMT
ADD file:8abaf7bef475e944e369ee2369d14001ea58594579438de5aa0e2fa72e805c72 in / 
# Fri, 12 May 2023 09:26:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a12e7cfb7944cd543eb7d5ad191ce8ad1dc586d5d5f66cc3d3a5a84ebcc5488b`  
		Last Modified: Fri, 12 May 2023 10:05:07 GMT  
		Size: 24.7 MB (24749748 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:db8bf6f4fb351aa7a26e27ba2686cf35a6a409f65603e59d4c203e58387dc6b3
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
$ docker pull ubuntu@sha256:b795f8e0caaaacad9859a9a38fe1c78154f8301fdaf0872eaf1520d66d9c0b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27504674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88bd6891718934e63638d9ca0ecee018e69b638270fe04990a310e5c78ab4a92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ca1778b6935686ad781c27472c4668fc61ec3aeb85494f72deb1921892b9d39e`  
		Last Modified: Thu, 13 Apr 2023 13:45:57 GMT  
		Size: 27.5 MB (27504674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:6de8d817428e3d064da83ce59b4dccf7c6749aa60b36a17ad6cc3b1f7d10123c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23609760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86b1180d68d3d67c103b16d57b364242467c2eacbbe69a9ddc04dcf1cf801d75`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:39f91c5e27647c786293528ceed473da81ca1f8e8a07bd92474a6d695bad1e22`  
		Last Modified: Thu, 13 Apr 2023 13:46:09 GMT  
		Size: 23.6 MB (23609760 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:144e6a778925a0c11c4cd9fe5fce1172e620f215b0410bb43e7fa41bbcfe4522
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25972971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:758cd4ebb2178eb0cd2ce78dea8ffad569f5bba415c4b33b694e891e7697e854`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8659cf1709ef03be2c0b2dc339b19432bff8a0753d2d7d53f47272f098f56ef4`  
		Last Modified: Thu, 13 Apr 2023 13:46:03 GMT  
		Size: 26.0 MB (25972971 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:98fcf155d7d9fe687af0af87ccbe0dcc17338686504d341cf8a731499f40cf16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32068809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3bd2848d7eadab46995f05c8e09edecfc3845d61e418304136f82bb9e22601d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f161979f5cb055a8a6d3d728b7db322422139cc28b60c716d107993a794cd86c`  
		Last Modified: Thu, 13 Apr 2023 13:46:15 GMT  
		Size: 32.1 MB (32068809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:91c315263bf6ce2500fa1b15cdb916c2c7e77a2e436dafde1788b40bc3105250
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26364733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a42c37c658114d3d2893b096a54d2deab61f556eb08c89764d35cdf13faf7ce`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f4c3f72acab731ed4e440147b25e7d155c3d98eb8738b731250868ad184e54d9`  
		Last Modified: Thu, 13 Apr 2023 13:46:21 GMT  
		Size: 26.4 MB (26364733 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.04`

```console
$ docker pull ubuntu@sha256:dfd64a3b4296d8c9b62aa3309984f8620b98d87e47492599ee20739e8eb54fbf
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
$ docker pull ubuntu@sha256:ca5534a51dd04bbcebe9b23ba05f389466cf0c190f1f8f182d7eea92a9671d00
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29534634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b418d7b466ac6275a6bfcb0c86fbe4422ff6ea0af444a294f82d3bf5173ce74`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dbf6a9befcdeecbb8813406afbd62ce81394e3869d84599f19f941aa5c74f3d1`  
		Last Modified: Tue, 25 Apr 2023 18:16:55 GMT  
		Size: 29.5 MB (29534634 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2faed463fb00a57a51cc1fe0e0884d46eacac8e7784ca7a93c3e861661d3e752
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26141443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb792700b74824c2d05fca92a19eabc234d542f7dc4699bdb95b35d6fb5f795a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:36:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:36:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:36:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:36:58 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:37:01 GMT
ADD file:08f4534e90f8ffc3bdb6cf9c04b599190ea4e1d39328135a84f4ffcd614bacb4 in / 
# Tue, 25 Apr 2023 17:37:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c082b7c88a9dba576d2339a3074cb358c028fb37a204afe47144788c8a242b32`  
		Last Modified: Tue, 25 Apr 2023 18:17:07 GMT  
		Size: 26.1 MB (26141443 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:6f8fe7bff0bee25c481cdc26e28bba984ebf72e6152005c18e1036983c01a28b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27349920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5ef9003cefb5e93a3fb4d9f175527a6751dd2f18d5179cb530c29298550b92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:79d0ea7dc1a848165a31e288cada1fa51dcd9bf302a305fe83a353c5c407110b`  
		Last Modified: Tue, 25 Apr 2023 18:17:01 GMT  
		Size: 27.3 MB (27349920 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:93fbac516e3f64e076e953306215d0a05e691e8350bf7c2e6b600ed2678990e5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34594820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048699846e4395b96648953c996e16964162e51473be900161346bb6ee97a45b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:680addf267238cca0a5d13b4eb4be2f06465f4b0f7865751e1109069a1971f46`  
		Last Modified: Tue, 25 Apr 2023 18:17:14 GMT  
		Size: 34.6 MB (34594820 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:6f86459a9bb50cb27768ad53ba78d6f02612bbf7f1efeb513569bd2160c76834
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28017013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa44e363572ab7e275bd5517e384c3e0e9e0f0d69e926aa68e85eaafc35e1373`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:44:52 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:44:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:44:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:44:52 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:44:54 GMT
ADD file:bbc65a9f059dc165e33f9a25ffaa40aab1a1f65164198a44394ec3065c82ae21 in / 
# Tue, 25 Apr 2023 17:44:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:27be50396e3447f2e65a022e1d493eb54352cd28760269836b6a06f99639e4cf`  
		Last Modified: Tue, 25 Apr 2023 18:17:20 GMT  
		Size: 28.0 MB (28017013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.10`

```console
$ docker pull ubuntu@sha256:a9a425d086dbb34c1b5b99765596e2a3cc79b33826866c51cd4508d8eb327d2b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:22.10` - linux; amd64

```console
$ docker pull ubuntu@sha256:d69f6ed3c483abe6ed19d7310acacd14012fd62874ea98edccddf6ac7af3ce93
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26695202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15f05d8742509cfc142f79dfe4cc2fa4e1b7bd20415675f7b52d3e22fd53670`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:03:38 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:03:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:03:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:03:38 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:03:39 GMT
ADD file:ba742ddbebcc8282f5094275969bfb2ff4b2973e385c198b6897bea2a9cb4b85 in / 
# Thu, 13 Apr 2023 13:03:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0963d61c5d36e157f4d244438f1a5213d8590b724d49300d6df8ebf5d70342a9`  
		Last Modified: Fri, 14 Apr 2023 11:09:15 GMT  
		Size: 26.7 MB (26695202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:9afa28d1eb80d78129debbef52b3f2a59b19479b2c15f01d16c2beeccd72dc10
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25067534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3781448a65e540dff394a6ae765d032b6c5fee3e0bc008f323330bd44a5aa797`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:51 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:52 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:10:01 GMT
ADD file:7c943de57b75e515f072a13706b12ee97f17d22a120991f8effbc0615c544253 in / 
# Thu, 13 Apr 2023 13:10:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:049083b382db595e625c4760cee04d50fb6110bda597a3dd936406027ce01994`  
		Last Modified: Fri, 14 Apr 2023 11:09:28 GMT  
		Size: 25.1 MB (25067534 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:9ff03c2930fce7e915f3b321c6c601380ffb845140bd36715c44ec31d7ae551e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25759013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490b20d4c90f834abcf386620a8906d21821aaa4db91c4665016883f043a10e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:37 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:37 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:20:38 GMT
ADD file:8b5c9a166ff42d52b423d188428558ea2bf225c42aeb3de339514e6ad9fdd504 in / 
# Thu, 13 Apr 2023 13:20:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4bb7992c0b6c454d95752fadeb8ec30f02376e386e2dbcde466ab9e74283ed78`  
		Last Modified: Fri, 14 Apr 2023 11:09:21 GMT  
		Size: 25.8 MB (25759013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:56185868328c6dcfff4b9f97915a8868905668fa8ffab0b2b0285dac1dfd84cf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31113926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaa908635f261aa7b8aa52c329990cdc01c4716fdac960a6f3cfff6706f2b56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:21:42 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:21:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:21:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:21:43 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:21:45 GMT
ADD file:2f24914c3a2e66342aa7cf589af143b01a1cd7532c92c4263d251fb826b8b810 in / 
# Thu, 13 Apr 2023 13:21:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c6864d2efca45377dbba7535ab73bb2a64f10d73c7d97bfbd768b173970bf455`  
		Last Modified: Fri, 14 Apr 2023 11:09:34 GMT  
		Size: 31.1 MB (31113926 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:3761fb8cb1cfa0facc994bb50e559e50144c999ff6ac5a43712396f98dd92045
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25488667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1d1b46d5d955e3fbe7be0da291db9a566b03ebbac3335bca37d70d66078e9a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:08:08 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:08:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:08:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:08:08 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:08:09 GMT
ADD file:df5733230d0258ecd0cbdcc7c2075865bc335200f2cafee8dacccfd082710b96 in / 
# Thu, 13 Apr 2023 13:08:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:91664c4b18004c964fd7a8e4cc1d53adb98ce8158f5d0dde54befa1c1f754635`  
		Last Modified: Fri, 14 Apr 2023 11:09:40 GMT  
		Size: 25.5 MB (25488667 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.04`

```console
$ docker pull ubuntu@sha256:db2764b64a490a9ce44a7ce0c7ba7cc6d0472c8c44684960dbca7a06525eb597
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
$ docker pull ubuntu@sha256:ce7f6664be1081be78dfcf319cb11d7bceeef17b32df373282a66fe940e47f6d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26825231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0120ea4307c597784895e9f539a67d88239d2c71ebfa830195fa2a650e4f3b5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:20:41 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:20:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:20:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:20:41 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:20:43 GMT
ADD file:6652bceb064b5b28324fcb2db853ca272d29914a5b10e6c33ef0fd824018efa0 in / 
# Thu, 20 Apr 2023 18:20:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cc1fe050fbd8eee8b0e2ef684c783d2c269fb7f61a0df0dee4639340bf612925`  
		Last Modified: Thu, 20 Apr 2023 18:59:08 GMT  
		Size: 26.8 MB (26825231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2d379e00f7bf822cf2133d5f353ef6a5e4621a2c34334f99d800bb6440b0e97a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24632909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abdc4400067184574d122f092a66f0f8d2ed3d785bb9cbd8be35a0093b594151`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:20:52 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:20:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:20:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:20:52 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:20:55 GMT
ADD file:61209c58d1b634acf67890d77ce3b799ba77b810241b26943e2a3e9b59328216 in / 
# Thu, 20 Apr 2023 18:20:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:604aa9b61f196d7ae0abd17a6d697aeab5a916fb6500d6887e59a05d362a1a06`  
		Last Modified: Thu, 20 Apr 2023 18:59:21 GMT  
		Size: 24.6 MB (24632909 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:e73844b55fb1ba94e595d64538acfcc1c4840b750f967ce368d91a51fa5007ee
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26079115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6513df0534cf35764514504f883f2163eb1bda7be89a511cad89c8c7d38b2626`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:23:18 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:23:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:23:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:23:19 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:23:26 GMT
ADD file:c9e694041e535b8a119a8dd2c03795193f66cbbcceb27694bfdae2411765e386 in / 
# Thu, 20 Apr 2023 18:23:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0da974cf49e20cf8a8d93e9fda8598c48fbe9736275600c0efafa363ab592eb2`  
		Last Modified: Thu, 20 Apr 2023 18:59:15 GMT  
		Size: 26.1 MB (26079115 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:2089e70e7b8920b03336e193bc9033456b915b5b8c4121560c7a3da7d30099d3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31018578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad251fd919f54dab755c74649e0840aaa3f64b540f00b79db2980bf4cff7fc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:20:26 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:20:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:20:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:20:26 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:20:29 GMT
ADD file:8d28b8fff20cf3ef8af5805d942e8aa5d19026e5ee01beb77e5863eb33637893 in / 
# Thu, 20 Apr 2023 18:20:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:441a86ac5a883ce4ca690a47f648f87bc8b93a71f7142dabb2c24c577ca5927b`  
		Last Modified: Thu, 20 Apr 2023 18:59:27 GMT  
		Size: 31.0 MB (31018578 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:d4cede9f231a2ccae7481724b428d8ba496cfea01e5f4e4229fe92283851d15c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25706020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03e420e560be9d01dfa32aaaade4fbf8062261fdde810eca6c4ec0e13dd411`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:21:08 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:21:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:21:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:21:08 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:21:10 GMT
ADD file:96d7710293ddafe0813d47d0fbeae45dc31a20c6115c489702cab4d2352d48bd in / 
# Thu, 20 Apr 2023 18:21:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:99b4daa0c7842dc58f7f322faa32fd0ecc93065e8815d65f3c296b7e9ea970cb`  
		Last Modified: Thu, 20 Apr 2023 18:59:34 GMT  
		Size: 25.7 MB (25706020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.10`

```console
$ docker pull ubuntu@sha256:fc60884034bc6c05862dbcfd55875c6dccd0114ebdb908f56ea7645e978373db
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
$ docker pull ubuntu@sha256:3853398d8cefdc1c02ca82cd809ab3ab3851728da0de68325389b7e53eb26acd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26836996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7706838f5f6178dc1fe5361e5f015d4f417d74921ee28ee5e2ef8abc8cc287e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:44:41 GMT
ARG RELEASE
# Tue, 09 May 2023 12:44:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:44:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:44:42 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:44:44 GMT
ADD file:f074265119093d25dbd3022b9335bcff83e7bd893a43de3f4c62e7b9f86f3180 in / 
# Tue, 09 May 2023 12:44:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:564b6a27159f34f1a7bebb7b6243b7eb326fd1752abce676bacf0b5f188af853`  
		Last Modified: Tue, 09 May 2023 14:44:37 GMT  
		Size: 26.8 MB (26836996 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2be07c22bde62369222d227a95ba36dd96effb7b98f8ff216b52567a6a702bf0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24643017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:428b69349216556102ae13c3eb318e046cd2ba25e231e18af78aa359a9d7fb72`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:44:03 GMT
ARG RELEASE
# Tue, 09 May 2023 12:44:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:44:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:44:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:44:06 GMT
ADD file:db8559cdcf696ac1fdef17e2d7eabaef48d874580294f6af72e95bae947fe358 in / 
# Tue, 09 May 2023 12:44:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec776e82e038d9043a4520f6e964ceffc2dcacf3ef14916c37efc207c2183513`  
		Last Modified: Tue, 09 May 2023 14:44:48 GMT  
		Size: 24.6 MB (24643017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:c4a4577d73dce69a7bff07d8621970b9531ab34d3b5ac18a2346b1545d469ace
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26086298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f0d7e7c16f044337f6726471eb8a478c3c5863c87bff5816f90658aed37f9b0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:45:45 GMT
ARG RELEASE
# Tue, 09 May 2023 12:45:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:45:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:45:45 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:45:53 GMT
ADD file:87293581d53f522106a37eee2d3056cd4d9bdbb4a58077389c817bd655a4e0c7 in / 
# Tue, 09 May 2023 12:45:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:49c508bd5d83e298203ae90aea0ab79d68a517dca11cd8a32feaf46f77ebe5f0`  
		Last Modified: Tue, 09 May 2023 14:44:43 GMT  
		Size: 26.1 MB (26086298 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:286d68dd3b2f3880d181ec4a94beecca844c4ad82732c8fafd8f2ac41979eb50
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31027700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644cebd854e8ec43fc628ef9f5c30b615b8e23dd1e443f286b33541214ca036c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:44:00 GMT
ARG RELEASE
# Tue, 09 May 2023 12:44:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:44:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:44:00 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:44:03 GMT
ADD file:d42dac32e11311d9b5e412834823455c0173f98c6a52bbb537a30dffb3bc872f in / 
# Tue, 09 May 2023 12:44:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b39516e102e93f59debcbceb6f11fe7ebd912108043d7cd08d376622b755a8dc`  
		Last Modified: Tue, 09 May 2023 14:44:54 GMT  
		Size: 31.0 MB (31027700 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:f82cdb2f41c19f169a156cce20b6964735b1785e14df5769f9c3fd38fa06a153
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25713103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af3ae1d5e7dee25afbe0d905cd1cb874cfb69cbe666d86ab60e4d4bd9497a57`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 13:09:19 GMT
ARG RELEASE
# Tue, 09 May 2023 13:09:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 13:09:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 13:09:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 13:09:21 GMT
ADD file:a5ed2ab846477e26003abb09795ef405e1d96bec9be1a3cb0b258dd5aa83f075 in / 
# Tue, 09 May 2023 13:09:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:259f618fdcee4b51fac02b4434116d3c9258a3663ad20b09cdea3f5c46517097`  
		Last Modified: Tue, 09 May 2023 14:45:01 GMT  
		Size: 25.7 MB (25713103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:bionic`

```console
$ docker pull ubuntu@sha256:14f1045816502e16fcbfc0b2a76747e9f5e40bc3899f8cfe20745abaafeaeab3
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic` - linux; amd64

```console
$ docker pull ubuntu@sha256:ffa418d98d4c763f2cba0d3b37e741c3d8b20dc6b60267e952e83fa466c83e9e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25689788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ba4bbc97fcec201c950799697650b5cd8e5de150322c4ec76e74e79f32522a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4e43cebf9258af1a3b1edd74432c71dcb190dea879f69291328e63a25dbf46b9`  
		Last Modified: Fri, 12 May 2023 10:04:36 GMT  
		Size: 25.7 MB (25689788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2852f36559cee4a83bf2a5102d91bde01826c2516fb9e78f3981775acf381292
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21397046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681870535343e99c778a531dd39e84779dbe994a1fe2c25861c52b492821046a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:03f27c2d942e1a5d45465a03e3dd48a5780a2267320eb05cf2a20a24315311d7`  
		Last Modified: Fri, 12 May 2023 10:04:49 GMT  
		Size: 21.4 MB (21397046 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:0723751a9fa8136b2eae5480865da9f5297dd3d33de90fef6a6ed1327e24e93c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22714573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9975d13233dc73c02ceeefb268a50537275756a8d449d57a953e23d75f3ba97c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:eade1387e79d6054aabd28e61e19e7f508c8b90dbfb315efd786c4bbf9105b82`  
		Last Modified: Fri, 12 May 2023 10:04:42 GMT  
		Size: 22.7 MB (22714573 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic` - linux; 386

```console
$ docker pull ubuntu@sha256:6aff964c02b698a6b9a1f56d5a4f53a05d058156c90b21eb13f1d19ad6fe5a48
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26100600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c538b40d4e71fe0c64743ec5b5b6ee01c6bfb4bc066487fbbd612c6b55a72563`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:24:44 GMT
ARG RELEASE
# Fri, 12 May 2023 09:24:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:24:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:24:44 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:24:46 GMT
ADD file:400a181ec702fbfed9b51deb54f6c139365447e930201358981e10d21f6b672a in / 
# Fri, 12 May 2023 09:24:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1014939f0ab9331b59103a726ba635761885039c8e1224d8758703cb908c4535`  
		Last Modified: Fri, 12 May 2023 10:04:55 GMT  
		Size: 26.1 MB (26100600 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:a2ce16414f3148bd5374101b0eff84010b1b3a88125128574f12bb91d9443352
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29349033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:911c59e5d7f84bb1095d381c4097fcff5263242798611c0e244d53c8df470a94`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:21 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:21 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:23 GMT
ADD file:362fa5164fb227e6f3d45a41742ca485fc50dde3cfdc3fdc1f9233011d3d1b84 in / 
# Fri, 12 May 2023 09:26:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7160f00a7fc40c6d0afc65058cd21aed4420e3159a62aa78ac2e008c8719469e`  
		Last Modified: Fri, 12 May 2023 10:05:01 GMT  
		Size: 29.3 MB (29349033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic` - linux; s390x

```console
$ docker pull ubuntu@sha256:815ada59be008836670b1f63c1e828498f88b816bd474327a4ec07445a464a4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.7 MB (24749748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:160d661e1d9a24ed6f7968ea2da9b60bfa148a2176a853098bc0bf829315387d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:12 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:13 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:14 GMT
ADD file:8abaf7bef475e944e369ee2369d14001ea58594579438de5aa0e2fa72e805c72 in / 
# Fri, 12 May 2023 09:26:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a12e7cfb7944cd543eb7d5ad191ce8ad1dc586d5d5f66cc3d3a5a84ebcc5488b`  
		Last Modified: Fri, 12 May 2023 10:05:07 GMT  
		Size: 24.7 MB (24749748 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:bionic-20230530`

**does not exist** (yet?)

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:fc60884034bc6c05862dbcfd55875c6dccd0114ebdb908f56ea7645e978373db
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
$ docker pull ubuntu@sha256:3853398d8cefdc1c02ca82cd809ab3ab3851728da0de68325389b7e53eb26acd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26836996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7706838f5f6178dc1fe5361e5f015d4f417d74921ee28ee5e2ef8abc8cc287e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:44:41 GMT
ARG RELEASE
# Tue, 09 May 2023 12:44:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:44:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:44:42 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:44:44 GMT
ADD file:f074265119093d25dbd3022b9335bcff83e7bd893a43de3f4c62e7b9f86f3180 in / 
# Tue, 09 May 2023 12:44:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:564b6a27159f34f1a7bebb7b6243b7eb326fd1752abce676bacf0b5f188af853`  
		Last Modified: Tue, 09 May 2023 14:44:37 GMT  
		Size: 26.8 MB (26836996 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2be07c22bde62369222d227a95ba36dd96effb7b98f8ff216b52567a6a702bf0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24643017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:428b69349216556102ae13c3eb318e046cd2ba25e231e18af78aa359a9d7fb72`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:44:03 GMT
ARG RELEASE
# Tue, 09 May 2023 12:44:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:44:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:44:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:44:06 GMT
ADD file:db8559cdcf696ac1fdef17e2d7eabaef48d874580294f6af72e95bae947fe358 in / 
# Tue, 09 May 2023 12:44:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec776e82e038d9043a4520f6e964ceffc2dcacf3ef14916c37efc207c2183513`  
		Last Modified: Tue, 09 May 2023 14:44:48 GMT  
		Size: 24.6 MB (24643017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:c4a4577d73dce69a7bff07d8621970b9531ab34d3b5ac18a2346b1545d469ace
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26086298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f0d7e7c16f044337f6726471eb8a478c3c5863c87bff5816f90658aed37f9b0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:45:45 GMT
ARG RELEASE
# Tue, 09 May 2023 12:45:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:45:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:45:45 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:45:53 GMT
ADD file:87293581d53f522106a37eee2d3056cd4d9bdbb4a58077389c817bd655a4e0c7 in / 
# Tue, 09 May 2023 12:45:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:49c508bd5d83e298203ae90aea0ab79d68a517dca11cd8a32feaf46f77ebe5f0`  
		Last Modified: Tue, 09 May 2023 14:44:43 GMT  
		Size: 26.1 MB (26086298 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:286d68dd3b2f3880d181ec4a94beecca844c4ad82732c8fafd8f2ac41979eb50
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31027700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644cebd854e8ec43fc628ef9f5c30b615b8e23dd1e443f286b33541214ca036c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:44:00 GMT
ARG RELEASE
# Tue, 09 May 2023 12:44:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:44:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:44:00 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:44:03 GMT
ADD file:d42dac32e11311d9b5e412834823455c0173f98c6a52bbb537a30dffb3bc872f in / 
# Tue, 09 May 2023 12:44:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b39516e102e93f59debcbceb6f11fe7ebd912108043d7cd08d376622b755a8dc`  
		Last Modified: Tue, 09 May 2023 14:44:54 GMT  
		Size: 31.0 MB (31027700 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:f82cdb2f41c19f169a156cce20b6964735b1785e14df5769f9c3fd38fa06a153
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25713103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af3ae1d5e7dee25afbe0d905cd1cb874cfb69cbe666d86ab60e4d4bd9497a57`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 13:09:19 GMT
ARG RELEASE
# Tue, 09 May 2023 13:09:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 13:09:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 13:09:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 13:09:21 GMT
ADD file:a5ed2ab846477e26003abb09795ef405e1d96bec9be1a3cb0b258dd5aa83f075 in / 
# Tue, 09 May 2023 13:09:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:259f618fdcee4b51fac02b4434116d3c9258a3663ad20b09cdea3f5c46517097`  
		Last Modified: Tue, 09 May 2023 14:45:01 GMT  
		Size: 25.7 MB (25713103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:db8bf6f4fb351aa7a26e27ba2686cf35a6a409f65603e59d4c203e58387dc6b3
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
$ docker pull ubuntu@sha256:b795f8e0caaaacad9859a9a38fe1c78154f8301fdaf0872eaf1520d66d9c0b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27504674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88bd6891718934e63638d9ca0ecee018e69b638270fe04990a310e5c78ab4a92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ca1778b6935686ad781c27472c4668fc61ec3aeb85494f72deb1921892b9d39e`  
		Last Modified: Thu, 13 Apr 2023 13:45:57 GMT  
		Size: 27.5 MB (27504674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:6de8d817428e3d064da83ce59b4dccf7c6749aa60b36a17ad6cc3b1f7d10123c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23609760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86b1180d68d3d67c103b16d57b364242467c2eacbbe69a9ddc04dcf1cf801d75`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:39f91c5e27647c786293528ceed473da81ca1f8e8a07bd92474a6d695bad1e22`  
		Last Modified: Thu, 13 Apr 2023 13:46:09 GMT  
		Size: 23.6 MB (23609760 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:144e6a778925a0c11c4cd9fe5fce1172e620f215b0410bb43e7fa41bbcfe4522
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25972971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:758cd4ebb2178eb0cd2ce78dea8ffad569f5bba415c4b33b694e891e7697e854`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8659cf1709ef03be2c0b2dc339b19432bff8a0753d2d7d53f47272f098f56ef4`  
		Last Modified: Thu, 13 Apr 2023 13:46:03 GMT  
		Size: 26.0 MB (25972971 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:98fcf155d7d9fe687af0af87ccbe0dcc17338686504d341cf8a731499f40cf16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32068809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3bd2848d7eadab46995f05c8e09edecfc3845d61e418304136f82bb9e22601d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f161979f5cb055a8a6d3d728b7db322422139cc28b60c716d107993a794cd86c`  
		Last Modified: Thu, 13 Apr 2023 13:46:15 GMT  
		Size: 32.1 MB (32068809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:91c315263bf6ce2500fa1b15cdb916c2c7e77a2e436dafde1788b40bc3105250
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26364733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a42c37c658114d3d2893b096a54d2deab61f556eb08c89764d35cdf13faf7ce`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f4c3f72acab731ed4e440147b25e7d155c3d98eb8738b731250868ad184e54d9`  
		Last Modified: Thu, 13 Apr 2023 13:46:21 GMT  
		Size: 26.4 MB (26364733 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal-20230412`

```console
$ docker pull ubuntu@sha256:db8bf6f4fb351aa7a26e27ba2686cf35a6a409f65603e59d4c203e58387dc6b3
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:focal-20230412` - linux; amd64

```console
$ docker pull ubuntu@sha256:b795f8e0caaaacad9859a9a38fe1c78154f8301fdaf0872eaf1520d66d9c0b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27504674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88bd6891718934e63638d9ca0ecee018e69b638270fe04990a310e5c78ab4a92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ca1778b6935686ad781c27472c4668fc61ec3aeb85494f72deb1921892b9d39e`  
		Last Modified: Thu, 13 Apr 2023 13:45:57 GMT  
		Size: 27.5 MB (27504674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230412` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:6de8d817428e3d064da83ce59b4dccf7c6749aa60b36a17ad6cc3b1f7d10123c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23609760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86b1180d68d3d67c103b16d57b364242467c2eacbbe69a9ddc04dcf1cf801d75`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:39f91c5e27647c786293528ceed473da81ca1f8e8a07bd92474a6d695bad1e22`  
		Last Modified: Thu, 13 Apr 2023 13:46:09 GMT  
		Size: 23.6 MB (23609760 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230412` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:144e6a778925a0c11c4cd9fe5fce1172e620f215b0410bb43e7fa41bbcfe4522
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25972971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:758cd4ebb2178eb0cd2ce78dea8ffad569f5bba415c4b33b694e891e7697e854`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8659cf1709ef03be2c0b2dc339b19432bff8a0753d2d7d53f47272f098f56ef4`  
		Last Modified: Thu, 13 Apr 2023 13:46:03 GMT  
		Size: 26.0 MB (25972971 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230412` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:98fcf155d7d9fe687af0af87ccbe0dcc17338686504d341cf8a731499f40cf16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32068809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3bd2848d7eadab46995f05c8e09edecfc3845d61e418304136f82bb9e22601d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f161979f5cb055a8a6d3d728b7db322422139cc28b60c716d107993a794cd86c`  
		Last Modified: Thu, 13 Apr 2023 13:46:15 GMT  
		Size: 32.1 MB (32068809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230412` - linux; s390x

```console
$ docker pull ubuntu@sha256:91c315263bf6ce2500fa1b15cdb916c2c7e77a2e436dafde1788b40bc3105250
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26364733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a42c37c658114d3d2893b096a54d2deab61f556eb08c89764d35cdf13faf7ce`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f4c3f72acab731ed4e440147b25e7d155c3d98eb8738b731250868ad184e54d9`  
		Last Modified: Thu, 13 Apr 2023 13:46:21 GMT  
		Size: 26.4 MB (26364733 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy`

```console
$ docker pull ubuntu@sha256:dfd64a3b4296d8c9b62aa3309984f8620b98d87e47492599ee20739e8eb54fbf
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
$ docker pull ubuntu@sha256:ca5534a51dd04bbcebe9b23ba05f389466cf0c190f1f8f182d7eea92a9671d00
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29534634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b418d7b466ac6275a6bfcb0c86fbe4422ff6ea0af444a294f82d3bf5173ce74`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dbf6a9befcdeecbb8813406afbd62ce81394e3869d84599f19f941aa5c74f3d1`  
		Last Modified: Tue, 25 Apr 2023 18:16:55 GMT  
		Size: 29.5 MB (29534634 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2faed463fb00a57a51cc1fe0e0884d46eacac8e7784ca7a93c3e861661d3e752
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26141443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb792700b74824c2d05fca92a19eabc234d542f7dc4699bdb95b35d6fb5f795a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:36:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:36:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:36:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:36:58 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:37:01 GMT
ADD file:08f4534e90f8ffc3bdb6cf9c04b599190ea4e1d39328135a84f4ffcd614bacb4 in / 
# Tue, 25 Apr 2023 17:37:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c082b7c88a9dba576d2339a3074cb358c028fb37a204afe47144788c8a242b32`  
		Last Modified: Tue, 25 Apr 2023 18:17:07 GMT  
		Size: 26.1 MB (26141443 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:6f8fe7bff0bee25c481cdc26e28bba984ebf72e6152005c18e1036983c01a28b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27349920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5ef9003cefb5e93a3fb4d9f175527a6751dd2f18d5179cb530c29298550b92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:79d0ea7dc1a848165a31e288cada1fa51dcd9bf302a305fe83a353c5c407110b`  
		Last Modified: Tue, 25 Apr 2023 18:17:01 GMT  
		Size: 27.3 MB (27349920 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:93fbac516e3f64e076e953306215d0a05e691e8350bf7c2e6b600ed2678990e5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34594820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048699846e4395b96648953c996e16964162e51473be900161346bb6ee97a45b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:680addf267238cca0a5d13b4eb4be2f06465f4b0f7865751e1109069a1971f46`  
		Last Modified: Tue, 25 Apr 2023 18:17:14 GMT  
		Size: 34.6 MB (34594820 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; s390x

```console
$ docker pull ubuntu@sha256:6f86459a9bb50cb27768ad53ba78d6f02612bbf7f1efeb513569bd2160c76834
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28017013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa44e363572ab7e275bd5517e384c3e0e9e0f0d69e926aa68e85eaafc35e1373`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:44:52 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:44:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:44:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:44:52 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:44:54 GMT
ADD file:bbc65a9f059dc165e33f9a25ffaa40aab1a1f65164198a44394ec3065c82ae21 in / 
# Tue, 25 Apr 2023 17:44:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:27be50396e3447f2e65a022e1d493eb54352cd28760269836b6a06f99639e4cf`  
		Last Modified: Tue, 25 Apr 2023 18:17:20 GMT  
		Size: 28.0 MB (28017013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy-20230522`

**does not exist** (yet?)

## `ubuntu:kinetic`

```console
$ docker pull ubuntu@sha256:a9a425d086dbb34c1b5b99765596e2a3cc79b33826866c51cd4508d8eb327d2b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:kinetic` - linux; amd64

```console
$ docker pull ubuntu@sha256:d69f6ed3c483abe6ed19d7310acacd14012fd62874ea98edccddf6ac7af3ce93
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26695202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15f05d8742509cfc142f79dfe4cc2fa4e1b7bd20415675f7b52d3e22fd53670`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:03:38 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:03:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:03:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:03:38 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:03:39 GMT
ADD file:ba742ddbebcc8282f5094275969bfb2ff4b2973e385c198b6897bea2a9cb4b85 in / 
# Thu, 13 Apr 2023 13:03:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0963d61c5d36e157f4d244438f1a5213d8590b724d49300d6df8ebf5d70342a9`  
		Last Modified: Fri, 14 Apr 2023 11:09:15 GMT  
		Size: 26.7 MB (26695202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:9afa28d1eb80d78129debbef52b3f2a59b19479b2c15f01d16c2beeccd72dc10
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25067534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3781448a65e540dff394a6ae765d032b6c5fee3e0bc008f323330bd44a5aa797`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:51 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:52 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:10:01 GMT
ADD file:7c943de57b75e515f072a13706b12ee97f17d22a120991f8effbc0615c544253 in / 
# Thu, 13 Apr 2023 13:10:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:049083b382db595e625c4760cee04d50fb6110bda597a3dd936406027ce01994`  
		Last Modified: Fri, 14 Apr 2023 11:09:28 GMT  
		Size: 25.1 MB (25067534 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:9ff03c2930fce7e915f3b321c6c601380ffb845140bd36715c44ec31d7ae551e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25759013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490b20d4c90f834abcf386620a8906d21821aaa4db91c4665016883f043a10e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:37 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:37 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:20:38 GMT
ADD file:8b5c9a166ff42d52b423d188428558ea2bf225c42aeb3de339514e6ad9fdd504 in / 
# Thu, 13 Apr 2023 13:20:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4bb7992c0b6c454d95752fadeb8ec30f02376e386e2dbcde466ab9e74283ed78`  
		Last Modified: Fri, 14 Apr 2023 11:09:21 GMT  
		Size: 25.8 MB (25759013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:56185868328c6dcfff4b9f97915a8868905668fa8ffab0b2b0285dac1dfd84cf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31113926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaa908635f261aa7b8aa52c329990cdc01c4716fdac960a6f3cfff6706f2b56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:21:42 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:21:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:21:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:21:43 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:21:45 GMT
ADD file:2f24914c3a2e66342aa7cf589af143b01a1cd7532c92c4263d251fb826b8b810 in / 
# Thu, 13 Apr 2023 13:21:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c6864d2efca45377dbba7535ab73bb2a64f10d73c7d97bfbd768b173970bf455`  
		Last Modified: Fri, 14 Apr 2023 11:09:34 GMT  
		Size: 31.1 MB (31113926 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; s390x

```console
$ docker pull ubuntu@sha256:3761fb8cb1cfa0facc994bb50e559e50144c999ff6ac5a43712396f98dd92045
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25488667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1d1b46d5d955e3fbe7be0da291db9a566b03ebbac3335bca37d70d66078e9a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:08:08 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:08:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:08:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:08:08 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:08:09 GMT
ADD file:df5733230d0258ecd0cbdcc7c2075865bc335200f2cafee8dacccfd082710b96 in / 
# Thu, 13 Apr 2023 13:08:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:91664c4b18004c964fd7a8e4cc1d53adb98ce8158f5d0dde54befa1c1f754635`  
		Last Modified: Fri, 14 Apr 2023 11:09:40 GMT  
		Size: 25.5 MB (25488667 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:kinetic-20230412`

```console
$ docker pull ubuntu@sha256:a9a425d086dbb34c1b5b99765596e2a3cc79b33826866c51cd4508d8eb327d2b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:kinetic-20230412` - linux; amd64

```console
$ docker pull ubuntu@sha256:d69f6ed3c483abe6ed19d7310acacd14012fd62874ea98edccddf6ac7af3ce93
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26695202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15f05d8742509cfc142f79dfe4cc2fa4e1b7bd20415675f7b52d3e22fd53670`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:03:38 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:03:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:03:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:03:38 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:03:39 GMT
ADD file:ba742ddbebcc8282f5094275969bfb2ff4b2973e385c198b6897bea2a9cb4b85 in / 
# Thu, 13 Apr 2023 13:03:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0963d61c5d36e157f4d244438f1a5213d8590b724d49300d6df8ebf5d70342a9`  
		Last Modified: Fri, 14 Apr 2023 11:09:15 GMT  
		Size: 26.7 MB (26695202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic-20230412` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:9afa28d1eb80d78129debbef52b3f2a59b19479b2c15f01d16c2beeccd72dc10
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25067534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3781448a65e540dff394a6ae765d032b6c5fee3e0bc008f323330bd44a5aa797`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:51 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:52 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:10:01 GMT
ADD file:7c943de57b75e515f072a13706b12ee97f17d22a120991f8effbc0615c544253 in / 
# Thu, 13 Apr 2023 13:10:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:049083b382db595e625c4760cee04d50fb6110bda597a3dd936406027ce01994`  
		Last Modified: Fri, 14 Apr 2023 11:09:28 GMT  
		Size: 25.1 MB (25067534 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic-20230412` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:9ff03c2930fce7e915f3b321c6c601380ffb845140bd36715c44ec31d7ae551e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25759013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490b20d4c90f834abcf386620a8906d21821aaa4db91c4665016883f043a10e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:37 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:37 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:20:38 GMT
ADD file:8b5c9a166ff42d52b423d188428558ea2bf225c42aeb3de339514e6ad9fdd504 in / 
# Thu, 13 Apr 2023 13:20:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4bb7992c0b6c454d95752fadeb8ec30f02376e386e2dbcde466ab9e74283ed78`  
		Last Modified: Fri, 14 Apr 2023 11:09:21 GMT  
		Size: 25.8 MB (25759013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic-20230412` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:56185868328c6dcfff4b9f97915a8868905668fa8ffab0b2b0285dac1dfd84cf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31113926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaa908635f261aa7b8aa52c329990cdc01c4716fdac960a6f3cfff6706f2b56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:21:42 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:21:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:21:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:21:43 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:21:45 GMT
ADD file:2f24914c3a2e66342aa7cf589af143b01a1cd7532c92c4263d251fb826b8b810 in / 
# Thu, 13 Apr 2023 13:21:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c6864d2efca45377dbba7535ab73bb2a64f10d73c7d97bfbd768b173970bf455`  
		Last Modified: Fri, 14 Apr 2023 11:09:34 GMT  
		Size: 31.1 MB (31113926 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic-20230412` - linux; s390x

```console
$ docker pull ubuntu@sha256:3761fb8cb1cfa0facc994bb50e559e50144c999ff6ac5a43712396f98dd92045
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25488667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1d1b46d5d955e3fbe7be0da291db9a566b03ebbac3335bca37d70d66078e9a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:08:08 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:08:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:08:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:08:08 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:08:09 GMT
ADD file:df5733230d0258ecd0cbdcc7c2075865bc335200f2cafee8dacccfd082710b96 in / 
# Thu, 13 Apr 2023 13:08:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:91664c4b18004c964fd7a8e4cc1d53adb98ce8158f5d0dde54befa1c1f754635`  
		Last Modified: Fri, 14 Apr 2023 11:09:40 GMT  
		Size: 25.5 MB (25488667 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:dfd64a3b4296d8c9b62aa3309984f8620b98d87e47492599ee20739e8eb54fbf
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
$ docker pull ubuntu@sha256:ca5534a51dd04bbcebe9b23ba05f389466cf0c190f1f8f182d7eea92a9671d00
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29534634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b418d7b466ac6275a6bfcb0c86fbe4422ff6ea0af444a294f82d3bf5173ce74`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dbf6a9befcdeecbb8813406afbd62ce81394e3869d84599f19f941aa5c74f3d1`  
		Last Modified: Tue, 25 Apr 2023 18:16:55 GMT  
		Size: 29.5 MB (29534634 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2faed463fb00a57a51cc1fe0e0884d46eacac8e7784ca7a93c3e861661d3e752
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26141443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb792700b74824c2d05fca92a19eabc234d542f7dc4699bdb95b35d6fb5f795a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:36:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:36:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:36:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:36:58 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:37:01 GMT
ADD file:08f4534e90f8ffc3bdb6cf9c04b599190ea4e1d39328135a84f4ffcd614bacb4 in / 
# Tue, 25 Apr 2023 17:37:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c082b7c88a9dba576d2339a3074cb358c028fb37a204afe47144788c8a242b32`  
		Last Modified: Tue, 25 Apr 2023 18:17:07 GMT  
		Size: 26.1 MB (26141443 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:6f8fe7bff0bee25c481cdc26e28bba984ebf72e6152005c18e1036983c01a28b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27349920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5ef9003cefb5e93a3fb4d9f175527a6751dd2f18d5179cb530c29298550b92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:79d0ea7dc1a848165a31e288cada1fa51dcd9bf302a305fe83a353c5c407110b`  
		Last Modified: Tue, 25 Apr 2023 18:17:01 GMT  
		Size: 27.3 MB (27349920 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:93fbac516e3f64e076e953306215d0a05e691e8350bf7c2e6b600ed2678990e5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34594820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048699846e4395b96648953c996e16964162e51473be900161346bb6ee97a45b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:680addf267238cca0a5d13b4eb4be2f06465f4b0f7865751e1109069a1971f46`  
		Last Modified: Tue, 25 Apr 2023 18:17:14 GMT  
		Size: 34.6 MB (34594820 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:6f86459a9bb50cb27768ad53ba78d6f02612bbf7f1efeb513569bd2160c76834
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28017013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa44e363572ab7e275bd5517e384c3e0e9e0f0d69e926aa68e85eaafc35e1373`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:44:52 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:44:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:44:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:44:52 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:44:54 GMT
ADD file:bbc65a9f059dc165e33f9a25ffaa40aab1a1f65164198a44394ec3065c82ae21 in / 
# Tue, 25 Apr 2023 17:44:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:27be50396e3447f2e65a022e1d493eb54352cd28760269836b6a06f99639e4cf`  
		Last Modified: Tue, 25 Apr 2023 18:17:20 GMT  
		Size: 28.0 MB (28017013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar`

```console
$ docker pull ubuntu@sha256:db2764b64a490a9ce44a7ce0c7ba7cc6d0472c8c44684960dbca7a06525eb597
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
$ docker pull ubuntu@sha256:ce7f6664be1081be78dfcf319cb11d7bceeef17b32df373282a66fe940e47f6d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26825231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0120ea4307c597784895e9f539a67d88239d2c71ebfa830195fa2a650e4f3b5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:20:41 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:20:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:20:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:20:41 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:20:43 GMT
ADD file:6652bceb064b5b28324fcb2db853ca272d29914a5b10e6c33ef0fd824018efa0 in / 
# Thu, 20 Apr 2023 18:20:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cc1fe050fbd8eee8b0e2ef684c783d2c269fb7f61a0df0dee4639340bf612925`  
		Last Modified: Thu, 20 Apr 2023 18:59:08 GMT  
		Size: 26.8 MB (26825231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2d379e00f7bf822cf2133d5f353ef6a5e4621a2c34334f99d800bb6440b0e97a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24632909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abdc4400067184574d122f092a66f0f8d2ed3d785bb9cbd8be35a0093b594151`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:20:52 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:20:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:20:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:20:52 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:20:55 GMT
ADD file:61209c58d1b634acf67890d77ce3b799ba77b810241b26943e2a3e9b59328216 in / 
# Thu, 20 Apr 2023 18:20:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:604aa9b61f196d7ae0abd17a6d697aeab5a916fb6500d6887e59a05d362a1a06`  
		Last Modified: Thu, 20 Apr 2023 18:59:21 GMT  
		Size: 24.6 MB (24632909 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:e73844b55fb1ba94e595d64538acfcc1c4840b750f967ce368d91a51fa5007ee
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26079115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6513df0534cf35764514504f883f2163eb1bda7be89a511cad89c8c7d38b2626`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:23:18 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:23:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:23:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:23:19 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:23:26 GMT
ADD file:c9e694041e535b8a119a8dd2c03795193f66cbbcceb27694bfdae2411765e386 in / 
# Thu, 20 Apr 2023 18:23:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0da974cf49e20cf8a8d93e9fda8598c48fbe9736275600c0efafa363ab592eb2`  
		Last Modified: Thu, 20 Apr 2023 18:59:15 GMT  
		Size: 26.1 MB (26079115 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:2089e70e7b8920b03336e193bc9033456b915b5b8c4121560c7a3da7d30099d3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31018578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad251fd919f54dab755c74649e0840aaa3f64b540f00b79db2980bf4cff7fc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:20:26 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:20:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:20:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:20:26 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:20:29 GMT
ADD file:8d28b8fff20cf3ef8af5805d942e8aa5d19026e5ee01beb77e5863eb33637893 in / 
# Thu, 20 Apr 2023 18:20:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:441a86ac5a883ce4ca690a47f648f87bc8b93a71f7142dabb2c24c577ca5927b`  
		Last Modified: Thu, 20 Apr 2023 18:59:27 GMT  
		Size: 31.0 MB (31018578 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; s390x

```console
$ docker pull ubuntu@sha256:d4cede9f231a2ccae7481724b428d8ba496cfea01e5f4e4229fe92283851d15c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25706020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03e420e560be9d01dfa32aaaade4fbf8062261fdde810eca6c4ec0e13dd411`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:21:08 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:21:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:21:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:21:08 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:21:10 GMT
ADD file:96d7710293ddafe0813d47d0fbeae45dc31a20c6115c489702cab4d2352d48bd in / 
# Thu, 20 Apr 2023 18:21:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:99b4daa0c7842dc58f7f322faa32fd0ecc93065e8815d65f3c296b7e9ea970cb`  
		Last Modified: Thu, 20 Apr 2023 18:59:34 GMT  
		Size: 25.7 MB (25706020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar-20230522`

**does not exist** (yet?)

## `ubuntu:mantic`

```console
$ docker pull ubuntu@sha256:fc60884034bc6c05862dbcfd55875c6dccd0114ebdb908f56ea7645e978373db
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
$ docker pull ubuntu@sha256:3853398d8cefdc1c02ca82cd809ab3ab3851728da0de68325389b7e53eb26acd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26836996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7706838f5f6178dc1fe5361e5f015d4f417d74921ee28ee5e2ef8abc8cc287e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:44:41 GMT
ARG RELEASE
# Tue, 09 May 2023 12:44:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:44:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:44:42 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:44:44 GMT
ADD file:f074265119093d25dbd3022b9335bcff83e7bd893a43de3f4c62e7b9f86f3180 in / 
# Tue, 09 May 2023 12:44:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:564b6a27159f34f1a7bebb7b6243b7eb326fd1752abce676bacf0b5f188af853`  
		Last Modified: Tue, 09 May 2023 14:44:37 GMT  
		Size: 26.8 MB (26836996 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2be07c22bde62369222d227a95ba36dd96effb7b98f8ff216b52567a6a702bf0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24643017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:428b69349216556102ae13c3eb318e046cd2ba25e231e18af78aa359a9d7fb72`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:44:03 GMT
ARG RELEASE
# Tue, 09 May 2023 12:44:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:44:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:44:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:44:06 GMT
ADD file:db8559cdcf696ac1fdef17e2d7eabaef48d874580294f6af72e95bae947fe358 in / 
# Tue, 09 May 2023 12:44:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec776e82e038d9043a4520f6e964ceffc2dcacf3ef14916c37efc207c2183513`  
		Last Modified: Tue, 09 May 2023 14:44:48 GMT  
		Size: 24.6 MB (24643017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:c4a4577d73dce69a7bff07d8621970b9531ab34d3b5ac18a2346b1545d469ace
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26086298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f0d7e7c16f044337f6726471eb8a478c3c5863c87bff5816f90658aed37f9b0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:45:45 GMT
ARG RELEASE
# Tue, 09 May 2023 12:45:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:45:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:45:45 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:45:53 GMT
ADD file:87293581d53f522106a37eee2d3056cd4d9bdbb4a58077389c817bd655a4e0c7 in / 
# Tue, 09 May 2023 12:45:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:49c508bd5d83e298203ae90aea0ab79d68a517dca11cd8a32feaf46f77ebe5f0`  
		Last Modified: Tue, 09 May 2023 14:44:43 GMT  
		Size: 26.1 MB (26086298 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:286d68dd3b2f3880d181ec4a94beecca844c4ad82732c8fafd8f2ac41979eb50
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31027700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644cebd854e8ec43fc628ef9f5c30b615b8e23dd1e443f286b33541214ca036c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 12:44:00 GMT
ARG RELEASE
# Tue, 09 May 2023 12:44:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 12:44:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 12:44:00 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 12:44:03 GMT
ADD file:d42dac32e11311d9b5e412834823455c0173f98c6a52bbb537a30dffb3bc872f in / 
# Tue, 09 May 2023 12:44:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b39516e102e93f59debcbceb6f11fe7ebd912108043d7cd08d376622b755a8dc`  
		Last Modified: Tue, 09 May 2023 14:44:54 GMT  
		Size: 31.0 MB (31027700 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; s390x

```console
$ docker pull ubuntu@sha256:f82cdb2f41c19f169a156cce20b6964735b1785e14df5769f9c3fd38fa06a153
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25713103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af3ae1d5e7dee25afbe0d905cd1cb874cfb69cbe666d86ab60e4d4bd9497a57`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 13:09:19 GMT
ARG RELEASE
# Tue, 09 May 2023 13:09:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 09 May 2023 13:09:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 09 May 2023 13:09:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 09 May 2023 13:09:21 GMT
ADD file:a5ed2ab846477e26003abb09795ef405e1d96bec9be1a3cb0b258dd5aa83f075 in / 
# Tue, 09 May 2023 13:09:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:259f618fdcee4b51fac02b4434116d3c9258a3663ad20b09cdea3f5c46517097`  
		Last Modified: Tue, 09 May 2023 14:45:01 GMT  
		Size: 25.7 MB (25713103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:mantic-20230520`

**does not exist** (yet?)

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:db2764b64a490a9ce44a7ce0c7ba7cc6d0472c8c44684960dbca7a06525eb597
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
$ docker pull ubuntu@sha256:ce7f6664be1081be78dfcf319cb11d7bceeef17b32df373282a66fe940e47f6d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26825231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0120ea4307c597784895e9f539a67d88239d2c71ebfa830195fa2a650e4f3b5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:20:41 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:20:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:20:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:20:41 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:20:43 GMT
ADD file:6652bceb064b5b28324fcb2db853ca272d29914a5b10e6c33ef0fd824018efa0 in / 
# Thu, 20 Apr 2023 18:20:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cc1fe050fbd8eee8b0e2ef684c783d2c269fb7f61a0df0dee4639340bf612925`  
		Last Modified: Thu, 20 Apr 2023 18:59:08 GMT  
		Size: 26.8 MB (26825231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2d379e00f7bf822cf2133d5f353ef6a5e4621a2c34334f99d800bb6440b0e97a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24632909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abdc4400067184574d122f092a66f0f8d2ed3d785bb9cbd8be35a0093b594151`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:20:52 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:20:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:20:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:20:52 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:20:55 GMT
ADD file:61209c58d1b634acf67890d77ce3b799ba77b810241b26943e2a3e9b59328216 in / 
# Thu, 20 Apr 2023 18:20:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:604aa9b61f196d7ae0abd17a6d697aeab5a916fb6500d6887e59a05d362a1a06`  
		Last Modified: Thu, 20 Apr 2023 18:59:21 GMT  
		Size: 24.6 MB (24632909 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:e73844b55fb1ba94e595d64538acfcc1c4840b750f967ce368d91a51fa5007ee
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26079115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6513df0534cf35764514504f883f2163eb1bda7be89a511cad89c8c7d38b2626`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:23:18 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:23:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:23:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:23:19 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:23:26 GMT
ADD file:c9e694041e535b8a119a8dd2c03795193f66cbbcceb27694bfdae2411765e386 in / 
# Thu, 20 Apr 2023 18:23:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0da974cf49e20cf8a8d93e9fda8598c48fbe9736275600c0efafa363ab592eb2`  
		Last Modified: Thu, 20 Apr 2023 18:59:15 GMT  
		Size: 26.1 MB (26079115 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:2089e70e7b8920b03336e193bc9033456b915b5b8c4121560c7a3da7d30099d3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31018578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad251fd919f54dab755c74649e0840aaa3f64b540f00b79db2980bf4cff7fc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:20:26 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:20:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:20:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:20:26 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:20:29 GMT
ADD file:8d28b8fff20cf3ef8af5805d942e8aa5d19026e5ee01beb77e5863eb33637893 in / 
# Thu, 20 Apr 2023 18:20:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:441a86ac5a883ce4ca690a47f648f87bc8b93a71f7142dabb2c24c577ca5927b`  
		Last Modified: Thu, 20 Apr 2023 18:59:27 GMT  
		Size: 31.0 MB (31018578 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:d4cede9f231a2ccae7481724b428d8ba496cfea01e5f4e4229fe92283851d15c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25706020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03e420e560be9d01dfa32aaaade4fbf8062261fdde810eca6c4ec0e13dd411`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Apr 2023 18:21:08 GMT
ARG RELEASE
# Thu, 20 Apr 2023 18:21:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 20 Apr 2023 18:21:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 20 Apr 2023 18:21:08 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 20 Apr 2023 18:21:10 GMT
ADD file:96d7710293ddafe0813d47d0fbeae45dc31a20c6115c489702cab4d2352d48bd in / 
# Thu, 20 Apr 2023 18:21:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:99b4daa0c7842dc58f7f322faa32fd0ecc93065e8815d65f3c296b7e9ea970cb`  
		Last Modified: Thu, 20 Apr 2023 18:59:34 GMT  
		Size: 25.7 MB (25706020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
