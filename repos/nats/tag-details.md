<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.18`](#nats2-alpine318)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.10`](#nats210)
-	[`nats:2.10-alpine`](#nats210-alpine)
-	[`nats:2.10-alpine3.18`](#nats210-alpine318)
-	[`nats:2.10-linux`](#nats210-linux)
-	[`nats:2.10-nanoserver`](#nats210-nanoserver)
-	[`nats:2.10-nanoserver-1809`](#nats210-nanoserver-1809)
-	[`nats:2.10-scratch`](#nats210-scratch)
-	[`nats:2.10-windowsservercore`](#nats210-windowsservercore)
-	[`nats:2.10-windowsservercore-1809`](#nats210-windowsservercore-1809)
-	[`nats:2.10.6`](#nats2106)
-	[`nats:2.10.6-alpine`](#nats2106-alpine)
-	[`nats:2.10.6-alpine3.18`](#nats2106-alpine318)
-	[`nats:2.10.6-linux`](#nats2106-linux)
-	[`nats:2.10.6-nanoserver`](#nats2106-nanoserver)
-	[`nats:2.10.6-nanoserver-1809`](#nats2106-nanoserver-1809)
-	[`nats:2.10.6-scratch`](#nats2106-scratch)
-	[`nats:2.10.6-windowsservercore`](#nats2106-windowsservercore)
-	[`nats:2.10.6-windowsservercore-1809`](#nats2106-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.18`](#nats29-alpine318)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.24`](#nats2924)
-	[`nats:2.9.24-alpine`](#nats2924-alpine)
-	[`nats:2.9.24-alpine3.18`](#nats2924-alpine318)
-	[`nats:2.9.24-linux`](#nats2924-linux)
-	[`nats:2.9.24-nanoserver`](#nats2924-nanoserver)
-	[`nats:2.9.24-nanoserver-1809`](#nats2924-nanoserver-1809)
-	[`nats:2.9.24-scratch`](#nats2924-scratch)
-	[`nats:2.9.24-windowsservercore`](#nats2924-windowsservercore)
-	[`nats:2.9.24-windowsservercore-1809`](#nats2924-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.18`](#natsalpine318)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:195df15e1f52f94fd5ca9120c099d64f7ed1ced5f2f7941ed658263e5c2c7530
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.5122; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:ca5325d2a2c84eca8c4f3e3ba96a4fcf6dc91e97e3d3ebd3bae69f7a126c0e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5248367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea934ed1a17a93225092fac66c8b617c594ecec00debda4eb753479eeadedab2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:c3d82eee52a26292cc80755a2b88f8b80cef5c80fd438c99768cd1c33ca95a9d in /nats-server 
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:22:59 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:22:59 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:22:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44811b84801c95891b1ccde13fe7e76a1ffd8795cd2a066ac0630ee836c23c2e`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 5.2 MB (5247859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927d64e5da79549425963bee122f44117e41eaa442b01673188effd14c9b236`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d3ccb1b790e4433d69872d7ddb8377aac40d6f000a66fa5b2795a62122a4f54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4984842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f1a1ecd1b37c66268f966a88d26fa44b35f70909dedab19c60bfd5aca2035e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:401de119a9fad5bd89c70f5a4d5c70f110d490ae5ab9aa60a7f963686ab297ee in /nats-server 
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:49:29 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f1d2c1b6f013f4386e7235452bc47cebd8001115c3a6504b418ee5b90071492a`  
		Last Modified: Wed, 08 Nov 2023 19:50:14 GMT  
		Size: 5.0 MB (4984334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5fea0f4bcfa87853f77179e249f0a8a09723aeb1c53882e3036fa6250a4ff5`  
		Last Modified: Wed, 08 Nov 2023 19:50:13 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:c73b24d4fb1ad910ad2f2bdefe0d18bfec11431afb4da9e3cd2be176e4fd49b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4977978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfe5b4a001ee28a1308edc00242441032b2afb69148c7ba17f692f75e2c1dba`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:cd8c3bf2b10d14de1f76a0617be080153909dadcd658bb62cab16d41a650d3de in /nats-server 
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:57:47 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:57:47 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:57:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e2a0a8d03803b71ab2e1e3540de965b9430b493bbd15bb2cb1372a7dd564c76d`  
		Last Modified: Wed, 08 Nov 2023 19:58:32 GMT  
		Size: 5.0 MB (4977470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe9df0b73b8b228e9331792251ba43d36af5e4e898411b4f9b725bb8928231`  
		Last Modified: Wed, 08 Nov 2023 19:58:31 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:770e514bf6ca4d8b056bd9d16b7df5f56c45c587ce3c815515051b6588e38325
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4785043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75bc6347feea13831461567c92c52c13e9085417ef409fb74364cf63105e346`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:40:10 GMT
COPY file:209cf40c58f80a36d8d8c8060f48a598dcf03ae451d8d658f267d02f3ce7bddc in /nats-server 
# Wed, 08 Nov 2023 19:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:40:11 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:40:11 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:40:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b497fc8beff1c9fb319e3b4b62e22135e8e8d81506ede3ca51365887947a8571`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 4.8 MB (4784535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbc2e7980e0793ef96d07cc5a7d9418109519d7d6982ba49570b90d02b2932c`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:b196b3729c3c8ceb8c4b7192d7be08520dfd17c42377322a4027b889bcb61d50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:280f97fc32445b7fbf78d249c8e08a78508600838b36b8633b08eed6c8e11b4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9516956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13309d27201a23f166d402964c2bc26937570c70c1ef85ba960d3e4171b6bb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 22:22:47 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:22:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 22:22:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 22:22:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3e725fa689593464ef203de1b06f2e55491fa077b59b693fd9e1ef8c249dd`  
		Last Modified: Fri, 01 Dec 2023 22:23:35 GMT  
		Size: 6.1 MB (6113534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ede37fe98c391207efb9e57a4e29197e178cd9afdafac3140fcf8e44aecc62b`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9177007628f506dd880c66a174348504e4589a3cd156d8377b4278242ffefb9c`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f9a012265e9ab4e95584f7ea9f4f78234e048366873dcef81b1b46359e22d9f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce4db94168c70869897e9c0941e0567f3ce732d60f92f80ef605d765d9c9686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:49:22 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:49:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:49:25 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9345d2089731ee6f2e92bf32245d1665e8357fecf55c50e9a428966a109c4ed`  
		Last Modified: Fri, 01 Dec 2023 21:50:01 GMT  
		Size: 5.8 MB (5827544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569cb676c86b2aeb776ffd80a904ac5e9bdcda8bea7c0684872fba5efc4b8007`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23edb8dc9637ca24330de881d8e57e7f369ebd6b7b100db2dbae3aff15d50f29`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d6be8cbc263e2393e2d5f07d4b579c143dada13fe2dd8966097c11e9a1ddc178
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c00554cdbce58cc9a6a11ca1b37f5b90932f2c7bc9b55f096f26b93ba240a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:57:27 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:57:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:57:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8756919eccb97dc6990af357a87c8ba743e3a3ee7ad6d8c8c3dc108620e3c`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 5.8 MB (5818288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55307c3335ece26e2e60bb611f614f94af63814be706d6b3394d9691f55e7f82`  
		Last Modified: Fri, 01 Dec 2023 21:58:15 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7195a7938dcaa9bf7c4b89602950f827640c5bbecbb4a4f858b6a846f6719b`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ecd307e2f9675cf866313820a53a82b1a1459cf04a50da39b145b79360877119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9018304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e350d93fb277376b154a1cc0e44e75d36e34a479bea66c1186b2ef6ce5ec9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:39:48 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:39:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:39:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099335ae91609137f74432a77e75ffc1877279b74582260fc094104662cc3707`  
		Last Modified: Fri, 01 Dec 2023 21:40:50 GMT  
		Size: 5.7 MB (5684273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10e033372c9ea54711e4453250cd168911b0b43394e197c03164fcab8331f7`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9486420e5d0bd9ffaf1e3828a6eec84d98d97415b6fe70f65534ff451b2c61`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.18`

```console
$ docker pull nats@sha256:b196b3729c3c8ceb8c4b7192d7be08520dfd17c42377322a4027b889bcb61d50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:280f97fc32445b7fbf78d249c8e08a78508600838b36b8633b08eed6c8e11b4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9516956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13309d27201a23f166d402964c2bc26937570c70c1ef85ba960d3e4171b6bb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 22:22:47 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:22:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 22:22:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 22:22:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3e725fa689593464ef203de1b06f2e55491fa077b59b693fd9e1ef8c249dd`  
		Last Modified: Fri, 01 Dec 2023 22:23:35 GMT  
		Size: 6.1 MB (6113534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ede37fe98c391207efb9e57a4e29197e178cd9afdafac3140fcf8e44aecc62b`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9177007628f506dd880c66a174348504e4589a3cd156d8377b4278242ffefb9c`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:f9a012265e9ab4e95584f7ea9f4f78234e048366873dcef81b1b46359e22d9f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce4db94168c70869897e9c0941e0567f3ce732d60f92f80ef605d765d9c9686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:49:22 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:49:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:49:25 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9345d2089731ee6f2e92bf32245d1665e8357fecf55c50e9a428966a109c4ed`  
		Last Modified: Fri, 01 Dec 2023 21:50:01 GMT  
		Size: 5.8 MB (5827544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569cb676c86b2aeb776ffd80a904ac5e9bdcda8bea7c0684872fba5efc4b8007`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23edb8dc9637ca24330de881d8e57e7f369ebd6b7b100db2dbae3aff15d50f29`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:d6be8cbc263e2393e2d5f07d4b579c143dada13fe2dd8966097c11e9a1ddc178
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c00554cdbce58cc9a6a11ca1b37f5b90932f2c7bc9b55f096f26b93ba240a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:57:27 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:57:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:57:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8756919eccb97dc6990af357a87c8ba743e3a3ee7ad6d8c8c3dc108620e3c`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 5.8 MB (5818288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55307c3335ece26e2e60bb611f614f94af63814be706d6b3394d9691f55e7f82`  
		Last Modified: Fri, 01 Dec 2023 21:58:15 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7195a7938dcaa9bf7c4b89602950f827640c5bbecbb4a4f858b6a846f6719b`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ecd307e2f9675cf866313820a53a82b1a1459cf04a50da39b145b79360877119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9018304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e350d93fb277376b154a1cc0e44e75d36e34a479bea66c1186b2ef6ce5ec9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:39:48 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:39:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:39:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099335ae91609137f74432a77e75ffc1877279b74582260fc094104662cc3707`  
		Last Modified: Fri, 01 Dec 2023 21:40:50 GMT  
		Size: 5.7 MB (5684273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10e033372c9ea54711e4453250cd168911b0b43394e197c03164fcab8331f7`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9486420e5d0bd9ffaf1e3828a6eec84d98d97415b6fe70f65534ff451b2c61`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:87853cd90752f3d33c3a31b152a11a2b9a7736f4a736218a570495225fcbecba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:cb6e962ac8351dd9c57425e277ee4df9a1891ceb36b91f96de71bcb32e5b7f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:cb6e962ac8351dd9c57425e277ee4df9a1891ceb36b91f96de71bcb32e5b7f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:87853cd90752f3d33c3a31b152a11a2b9a7736f4a736218a570495225fcbecba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:2635baef88f485e3e6c943dab77da02ccdfbaa09a4cf45a6cade2b95132aa291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:a615001ea716034c1ae2e5cbb7989e5d4b89aa83346c9bfa2c353194009f4c2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063764344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d4d13ef10f01fd53dab0e60ac169100d104101183a8b7564de4a935c98ce88`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:15:41 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:15:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.6/nats-server-v2.10.6-windows-amd64.zip
# Fri, 01 Dec 2023 22:15:43 GMT
ENV NATS_SERVER_SHASUM=8084fc5fc16fa099fae0bb2f74dcf077ab644310918cc16e68b9909330ac798b
# Fri, 01 Dec 2023 22:16:45 GMT
RUN Set-PSDebug -Trace 2
# Fri, 01 Dec 2023 22:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 01 Dec 2023 22:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482d1334c03f2dfeab20b372b19d03e4af7be1261b4b2c858cfa969d0f17c33f`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7056bd68c3f6a5bc1bfdfe4fd9aba9d36b5fa4490e1fa5856be9a04ae3e44a`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c875fab524e257138d947d0cc33bc83d5f79ddf950d886b48f307180daa7d3`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fecdb4839d326ad445940782e3c9036f5487a2f47c185e8682652ec5e049b32`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 437.1 KB (437133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc25e0a531b65458953a005d8f1426da0383911a7e6129de254b037f7a60244b`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 5.9 MB (5882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd9cd8a4c0fd879700f6adde2f07b9c978036ed06509a537e8e9e2327d1974`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5f74a80810732f5daca2a35b749a9c1e0fc520a8fb994930694a05ae073fa2`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cac74b0b7cc9e03fb9c78c17f45ed3e4153089be3dba95e03d5230d8e6336c4`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d9d2aa7f0e9065f683eaa5fcf692b200162ecce3161afef9e766e9a332ed53`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:2635baef88f485e3e6c943dab77da02ccdfbaa09a4cf45a6cade2b95132aa291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:a615001ea716034c1ae2e5cbb7989e5d4b89aa83346c9bfa2c353194009f4c2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063764344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d4d13ef10f01fd53dab0e60ac169100d104101183a8b7564de4a935c98ce88`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:15:41 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:15:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.6/nats-server-v2.10.6-windows-amd64.zip
# Fri, 01 Dec 2023 22:15:43 GMT
ENV NATS_SERVER_SHASUM=8084fc5fc16fa099fae0bb2f74dcf077ab644310918cc16e68b9909330ac798b
# Fri, 01 Dec 2023 22:16:45 GMT
RUN Set-PSDebug -Trace 2
# Fri, 01 Dec 2023 22:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 01 Dec 2023 22:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482d1334c03f2dfeab20b372b19d03e4af7be1261b4b2c858cfa969d0f17c33f`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7056bd68c3f6a5bc1bfdfe4fd9aba9d36b5fa4490e1fa5856be9a04ae3e44a`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c875fab524e257138d947d0cc33bc83d5f79ddf950d886b48f307180daa7d3`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fecdb4839d326ad445940782e3c9036f5487a2f47c185e8682652ec5e049b32`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 437.1 KB (437133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc25e0a531b65458953a005d8f1426da0383911a7e6129de254b037f7a60244b`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 5.9 MB (5882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd9cd8a4c0fd879700f6adde2f07b9c978036ed06509a537e8e9e2327d1974`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5f74a80810732f5daca2a35b749a9c1e0fc520a8fb994930694a05ae073fa2`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cac74b0b7cc9e03fb9c78c17f45ed3e4153089be3dba95e03d5230d8e6336c4`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d9d2aa7f0e9065f683eaa5fcf692b200162ecce3161afef9e766e9a332ed53`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10`

```console
$ docker pull nats@sha256:fc3dcb7f2944c437451c9091c6fac6ca3df2a53d6dd844f14b5754eabe003e21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-alpine`

```console
$ docker pull nats@sha256:b196b3729c3c8ceb8c4b7192d7be08520dfd17c42377322a4027b889bcb61d50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-alpine` - linux; amd64

```console
$ docker pull nats@sha256:280f97fc32445b7fbf78d249c8e08a78508600838b36b8633b08eed6c8e11b4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9516956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13309d27201a23f166d402964c2bc26937570c70c1ef85ba960d3e4171b6bb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 22:22:47 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:22:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 22:22:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 22:22:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3e725fa689593464ef203de1b06f2e55491fa077b59b693fd9e1ef8c249dd`  
		Last Modified: Fri, 01 Dec 2023 22:23:35 GMT  
		Size: 6.1 MB (6113534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ede37fe98c391207efb9e57a4e29197e178cd9afdafac3140fcf8e44aecc62b`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9177007628f506dd880c66a174348504e4589a3cd156d8377b4278242ffefb9c`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f9a012265e9ab4e95584f7ea9f4f78234e048366873dcef81b1b46359e22d9f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce4db94168c70869897e9c0941e0567f3ce732d60f92f80ef605d765d9c9686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:49:22 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:49:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:49:25 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9345d2089731ee6f2e92bf32245d1665e8357fecf55c50e9a428966a109c4ed`  
		Last Modified: Fri, 01 Dec 2023 21:50:01 GMT  
		Size: 5.8 MB (5827544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569cb676c86b2aeb776ffd80a904ac5e9bdcda8bea7c0684872fba5efc4b8007`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23edb8dc9637ca24330de881d8e57e7f369ebd6b7b100db2dbae3aff15d50f29`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d6be8cbc263e2393e2d5f07d4b579c143dada13fe2dd8966097c11e9a1ddc178
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c00554cdbce58cc9a6a11ca1b37f5b90932f2c7bc9b55f096f26b93ba240a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:57:27 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:57:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:57:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8756919eccb97dc6990af357a87c8ba743e3a3ee7ad6d8c8c3dc108620e3c`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 5.8 MB (5818288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55307c3335ece26e2e60bb611f614f94af63814be706d6b3394d9691f55e7f82`  
		Last Modified: Fri, 01 Dec 2023 21:58:15 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7195a7938dcaa9bf7c4b89602950f827640c5bbecbb4a4f858b6a846f6719b`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ecd307e2f9675cf866313820a53a82b1a1459cf04a50da39b145b79360877119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9018304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e350d93fb277376b154a1cc0e44e75d36e34a479bea66c1186b2ef6ce5ec9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:39:48 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:39:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:39:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099335ae91609137f74432a77e75ffc1877279b74582260fc094104662cc3707`  
		Last Modified: Fri, 01 Dec 2023 21:40:50 GMT  
		Size: 5.7 MB (5684273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10e033372c9ea54711e4453250cd168911b0b43394e197c03164fcab8331f7`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9486420e5d0bd9ffaf1e3828a6eec84d98d97415b6fe70f65534ff451b2c61`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-alpine3.18`

```console
$ docker pull nats@sha256:b196b3729c3c8ceb8c4b7192d7be08520dfd17c42377322a4027b889bcb61d50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:280f97fc32445b7fbf78d249c8e08a78508600838b36b8633b08eed6c8e11b4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9516956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13309d27201a23f166d402964c2bc26937570c70c1ef85ba960d3e4171b6bb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 22:22:47 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:22:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 22:22:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 22:22:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3e725fa689593464ef203de1b06f2e55491fa077b59b693fd9e1ef8c249dd`  
		Last Modified: Fri, 01 Dec 2023 22:23:35 GMT  
		Size: 6.1 MB (6113534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ede37fe98c391207efb9e57a4e29197e178cd9afdafac3140fcf8e44aecc62b`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9177007628f506dd880c66a174348504e4589a3cd156d8377b4278242ffefb9c`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:f9a012265e9ab4e95584f7ea9f4f78234e048366873dcef81b1b46359e22d9f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce4db94168c70869897e9c0941e0567f3ce732d60f92f80ef605d765d9c9686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:49:22 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:49:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:49:25 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9345d2089731ee6f2e92bf32245d1665e8357fecf55c50e9a428966a109c4ed`  
		Last Modified: Fri, 01 Dec 2023 21:50:01 GMT  
		Size: 5.8 MB (5827544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569cb676c86b2aeb776ffd80a904ac5e9bdcda8bea7c0684872fba5efc4b8007`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23edb8dc9637ca24330de881d8e57e7f369ebd6b7b100db2dbae3aff15d50f29`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:d6be8cbc263e2393e2d5f07d4b579c143dada13fe2dd8966097c11e9a1ddc178
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c00554cdbce58cc9a6a11ca1b37f5b90932f2c7bc9b55f096f26b93ba240a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:57:27 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:57:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:57:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8756919eccb97dc6990af357a87c8ba743e3a3ee7ad6d8c8c3dc108620e3c`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 5.8 MB (5818288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55307c3335ece26e2e60bb611f614f94af63814be706d6b3394d9691f55e7f82`  
		Last Modified: Fri, 01 Dec 2023 21:58:15 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7195a7938dcaa9bf7c4b89602950f827640c5bbecbb4a4f858b6a846f6719b`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ecd307e2f9675cf866313820a53a82b1a1459cf04a50da39b145b79360877119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9018304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e350d93fb277376b154a1cc0e44e75d36e34a479bea66c1186b2ef6ce5ec9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:39:48 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:39:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:39:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099335ae91609137f74432a77e75ffc1877279b74582260fc094104662cc3707`  
		Last Modified: Fri, 01 Dec 2023 21:40:50 GMT  
		Size: 5.7 MB (5684273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10e033372c9ea54711e4453250cd168911b0b43394e197c03164fcab8331f7`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9486420e5d0bd9ffaf1e3828a6eec84d98d97415b6fe70f65534ff451b2c61`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-linux`

```console
$ docker pull nats@sha256:87853cd90752f3d33c3a31b152a11a2b9a7736f4a736218a570495225fcbecba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-linux` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-nanoserver`

```console
$ docker pull nats@sha256:cb6e962ac8351dd9c57425e277ee4df9a1891ceb36b91f96de71bcb32e5b7f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10-nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-nanoserver-1809`

```console
$ docker pull nats@sha256:cb6e962ac8351dd9c57425e277ee4df9a1891ceb36b91f96de71bcb32e5b7f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10-nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-scratch`

```console
$ docker pull nats@sha256:87853cd90752f3d33c3a31b152a11a2b9a7736f4a736218a570495225fcbecba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-scratch` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-windowsservercore`

```console
$ docker pull nats@sha256:2635baef88f485e3e6c943dab77da02ccdfbaa09a4cf45a6cade2b95132aa291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:a615001ea716034c1ae2e5cbb7989e5d4b89aa83346c9bfa2c353194009f4c2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063764344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d4d13ef10f01fd53dab0e60ac169100d104101183a8b7564de4a935c98ce88`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:15:41 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:15:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.6/nats-server-v2.10.6-windows-amd64.zip
# Fri, 01 Dec 2023 22:15:43 GMT
ENV NATS_SERVER_SHASUM=8084fc5fc16fa099fae0bb2f74dcf077ab644310918cc16e68b9909330ac798b
# Fri, 01 Dec 2023 22:16:45 GMT
RUN Set-PSDebug -Trace 2
# Fri, 01 Dec 2023 22:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 01 Dec 2023 22:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482d1334c03f2dfeab20b372b19d03e4af7be1261b4b2c858cfa969d0f17c33f`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7056bd68c3f6a5bc1bfdfe4fd9aba9d36b5fa4490e1fa5856be9a04ae3e44a`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c875fab524e257138d947d0cc33bc83d5f79ddf950d886b48f307180daa7d3`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fecdb4839d326ad445940782e3c9036f5487a2f47c185e8682652ec5e049b32`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 437.1 KB (437133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc25e0a531b65458953a005d8f1426da0383911a7e6129de254b037f7a60244b`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 5.9 MB (5882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd9cd8a4c0fd879700f6adde2f07b9c978036ed06509a537e8e9e2327d1974`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5f74a80810732f5daca2a35b749a9c1e0fc520a8fb994930694a05ae073fa2`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cac74b0b7cc9e03fb9c78c17f45ed3e4153089be3dba95e03d5230d8e6336c4`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d9d2aa7f0e9065f683eaa5fcf692b200162ecce3161afef9e766e9a332ed53`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-windowsservercore-1809`

```console
$ docker pull nats@sha256:2635baef88f485e3e6c943dab77da02ccdfbaa09a4cf45a6cade2b95132aa291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:a615001ea716034c1ae2e5cbb7989e5d4b89aa83346c9bfa2c353194009f4c2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063764344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d4d13ef10f01fd53dab0e60ac169100d104101183a8b7564de4a935c98ce88`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:15:41 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:15:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.6/nats-server-v2.10.6-windows-amd64.zip
# Fri, 01 Dec 2023 22:15:43 GMT
ENV NATS_SERVER_SHASUM=8084fc5fc16fa099fae0bb2f74dcf077ab644310918cc16e68b9909330ac798b
# Fri, 01 Dec 2023 22:16:45 GMT
RUN Set-PSDebug -Trace 2
# Fri, 01 Dec 2023 22:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 01 Dec 2023 22:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482d1334c03f2dfeab20b372b19d03e4af7be1261b4b2c858cfa969d0f17c33f`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7056bd68c3f6a5bc1bfdfe4fd9aba9d36b5fa4490e1fa5856be9a04ae3e44a`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c875fab524e257138d947d0cc33bc83d5f79ddf950d886b48f307180daa7d3`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fecdb4839d326ad445940782e3c9036f5487a2f47c185e8682652ec5e049b32`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 437.1 KB (437133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc25e0a531b65458953a005d8f1426da0383911a7e6129de254b037f7a60244b`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 5.9 MB (5882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd9cd8a4c0fd879700f6adde2f07b9c978036ed06509a537e8e9e2327d1974`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5f74a80810732f5daca2a35b749a9c1e0fc520a8fb994930694a05ae073fa2`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cac74b0b7cc9e03fb9c78c17f45ed3e4153089be3dba95e03d5230d8e6336c4`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d9d2aa7f0e9065f683eaa5fcf692b200162ecce3161afef9e766e9a332ed53`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.6`

```console
$ docker pull nats@sha256:fc3dcb7f2944c437451c9091c6fac6ca3df2a53d6dd844f14b5754eabe003e21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10.6` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.6-alpine`

```console
$ docker pull nats@sha256:b196b3729c3c8ceb8c4b7192d7be08520dfd17c42377322a4027b889bcb61d50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.6-alpine` - linux; amd64

```console
$ docker pull nats@sha256:280f97fc32445b7fbf78d249c8e08a78508600838b36b8633b08eed6c8e11b4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9516956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13309d27201a23f166d402964c2bc26937570c70c1ef85ba960d3e4171b6bb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 22:22:47 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:22:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 22:22:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 22:22:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3e725fa689593464ef203de1b06f2e55491fa077b59b693fd9e1ef8c249dd`  
		Last Modified: Fri, 01 Dec 2023 22:23:35 GMT  
		Size: 6.1 MB (6113534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ede37fe98c391207efb9e57a4e29197e178cd9afdafac3140fcf8e44aecc62b`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9177007628f506dd880c66a174348504e4589a3cd156d8377b4278242ffefb9c`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f9a012265e9ab4e95584f7ea9f4f78234e048366873dcef81b1b46359e22d9f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce4db94168c70869897e9c0941e0567f3ce732d60f92f80ef605d765d9c9686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:49:22 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:49:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:49:25 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9345d2089731ee6f2e92bf32245d1665e8357fecf55c50e9a428966a109c4ed`  
		Last Modified: Fri, 01 Dec 2023 21:50:01 GMT  
		Size: 5.8 MB (5827544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569cb676c86b2aeb776ffd80a904ac5e9bdcda8bea7c0684872fba5efc4b8007`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23edb8dc9637ca24330de881d8e57e7f369ebd6b7b100db2dbae3aff15d50f29`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d6be8cbc263e2393e2d5f07d4b579c143dada13fe2dd8966097c11e9a1ddc178
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c00554cdbce58cc9a6a11ca1b37f5b90932f2c7bc9b55f096f26b93ba240a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:57:27 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:57:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:57:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8756919eccb97dc6990af357a87c8ba743e3a3ee7ad6d8c8c3dc108620e3c`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 5.8 MB (5818288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55307c3335ece26e2e60bb611f614f94af63814be706d6b3394d9691f55e7f82`  
		Last Modified: Fri, 01 Dec 2023 21:58:15 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7195a7938dcaa9bf7c4b89602950f827640c5bbecbb4a4f858b6a846f6719b`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ecd307e2f9675cf866313820a53a82b1a1459cf04a50da39b145b79360877119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9018304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e350d93fb277376b154a1cc0e44e75d36e34a479bea66c1186b2ef6ce5ec9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:39:48 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:39:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:39:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099335ae91609137f74432a77e75ffc1877279b74582260fc094104662cc3707`  
		Last Modified: Fri, 01 Dec 2023 21:40:50 GMT  
		Size: 5.7 MB (5684273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10e033372c9ea54711e4453250cd168911b0b43394e197c03164fcab8331f7`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9486420e5d0bd9ffaf1e3828a6eec84d98d97415b6fe70f65534ff451b2c61`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.6-alpine3.18`

```console
$ docker pull nats@sha256:b196b3729c3c8ceb8c4b7192d7be08520dfd17c42377322a4027b889bcb61d50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.6-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:280f97fc32445b7fbf78d249c8e08a78508600838b36b8633b08eed6c8e11b4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9516956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13309d27201a23f166d402964c2bc26937570c70c1ef85ba960d3e4171b6bb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 22:22:47 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:22:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 22:22:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 22:22:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3e725fa689593464ef203de1b06f2e55491fa077b59b693fd9e1ef8c249dd`  
		Last Modified: Fri, 01 Dec 2023 22:23:35 GMT  
		Size: 6.1 MB (6113534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ede37fe98c391207efb9e57a4e29197e178cd9afdafac3140fcf8e44aecc62b`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9177007628f506dd880c66a174348504e4589a3cd156d8377b4278242ffefb9c`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:f9a012265e9ab4e95584f7ea9f4f78234e048366873dcef81b1b46359e22d9f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce4db94168c70869897e9c0941e0567f3ce732d60f92f80ef605d765d9c9686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:49:22 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:49:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:49:25 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9345d2089731ee6f2e92bf32245d1665e8357fecf55c50e9a428966a109c4ed`  
		Last Modified: Fri, 01 Dec 2023 21:50:01 GMT  
		Size: 5.8 MB (5827544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569cb676c86b2aeb776ffd80a904ac5e9bdcda8bea7c0684872fba5efc4b8007`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23edb8dc9637ca24330de881d8e57e7f369ebd6b7b100db2dbae3aff15d50f29`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:d6be8cbc263e2393e2d5f07d4b579c143dada13fe2dd8966097c11e9a1ddc178
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c00554cdbce58cc9a6a11ca1b37f5b90932f2c7bc9b55f096f26b93ba240a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:57:27 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:57:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:57:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8756919eccb97dc6990af357a87c8ba743e3a3ee7ad6d8c8c3dc108620e3c`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 5.8 MB (5818288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55307c3335ece26e2e60bb611f614f94af63814be706d6b3394d9691f55e7f82`  
		Last Modified: Fri, 01 Dec 2023 21:58:15 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7195a7938dcaa9bf7c4b89602950f827640c5bbecbb4a4f858b6a846f6719b`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ecd307e2f9675cf866313820a53a82b1a1459cf04a50da39b145b79360877119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9018304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e350d93fb277376b154a1cc0e44e75d36e34a479bea66c1186b2ef6ce5ec9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:39:48 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:39:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:39:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099335ae91609137f74432a77e75ffc1877279b74582260fc094104662cc3707`  
		Last Modified: Fri, 01 Dec 2023 21:40:50 GMT  
		Size: 5.7 MB (5684273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10e033372c9ea54711e4453250cd168911b0b43394e197c03164fcab8331f7`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9486420e5d0bd9ffaf1e3828a6eec84d98d97415b6fe70f65534ff451b2c61`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.6-linux`

```console
$ docker pull nats@sha256:87853cd90752f3d33c3a31b152a11a2b9a7736f4a736218a570495225fcbecba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.6-linux` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.6-nanoserver`

```console
$ docker pull nats@sha256:cb6e962ac8351dd9c57425e277ee4df9a1891ceb36b91f96de71bcb32e5b7f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10.6-nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.6-nanoserver-1809`

```console
$ docker pull nats@sha256:cb6e962ac8351dd9c57425e277ee4df9a1891ceb36b91f96de71bcb32e5b7f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10.6-nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.6-scratch`

```console
$ docker pull nats@sha256:87853cd90752f3d33c3a31b152a11a2b9a7736f4a736218a570495225fcbecba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.6-scratch` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.6-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.6-windowsservercore`

```console
$ docker pull nats@sha256:2635baef88f485e3e6c943dab77da02ccdfbaa09a4cf45a6cade2b95132aa291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10.6-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:a615001ea716034c1ae2e5cbb7989e5d4b89aa83346c9bfa2c353194009f4c2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063764344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d4d13ef10f01fd53dab0e60ac169100d104101183a8b7564de4a935c98ce88`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:15:41 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:15:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.6/nats-server-v2.10.6-windows-amd64.zip
# Fri, 01 Dec 2023 22:15:43 GMT
ENV NATS_SERVER_SHASUM=8084fc5fc16fa099fae0bb2f74dcf077ab644310918cc16e68b9909330ac798b
# Fri, 01 Dec 2023 22:16:45 GMT
RUN Set-PSDebug -Trace 2
# Fri, 01 Dec 2023 22:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 01 Dec 2023 22:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482d1334c03f2dfeab20b372b19d03e4af7be1261b4b2c858cfa969d0f17c33f`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7056bd68c3f6a5bc1bfdfe4fd9aba9d36b5fa4490e1fa5856be9a04ae3e44a`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c875fab524e257138d947d0cc33bc83d5f79ddf950d886b48f307180daa7d3`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fecdb4839d326ad445940782e3c9036f5487a2f47c185e8682652ec5e049b32`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 437.1 KB (437133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc25e0a531b65458953a005d8f1426da0383911a7e6129de254b037f7a60244b`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 5.9 MB (5882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd9cd8a4c0fd879700f6adde2f07b9c978036ed06509a537e8e9e2327d1974`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5f74a80810732f5daca2a35b749a9c1e0fc520a8fb994930694a05ae073fa2`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cac74b0b7cc9e03fb9c78c17f45ed3e4153089be3dba95e03d5230d8e6336c4`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d9d2aa7f0e9065f683eaa5fcf692b200162ecce3161afef9e766e9a332ed53`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:2635baef88f485e3e6c943dab77da02ccdfbaa09a4cf45a6cade2b95132aa291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10.6-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:a615001ea716034c1ae2e5cbb7989e5d4b89aa83346c9bfa2c353194009f4c2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063764344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d4d13ef10f01fd53dab0e60ac169100d104101183a8b7564de4a935c98ce88`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:15:41 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:15:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.6/nats-server-v2.10.6-windows-amd64.zip
# Fri, 01 Dec 2023 22:15:43 GMT
ENV NATS_SERVER_SHASUM=8084fc5fc16fa099fae0bb2f74dcf077ab644310918cc16e68b9909330ac798b
# Fri, 01 Dec 2023 22:16:45 GMT
RUN Set-PSDebug -Trace 2
# Fri, 01 Dec 2023 22:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 01 Dec 2023 22:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482d1334c03f2dfeab20b372b19d03e4af7be1261b4b2c858cfa969d0f17c33f`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7056bd68c3f6a5bc1bfdfe4fd9aba9d36b5fa4490e1fa5856be9a04ae3e44a`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c875fab524e257138d947d0cc33bc83d5f79ddf950d886b48f307180daa7d3`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fecdb4839d326ad445940782e3c9036f5487a2f47c185e8682652ec5e049b32`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 437.1 KB (437133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc25e0a531b65458953a005d8f1426da0383911a7e6129de254b037f7a60244b`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 5.9 MB (5882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd9cd8a4c0fd879700f6adde2f07b9c978036ed06509a537e8e9e2327d1974`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5f74a80810732f5daca2a35b749a9c1e0fc520a8fb994930694a05ae073fa2`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cac74b0b7cc9e03fb9c78c17f45ed3e4153089be3dba95e03d5230d8e6336c4`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d9d2aa7f0e9065f683eaa5fcf692b200162ecce3161afef9e766e9a332ed53`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:92f7e9aef076cfefd13b8ceee7d3c2e603be5a9751c4fa686b9e1595422d97a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:ca5325d2a2c84eca8c4f3e3ba96a4fcf6dc91e97e3d3ebd3bae69f7a126c0e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5248367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea934ed1a17a93225092fac66c8b617c594ecec00debda4eb753479eeadedab2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:c3d82eee52a26292cc80755a2b88f8b80cef5c80fd438c99768cd1c33ca95a9d in /nats-server 
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:22:59 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:22:59 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:22:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44811b84801c95891b1ccde13fe7e76a1ffd8795cd2a066ac0630ee836c23c2e`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 5.2 MB (5247859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927d64e5da79549425963bee122f44117e41eaa442b01673188effd14c9b236`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d3ccb1b790e4433d69872d7ddb8377aac40d6f000a66fa5b2795a62122a4f54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4984842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f1a1ecd1b37c66268f966a88d26fa44b35f70909dedab19c60bfd5aca2035e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:401de119a9fad5bd89c70f5a4d5c70f110d490ae5ab9aa60a7f963686ab297ee in /nats-server 
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:49:29 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f1d2c1b6f013f4386e7235452bc47cebd8001115c3a6504b418ee5b90071492a`  
		Last Modified: Wed, 08 Nov 2023 19:50:14 GMT  
		Size: 5.0 MB (4984334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5fea0f4bcfa87853f77179e249f0a8a09723aeb1c53882e3036fa6250a4ff5`  
		Last Modified: Wed, 08 Nov 2023 19:50:13 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:c73b24d4fb1ad910ad2f2bdefe0d18bfec11431afb4da9e3cd2be176e4fd49b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4977978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfe5b4a001ee28a1308edc00242441032b2afb69148c7ba17f692f75e2c1dba`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:cd8c3bf2b10d14de1f76a0617be080153909dadcd658bb62cab16d41a650d3de in /nats-server 
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:57:47 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:57:47 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:57:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e2a0a8d03803b71ab2e1e3540de965b9430b493bbd15bb2cb1372a7dd564c76d`  
		Last Modified: Wed, 08 Nov 2023 19:58:32 GMT  
		Size: 5.0 MB (4977470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe9df0b73b8b228e9331792251ba43d36af5e4e898411b4f9b725bb8928231`  
		Last Modified: Wed, 08 Nov 2023 19:58:31 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:770e514bf6ca4d8b056bd9d16b7df5f56c45c587ce3c815515051b6588e38325
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4785043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75bc6347feea13831461567c92c52c13e9085417ef409fb74364cf63105e346`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:40:10 GMT
COPY file:209cf40c58f80a36d8d8c8060f48a598dcf03ae451d8d658f267d02f3ce7bddc in /nats-server 
# Wed, 08 Nov 2023 19:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:40:11 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:40:11 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:40:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b497fc8beff1c9fb319e3b4b62e22135e8e8d81506ede3ca51365887947a8571`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 4.8 MB (4784535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbc2e7980e0793ef96d07cc5a7d9418109519d7d6982ba49570b90d02b2932c`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:b087009ae59c4cdd4635da1705113414178def86fff87b1782aa641518aceabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b9760d6ab57277746ebd4a5f45cdd62d136ab263dde27530ecb393d7948a510c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9274592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f636d0b11c184a900b54c5d7a77db40637112bfd90df182fba840b790185af83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:09:38 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 07:09:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 07:09:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 07:09:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 07:09:41 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 07:09:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 07:09:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9578e239cd41494ce6bc261c76183aa35ba1635ff7da33f4953d482462199b0f`  
		Last Modified: Fri, 01 Dec 2023 07:10:35 GMT  
		Size: 5.9 MB (5871171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597cdbbc35cac5971c40aea18a64c7c83a8267d64c3fae6d8768f94ea0b74267`  
		Last Modified: Fri, 01 Dec 2023 07:10:34 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e3e4c7ded20424c41f2bb52c27d5d7d81fd98cbfdcd01d5c0165f223eaf5e5`  
		Last Modified: Fri, 01 Dec 2023 07:10:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:ea12096d05d14c61677a950ccecc14fa970228a2f9c32cc9756a34d16e23627e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8755974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:421c22f9992da9e131b79a8e00614b62903755a114929c4efeca51d4104147a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:11:34 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 01:11:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 01:11:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 01:11:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 01:11:37 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 01:11:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 01:11:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d08b1bd7ab7a87de18e67897b423e6b9889387c94e2409d3f50904ec9c4369`  
		Last Modified: Fri, 01 Dec 2023 01:12:26 GMT  
		Size: 5.6 MB (5608105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3e4b8e5ff4da13becde614c85a197b276c30ec0a40344c59375f6560dd0fae`  
		Last Modified: Fri, 01 Dec 2023 01:12:25 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea581f787924f03908f3e60d8c32cf33838817759152d4b770bfdf856f84a5e1`  
		Last Modified: Fri, 01 Dec 2023 01:12:25 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:05b36a001a744855e2a6c380a7bbae4e26dc97a919a3c3e3ebe5823f81bba33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8501789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c61d4486d4b114eaf1ce5b76c58021f275bb492b7833a0c80baa9663d0e3c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:40:43 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 08:40:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 08:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 08:40:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 08:40:45 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 08:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 08:40:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73711fc2619c12c62854a9c20221e8c3839f788c5a9008fb9c010d01ea3939a3`  
		Last Modified: Fri, 01 Dec 2023 08:41:33 GMT  
		Size: 5.6 MB (5599786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba96a64bd8cba7223b4ce5373e3023bdd5aa7396dd6835f9b937f1a947136a`  
		Last Modified: Fri, 01 Dec 2023 08:41:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52b2393485a327cca73588e8ee7193621866651443dd05e3405f98fc95e19c8`  
		Last Modified: Fri, 01 Dec 2023 08:41:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dca7f08c15964b4a8cc436c24991169164b12346402bd654463ec2ff681e0c3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8743160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77456cfbbeb9029aac27494820926655ed21a0fba12973c5f6f2503d158e8ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:51:49 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 06:51:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 06:51:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 06:51:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 06:51:51 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 06:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 06:51:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab8ef6574318adae379d2e75bbf778f65dff87dbcb0edea015ca7f1278fce8`  
		Last Modified: Fri, 01 Dec 2023 06:52:54 GMT  
		Size: 5.4 MB (5409130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3971496dd7ba6ccc13bc02b17a9cb6505875c932acdd92409788c1b30ba363df`  
		Last Modified: Fri, 01 Dec 2023 06:52:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e970079ad876afa0bb32bb58d51deb029ab07587a278cb947625fa85569ce1`  
		Last Modified: Fri, 01 Dec 2023 06:52:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.18`

```console
$ docker pull nats@sha256:b087009ae59c4cdd4635da1705113414178def86fff87b1782aa641518aceabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:b9760d6ab57277746ebd4a5f45cdd62d136ab263dde27530ecb393d7948a510c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9274592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f636d0b11c184a900b54c5d7a77db40637112bfd90df182fba840b790185af83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:09:38 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 07:09:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 07:09:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 07:09:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 07:09:41 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 07:09:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 07:09:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9578e239cd41494ce6bc261c76183aa35ba1635ff7da33f4953d482462199b0f`  
		Last Modified: Fri, 01 Dec 2023 07:10:35 GMT  
		Size: 5.9 MB (5871171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597cdbbc35cac5971c40aea18a64c7c83a8267d64c3fae6d8768f94ea0b74267`  
		Last Modified: Fri, 01 Dec 2023 07:10:34 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e3e4c7ded20424c41f2bb52c27d5d7d81fd98cbfdcd01d5c0165f223eaf5e5`  
		Last Modified: Fri, 01 Dec 2023 07:10:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:ea12096d05d14c61677a950ccecc14fa970228a2f9c32cc9756a34d16e23627e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8755974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:421c22f9992da9e131b79a8e00614b62903755a114929c4efeca51d4104147a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:11:34 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 01:11:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 01:11:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 01:11:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 01:11:37 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 01:11:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 01:11:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d08b1bd7ab7a87de18e67897b423e6b9889387c94e2409d3f50904ec9c4369`  
		Last Modified: Fri, 01 Dec 2023 01:12:26 GMT  
		Size: 5.6 MB (5608105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3e4b8e5ff4da13becde614c85a197b276c30ec0a40344c59375f6560dd0fae`  
		Last Modified: Fri, 01 Dec 2023 01:12:25 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea581f787924f03908f3e60d8c32cf33838817759152d4b770bfdf856f84a5e1`  
		Last Modified: Fri, 01 Dec 2023 01:12:25 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:05b36a001a744855e2a6c380a7bbae4e26dc97a919a3c3e3ebe5823f81bba33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8501789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c61d4486d4b114eaf1ce5b76c58021f275bb492b7833a0c80baa9663d0e3c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:40:43 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 08:40:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 08:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 08:40:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 08:40:45 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 08:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 08:40:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73711fc2619c12c62854a9c20221e8c3839f788c5a9008fb9c010d01ea3939a3`  
		Last Modified: Fri, 01 Dec 2023 08:41:33 GMT  
		Size: 5.6 MB (5599786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba96a64bd8cba7223b4ce5373e3023bdd5aa7396dd6835f9b937f1a947136a`  
		Last Modified: Fri, 01 Dec 2023 08:41:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52b2393485a327cca73588e8ee7193621866651443dd05e3405f98fc95e19c8`  
		Last Modified: Fri, 01 Dec 2023 08:41:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dca7f08c15964b4a8cc436c24991169164b12346402bd654463ec2ff681e0c3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8743160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77456cfbbeb9029aac27494820926655ed21a0fba12973c5f6f2503d158e8ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:51:49 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 06:51:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 06:51:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 06:51:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 06:51:51 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 06:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 06:51:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab8ef6574318adae379d2e75bbf778f65dff87dbcb0edea015ca7f1278fce8`  
		Last Modified: Fri, 01 Dec 2023 06:52:54 GMT  
		Size: 5.4 MB (5409130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3971496dd7ba6ccc13bc02b17a9cb6505875c932acdd92409788c1b30ba363df`  
		Last Modified: Fri, 01 Dec 2023 06:52:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e970079ad876afa0bb32bb58d51deb029ab07587a278cb947625fa85569ce1`  
		Last Modified: Fri, 01 Dec 2023 06:52:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:92f7e9aef076cfefd13b8ceee7d3c2e603be5a9751c4fa686b9e1595422d97a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:ca5325d2a2c84eca8c4f3e3ba96a4fcf6dc91e97e3d3ebd3bae69f7a126c0e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5248367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea934ed1a17a93225092fac66c8b617c594ecec00debda4eb753479eeadedab2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:c3d82eee52a26292cc80755a2b88f8b80cef5c80fd438c99768cd1c33ca95a9d in /nats-server 
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:22:59 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:22:59 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:22:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44811b84801c95891b1ccde13fe7e76a1ffd8795cd2a066ac0630ee836c23c2e`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 5.2 MB (5247859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927d64e5da79549425963bee122f44117e41eaa442b01673188effd14c9b236`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d3ccb1b790e4433d69872d7ddb8377aac40d6f000a66fa5b2795a62122a4f54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4984842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f1a1ecd1b37c66268f966a88d26fa44b35f70909dedab19c60bfd5aca2035e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:401de119a9fad5bd89c70f5a4d5c70f110d490ae5ab9aa60a7f963686ab297ee in /nats-server 
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:49:29 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f1d2c1b6f013f4386e7235452bc47cebd8001115c3a6504b418ee5b90071492a`  
		Last Modified: Wed, 08 Nov 2023 19:50:14 GMT  
		Size: 5.0 MB (4984334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5fea0f4bcfa87853f77179e249f0a8a09723aeb1c53882e3036fa6250a4ff5`  
		Last Modified: Wed, 08 Nov 2023 19:50:13 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:c73b24d4fb1ad910ad2f2bdefe0d18bfec11431afb4da9e3cd2be176e4fd49b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4977978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfe5b4a001ee28a1308edc00242441032b2afb69148c7ba17f692f75e2c1dba`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:cd8c3bf2b10d14de1f76a0617be080153909dadcd658bb62cab16d41a650d3de in /nats-server 
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:57:47 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:57:47 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:57:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e2a0a8d03803b71ab2e1e3540de965b9430b493bbd15bb2cb1372a7dd564c76d`  
		Last Modified: Wed, 08 Nov 2023 19:58:32 GMT  
		Size: 5.0 MB (4977470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe9df0b73b8b228e9331792251ba43d36af5e4e898411b4f9b725bb8928231`  
		Last Modified: Wed, 08 Nov 2023 19:58:31 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:770e514bf6ca4d8b056bd9d16b7df5f56c45c587ce3c815515051b6588e38325
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4785043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75bc6347feea13831461567c92c52c13e9085417ef409fb74364cf63105e346`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:40:10 GMT
COPY file:209cf40c58f80a36d8d8c8060f48a598dcf03ae451d8d658f267d02f3ce7bddc in /nats-server 
# Wed, 08 Nov 2023 19:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:40:11 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:40:11 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:40:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b497fc8beff1c9fb319e3b4b62e22135e8e8d81506ede3ca51365887947a8571`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 4.8 MB (4784535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbc2e7980e0793ef96d07cc5a7d9418109519d7d6982ba49570b90d02b2932c`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:1ad695d981e825ae558a90d280eff8792fd369346b2ea64dff57c1d3ce8e5c28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:73f5d1f23c60e8c64bea6d8e55905285d30fa448f7ade9f8597a2d00a3d27ce4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109832813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:760507fd1783c222411869a2c4984d6a7c25c9d95988192a123e33bd1c414f11`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Nov 2023 05:11:01 GMT
RUN cmd /S /C #(nop) COPY file:bb76bb5eb2960343e0d31314ed4649c426ed59ad3d060057e2c1038e39265b76 in C:\nats-server.exe 
# Thu, 16 Nov 2023 05:11:02 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Nov 2023 05:11:03 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Nov 2023 05:11:03 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Nov 2023 05:11:04 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ac187e96a930e789fbdb3f3db19e7bb86f976983a562cd0521cea11347081e`  
		Last Modified: Thu, 16 Nov 2023 05:12:32 GMT  
		Size: 5.3 MB (5328972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9411de359e9c869b82c760e0e711247a49a4f058e2af773d6dd88260a68676d1`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea6582c6c01cd47f9f93a5ab8ebdf0e7d2bb4e444102237dc7b1d065928549b`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166ef556e54aaa80a6793bd63fdb796202e73717cb42a0e92586c8359b032f79`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d79fe9949ea94463332152fddb029659945f9beb57010148579273228d8935`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:1ad695d981e825ae558a90d280eff8792fd369346b2ea64dff57c1d3ce8e5c28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:73f5d1f23c60e8c64bea6d8e55905285d30fa448f7ade9f8597a2d00a3d27ce4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109832813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:760507fd1783c222411869a2c4984d6a7c25c9d95988192a123e33bd1c414f11`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Nov 2023 05:11:01 GMT
RUN cmd /S /C #(nop) COPY file:bb76bb5eb2960343e0d31314ed4649c426ed59ad3d060057e2c1038e39265b76 in C:\nats-server.exe 
# Thu, 16 Nov 2023 05:11:02 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Nov 2023 05:11:03 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Nov 2023 05:11:03 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Nov 2023 05:11:04 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ac187e96a930e789fbdb3f3db19e7bb86f976983a562cd0521cea11347081e`  
		Last Modified: Thu, 16 Nov 2023 05:12:32 GMT  
		Size: 5.3 MB (5328972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9411de359e9c869b82c760e0e711247a49a4f058e2af773d6dd88260a68676d1`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea6582c6c01cd47f9f93a5ab8ebdf0e7d2bb4e444102237dc7b1d065928549b`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166ef556e54aaa80a6793bd63fdb796202e73717cb42a0e92586c8359b032f79`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d79fe9949ea94463332152fddb029659945f9beb57010148579273228d8935`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:92f7e9aef076cfefd13b8ceee7d3c2e603be5a9751c4fa686b9e1595422d97a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ca5325d2a2c84eca8c4f3e3ba96a4fcf6dc91e97e3d3ebd3bae69f7a126c0e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5248367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea934ed1a17a93225092fac66c8b617c594ecec00debda4eb753479eeadedab2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:c3d82eee52a26292cc80755a2b88f8b80cef5c80fd438c99768cd1c33ca95a9d in /nats-server 
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:22:59 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:22:59 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:22:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44811b84801c95891b1ccde13fe7e76a1ffd8795cd2a066ac0630ee836c23c2e`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 5.2 MB (5247859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927d64e5da79549425963bee122f44117e41eaa442b01673188effd14c9b236`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d3ccb1b790e4433d69872d7ddb8377aac40d6f000a66fa5b2795a62122a4f54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4984842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f1a1ecd1b37c66268f966a88d26fa44b35f70909dedab19c60bfd5aca2035e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:401de119a9fad5bd89c70f5a4d5c70f110d490ae5ab9aa60a7f963686ab297ee in /nats-server 
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:49:29 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f1d2c1b6f013f4386e7235452bc47cebd8001115c3a6504b418ee5b90071492a`  
		Last Modified: Wed, 08 Nov 2023 19:50:14 GMT  
		Size: 5.0 MB (4984334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5fea0f4bcfa87853f77179e249f0a8a09723aeb1c53882e3036fa6250a4ff5`  
		Last Modified: Wed, 08 Nov 2023 19:50:13 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:c73b24d4fb1ad910ad2f2bdefe0d18bfec11431afb4da9e3cd2be176e4fd49b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4977978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfe5b4a001ee28a1308edc00242441032b2afb69148c7ba17f692f75e2c1dba`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:cd8c3bf2b10d14de1f76a0617be080153909dadcd658bb62cab16d41a650d3de in /nats-server 
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:57:47 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:57:47 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:57:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e2a0a8d03803b71ab2e1e3540de965b9430b493bbd15bb2cb1372a7dd564c76d`  
		Last Modified: Wed, 08 Nov 2023 19:58:32 GMT  
		Size: 5.0 MB (4977470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe9df0b73b8b228e9331792251ba43d36af5e4e898411b4f9b725bb8928231`  
		Last Modified: Wed, 08 Nov 2023 19:58:31 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:770e514bf6ca4d8b056bd9d16b7df5f56c45c587ce3c815515051b6588e38325
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4785043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75bc6347feea13831461567c92c52c13e9085417ef409fb74364cf63105e346`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:40:10 GMT
COPY file:209cf40c58f80a36d8d8c8060f48a598dcf03ae451d8d658f267d02f3ce7bddc in /nats-server 
# Wed, 08 Nov 2023 19:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:40:11 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:40:11 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:40:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b497fc8beff1c9fb319e3b4b62e22135e8e8d81506ede3ca51365887947a8571`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 4.8 MB (4784535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbc2e7980e0793ef96d07cc5a7d9418109519d7d6982ba49570b90d02b2932c`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:b1e446a786a171431a795c1fa47128cacda24f39e0a7573a81959cbf2af4701e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:738db334d9d9b1f12a02ea151d9c48e0979703e801563bcf4e10d409d2d84172
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063502948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c10ef44f34cf615be280ea2fb6a99b60935a13a82fd8594ff2a80647ac91f420`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Nov 2023 05:07:47 GMT
ENV NATS_SERVER=2.9.24
# Thu, 16 Nov 2023 05:07:48 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.24/nats-server-v2.9.24-windows-amd64.zip
# Thu, 16 Nov 2023 05:07:49 GMT
ENV NATS_SERVER_SHASUM=4caa027910bfa0a79f2d1c01739e356df37dae15f1336174d459d2fd3a0e10d2
# Thu, 16 Nov 2023 05:08:53 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Nov 2023 05:10:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Nov 2023 05:10:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Nov 2023 05:10:39 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Nov 2023 05:10:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Nov 2023 05:10:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c35ae5a263cc82b97d893eece2f8371e8a0ad891752ccd514458fe125e1295`  
		Last Modified: Thu, 16 Nov 2023 05:12:21 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a68baad997636ffebee461869c70b5306f4dd52f21331e0586fff15e010659`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e56791fa6e91c6a1f2cec1bd459b01a184383d5ffc47cfff520d64f78f909a`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d6b958512faa97adacdb786dc3b6b2801ddeff298fd54a9be9279a625c993a`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 443.1 KB (443149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400de512823b4dd5067aeae94ba2b310e89bed83ff1730276164c6345459dc75`  
		Last Modified: Thu, 16 Nov 2023 05:12:19 GMT  
		Size: 5.6 MB (5615206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f93aaac049b5611b016e56ddddc1aec80f677513bd2506b0df17819e591e114`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 2.0 KB (1981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e740c0ab523cb4e1f0e60000a1a8da03fb645e9219eaf4cbbc8744134d83be`  
		Last Modified: Thu, 16 Nov 2023 05:12:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63012bc0bbc7f34223f89862b35418d4c72c8cfb1b43e4c97c09bd83d1dc43`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aab02fc5cc3eed11d240652a86121dff960e443a8f2538ebfaa9abf846d48d`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:b1e446a786a171431a795c1fa47128cacda24f39e0a7573a81959cbf2af4701e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:738db334d9d9b1f12a02ea151d9c48e0979703e801563bcf4e10d409d2d84172
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063502948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c10ef44f34cf615be280ea2fb6a99b60935a13a82fd8594ff2a80647ac91f420`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Nov 2023 05:07:47 GMT
ENV NATS_SERVER=2.9.24
# Thu, 16 Nov 2023 05:07:48 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.24/nats-server-v2.9.24-windows-amd64.zip
# Thu, 16 Nov 2023 05:07:49 GMT
ENV NATS_SERVER_SHASUM=4caa027910bfa0a79f2d1c01739e356df37dae15f1336174d459d2fd3a0e10d2
# Thu, 16 Nov 2023 05:08:53 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Nov 2023 05:10:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Nov 2023 05:10:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Nov 2023 05:10:39 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Nov 2023 05:10:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Nov 2023 05:10:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c35ae5a263cc82b97d893eece2f8371e8a0ad891752ccd514458fe125e1295`  
		Last Modified: Thu, 16 Nov 2023 05:12:21 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a68baad997636ffebee461869c70b5306f4dd52f21331e0586fff15e010659`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e56791fa6e91c6a1f2cec1bd459b01a184383d5ffc47cfff520d64f78f909a`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d6b958512faa97adacdb786dc3b6b2801ddeff298fd54a9be9279a625c993a`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 443.1 KB (443149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400de512823b4dd5067aeae94ba2b310e89bed83ff1730276164c6345459dc75`  
		Last Modified: Thu, 16 Nov 2023 05:12:19 GMT  
		Size: 5.6 MB (5615206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f93aaac049b5611b016e56ddddc1aec80f677513bd2506b0df17819e591e114`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 2.0 KB (1981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e740c0ab523cb4e1f0e60000a1a8da03fb645e9219eaf4cbbc8744134d83be`  
		Last Modified: Thu, 16 Nov 2023 05:12:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63012bc0bbc7f34223f89862b35418d4c72c8cfb1b43e4c97c09bd83d1dc43`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aab02fc5cc3eed11d240652a86121dff960e443a8f2538ebfaa9abf846d48d`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.24`

```console
$ docker pull nats@sha256:92f7e9aef076cfefd13b8ceee7d3c2e603be5a9751c4fa686b9e1595422d97a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.24` - linux; amd64

```console
$ docker pull nats@sha256:ca5325d2a2c84eca8c4f3e3ba96a4fcf6dc91e97e3d3ebd3bae69f7a126c0e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5248367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea934ed1a17a93225092fac66c8b617c594ecec00debda4eb753479eeadedab2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:c3d82eee52a26292cc80755a2b88f8b80cef5c80fd438c99768cd1c33ca95a9d in /nats-server 
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:22:59 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:22:59 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:22:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44811b84801c95891b1ccde13fe7e76a1ffd8795cd2a066ac0630ee836c23c2e`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 5.2 MB (5247859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927d64e5da79549425963bee122f44117e41eaa442b01673188effd14c9b236`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d3ccb1b790e4433d69872d7ddb8377aac40d6f000a66fa5b2795a62122a4f54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4984842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f1a1ecd1b37c66268f966a88d26fa44b35f70909dedab19c60bfd5aca2035e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:401de119a9fad5bd89c70f5a4d5c70f110d490ae5ab9aa60a7f963686ab297ee in /nats-server 
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:49:29 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f1d2c1b6f013f4386e7235452bc47cebd8001115c3a6504b418ee5b90071492a`  
		Last Modified: Wed, 08 Nov 2023 19:50:14 GMT  
		Size: 5.0 MB (4984334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5fea0f4bcfa87853f77179e249f0a8a09723aeb1c53882e3036fa6250a4ff5`  
		Last Modified: Wed, 08 Nov 2023 19:50:13 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24` - linux; arm variant v7

```console
$ docker pull nats@sha256:c73b24d4fb1ad910ad2f2bdefe0d18bfec11431afb4da9e3cd2be176e4fd49b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4977978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfe5b4a001ee28a1308edc00242441032b2afb69148c7ba17f692f75e2c1dba`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:cd8c3bf2b10d14de1f76a0617be080153909dadcd658bb62cab16d41a650d3de in /nats-server 
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:57:47 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:57:47 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:57:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e2a0a8d03803b71ab2e1e3540de965b9430b493bbd15bb2cb1372a7dd564c76d`  
		Last Modified: Wed, 08 Nov 2023 19:58:32 GMT  
		Size: 5.0 MB (4977470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe9df0b73b8b228e9331792251ba43d36af5e4e898411b4f9b725bb8928231`  
		Last Modified: Wed, 08 Nov 2023 19:58:31 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:770e514bf6ca4d8b056bd9d16b7df5f56c45c587ce3c815515051b6588e38325
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4785043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75bc6347feea13831461567c92c52c13e9085417ef409fb74364cf63105e346`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:40:10 GMT
COPY file:209cf40c58f80a36d8d8c8060f48a598dcf03ae451d8d658f267d02f3ce7bddc in /nats-server 
# Wed, 08 Nov 2023 19:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:40:11 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:40:11 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:40:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b497fc8beff1c9fb319e3b4b62e22135e8e8d81506ede3ca51365887947a8571`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 4.8 MB (4784535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbc2e7980e0793ef96d07cc5a7d9418109519d7d6982ba49570b90d02b2932c`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.24-alpine`

```console
$ docker pull nats@sha256:b087009ae59c4cdd4635da1705113414178def86fff87b1782aa641518aceabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.24-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b9760d6ab57277746ebd4a5f45cdd62d136ab263dde27530ecb393d7948a510c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9274592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f636d0b11c184a900b54c5d7a77db40637112bfd90df182fba840b790185af83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:09:38 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 07:09:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 07:09:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 07:09:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 07:09:41 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 07:09:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 07:09:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9578e239cd41494ce6bc261c76183aa35ba1635ff7da33f4953d482462199b0f`  
		Last Modified: Fri, 01 Dec 2023 07:10:35 GMT  
		Size: 5.9 MB (5871171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597cdbbc35cac5971c40aea18a64c7c83a8267d64c3fae6d8768f94ea0b74267`  
		Last Modified: Fri, 01 Dec 2023 07:10:34 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e3e4c7ded20424c41f2bb52c27d5d7d81fd98cbfdcd01d5c0165f223eaf5e5`  
		Last Modified: Fri, 01 Dec 2023 07:10:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:ea12096d05d14c61677a950ccecc14fa970228a2f9c32cc9756a34d16e23627e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8755974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:421c22f9992da9e131b79a8e00614b62903755a114929c4efeca51d4104147a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:11:34 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 01:11:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 01:11:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 01:11:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 01:11:37 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 01:11:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 01:11:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d08b1bd7ab7a87de18e67897b423e6b9889387c94e2409d3f50904ec9c4369`  
		Last Modified: Fri, 01 Dec 2023 01:12:26 GMT  
		Size: 5.6 MB (5608105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3e4b8e5ff4da13becde614c85a197b276c30ec0a40344c59375f6560dd0fae`  
		Last Modified: Fri, 01 Dec 2023 01:12:25 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea581f787924f03908f3e60d8c32cf33838817759152d4b770bfdf856f84a5e1`  
		Last Modified: Fri, 01 Dec 2023 01:12:25 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:05b36a001a744855e2a6c380a7bbae4e26dc97a919a3c3e3ebe5823f81bba33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8501789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c61d4486d4b114eaf1ce5b76c58021f275bb492b7833a0c80baa9663d0e3c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:40:43 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 08:40:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 08:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 08:40:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 08:40:45 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 08:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 08:40:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73711fc2619c12c62854a9c20221e8c3839f788c5a9008fb9c010d01ea3939a3`  
		Last Modified: Fri, 01 Dec 2023 08:41:33 GMT  
		Size: 5.6 MB (5599786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba96a64bd8cba7223b4ce5373e3023bdd5aa7396dd6835f9b937f1a947136a`  
		Last Modified: Fri, 01 Dec 2023 08:41:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52b2393485a327cca73588e8ee7193621866651443dd05e3405f98fc95e19c8`  
		Last Modified: Fri, 01 Dec 2023 08:41:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dca7f08c15964b4a8cc436c24991169164b12346402bd654463ec2ff681e0c3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8743160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77456cfbbeb9029aac27494820926655ed21a0fba12973c5f6f2503d158e8ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:51:49 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 06:51:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 06:51:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 06:51:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 06:51:51 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 06:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 06:51:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab8ef6574318adae379d2e75bbf778f65dff87dbcb0edea015ca7f1278fce8`  
		Last Modified: Fri, 01 Dec 2023 06:52:54 GMT  
		Size: 5.4 MB (5409130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3971496dd7ba6ccc13bc02b17a9cb6505875c932acdd92409788c1b30ba363df`  
		Last Modified: Fri, 01 Dec 2023 06:52:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e970079ad876afa0bb32bb58d51deb029ab07587a278cb947625fa85569ce1`  
		Last Modified: Fri, 01 Dec 2023 06:52:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.24-alpine3.18`

```console
$ docker pull nats@sha256:b087009ae59c4cdd4635da1705113414178def86fff87b1782aa641518aceabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.24-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:b9760d6ab57277746ebd4a5f45cdd62d136ab263dde27530ecb393d7948a510c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9274592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f636d0b11c184a900b54c5d7a77db40637112bfd90df182fba840b790185af83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:09:38 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 07:09:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 07:09:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 07:09:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 07:09:41 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 07:09:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 07:09:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9578e239cd41494ce6bc261c76183aa35ba1635ff7da33f4953d482462199b0f`  
		Last Modified: Fri, 01 Dec 2023 07:10:35 GMT  
		Size: 5.9 MB (5871171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597cdbbc35cac5971c40aea18a64c7c83a8267d64c3fae6d8768f94ea0b74267`  
		Last Modified: Fri, 01 Dec 2023 07:10:34 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e3e4c7ded20424c41f2bb52c27d5d7d81fd98cbfdcd01d5c0165f223eaf5e5`  
		Last Modified: Fri, 01 Dec 2023 07:10:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:ea12096d05d14c61677a950ccecc14fa970228a2f9c32cc9756a34d16e23627e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8755974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:421c22f9992da9e131b79a8e00614b62903755a114929c4efeca51d4104147a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:11:34 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 01:11:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 01:11:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 01:11:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 01:11:37 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 01:11:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 01:11:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d08b1bd7ab7a87de18e67897b423e6b9889387c94e2409d3f50904ec9c4369`  
		Last Modified: Fri, 01 Dec 2023 01:12:26 GMT  
		Size: 5.6 MB (5608105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3e4b8e5ff4da13becde614c85a197b276c30ec0a40344c59375f6560dd0fae`  
		Last Modified: Fri, 01 Dec 2023 01:12:25 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea581f787924f03908f3e60d8c32cf33838817759152d4b770bfdf856f84a5e1`  
		Last Modified: Fri, 01 Dec 2023 01:12:25 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:05b36a001a744855e2a6c380a7bbae4e26dc97a919a3c3e3ebe5823f81bba33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8501789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c61d4486d4b114eaf1ce5b76c58021f275bb492b7833a0c80baa9663d0e3c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:40:43 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 08:40:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 08:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 08:40:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 08:40:45 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 08:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 08:40:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73711fc2619c12c62854a9c20221e8c3839f788c5a9008fb9c010d01ea3939a3`  
		Last Modified: Fri, 01 Dec 2023 08:41:33 GMT  
		Size: 5.6 MB (5599786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba96a64bd8cba7223b4ce5373e3023bdd5aa7396dd6835f9b937f1a947136a`  
		Last Modified: Fri, 01 Dec 2023 08:41:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52b2393485a327cca73588e8ee7193621866651443dd05e3405f98fc95e19c8`  
		Last Modified: Fri, 01 Dec 2023 08:41:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dca7f08c15964b4a8cc436c24991169164b12346402bd654463ec2ff681e0c3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8743160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77456cfbbeb9029aac27494820926655ed21a0fba12973c5f6f2503d158e8ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:51:49 GMT
ENV NATS_SERVER=2.9.24
# Fri, 01 Dec 2023 06:51:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c6afa824992389dd0f7fa4073eeaa8b842849c71b0b782da11101b68e4e032fd' ;; 		armhf) natsArch='arm6'; sha256='a5ef539629cde74f974691a78a66a4e30a95a88de06040ad579a606931eade4a' ;; 		armv7) natsArch='arm7'; sha256='514e4a1123f82b775d6b17a12d1a7ce10fa8b5a1b86b9a831c09b13a7e6bc9b0' ;; 		x86_64) natsArch='amd64'; sha256='f4d5dc256d758fa42e7cbf2ddcacc2edfc379bedc0bbdcf5fe6cb67ff3a82d7c' ;; 		x86) natsArch='386'; sha256='b477a8e9a28746fce5bdf5333d16469351de2294402085df81126e699399ec48' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 06:51:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 06:51:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 06:51:51 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 06:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 06:51:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab8ef6574318adae379d2e75bbf778f65dff87dbcb0edea015ca7f1278fce8`  
		Last Modified: Fri, 01 Dec 2023 06:52:54 GMT  
		Size: 5.4 MB (5409130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3971496dd7ba6ccc13bc02b17a9cb6505875c932acdd92409788c1b30ba363df`  
		Last Modified: Fri, 01 Dec 2023 06:52:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e970079ad876afa0bb32bb58d51deb029ab07587a278cb947625fa85569ce1`  
		Last Modified: Fri, 01 Dec 2023 06:52:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.24-linux`

```console
$ docker pull nats@sha256:92f7e9aef076cfefd13b8ceee7d3c2e603be5a9751c4fa686b9e1595422d97a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.24-linux` - linux; amd64

```console
$ docker pull nats@sha256:ca5325d2a2c84eca8c4f3e3ba96a4fcf6dc91e97e3d3ebd3bae69f7a126c0e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5248367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea934ed1a17a93225092fac66c8b617c594ecec00debda4eb753479eeadedab2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:c3d82eee52a26292cc80755a2b88f8b80cef5c80fd438c99768cd1c33ca95a9d in /nats-server 
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:22:59 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:22:59 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:22:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44811b84801c95891b1ccde13fe7e76a1ffd8795cd2a066ac0630ee836c23c2e`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 5.2 MB (5247859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927d64e5da79549425963bee122f44117e41eaa442b01673188effd14c9b236`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d3ccb1b790e4433d69872d7ddb8377aac40d6f000a66fa5b2795a62122a4f54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4984842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f1a1ecd1b37c66268f966a88d26fa44b35f70909dedab19c60bfd5aca2035e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:401de119a9fad5bd89c70f5a4d5c70f110d490ae5ab9aa60a7f963686ab297ee in /nats-server 
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:49:29 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f1d2c1b6f013f4386e7235452bc47cebd8001115c3a6504b418ee5b90071492a`  
		Last Modified: Wed, 08 Nov 2023 19:50:14 GMT  
		Size: 5.0 MB (4984334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5fea0f4bcfa87853f77179e249f0a8a09723aeb1c53882e3036fa6250a4ff5`  
		Last Modified: Wed, 08 Nov 2023 19:50:13 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:c73b24d4fb1ad910ad2f2bdefe0d18bfec11431afb4da9e3cd2be176e4fd49b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4977978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfe5b4a001ee28a1308edc00242441032b2afb69148c7ba17f692f75e2c1dba`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:cd8c3bf2b10d14de1f76a0617be080153909dadcd658bb62cab16d41a650d3de in /nats-server 
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:57:47 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:57:47 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:57:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e2a0a8d03803b71ab2e1e3540de965b9430b493bbd15bb2cb1372a7dd564c76d`  
		Last Modified: Wed, 08 Nov 2023 19:58:32 GMT  
		Size: 5.0 MB (4977470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe9df0b73b8b228e9331792251ba43d36af5e4e898411b4f9b725bb8928231`  
		Last Modified: Wed, 08 Nov 2023 19:58:31 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:770e514bf6ca4d8b056bd9d16b7df5f56c45c587ce3c815515051b6588e38325
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4785043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75bc6347feea13831461567c92c52c13e9085417ef409fb74364cf63105e346`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:40:10 GMT
COPY file:209cf40c58f80a36d8d8c8060f48a598dcf03ae451d8d658f267d02f3ce7bddc in /nats-server 
# Wed, 08 Nov 2023 19:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:40:11 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:40:11 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:40:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b497fc8beff1c9fb319e3b4b62e22135e8e8d81506ede3ca51365887947a8571`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 4.8 MB (4784535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbc2e7980e0793ef96d07cc5a7d9418109519d7d6982ba49570b90d02b2932c`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.24-nanoserver`

```console
$ docker pull nats@sha256:1ad695d981e825ae558a90d280eff8792fd369346b2ea64dff57c1d3ce8e5c28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.9.24-nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:73f5d1f23c60e8c64bea6d8e55905285d30fa448f7ade9f8597a2d00a3d27ce4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109832813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:760507fd1783c222411869a2c4984d6a7c25c9d95988192a123e33bd1c414f11`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Nov 2023 05:11:01 GMT
RUN cmd /S /C #(nop) COPY file:bb76bb5eb2960343e0d31314ed4649c426ed59ad3d060057e2c1038e39265b76 in C:\nats-server.exe 
# Thu, 16 Nov 2023 05:11:02 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Nov 2023 05:11:03 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Nov 2023 05:11:03 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Nov 2023 05:11:04 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ac187e96a930e789fbdb3f3db19e7bb86f976983a562cd0521cea11347081e`  
		Last Modified: Thu, 16 Nov 2023 05:12:32 GMT  
		Size: 5.3 MB (5328972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9411de359e9c869b82c760e0e711247a49a4f058e2af773d6dd88260a68676d1`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea6582c6c01cd47f9f93a5ab8ebdf0e7d2bb4e444102237dc7b1d065928549b`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166ef556e54aaa80a6793bd63fdb796202e73717cb42a0e92586c8359b032f79`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d79fe9949ea94463332152fddb029659945f9beb57010148579273228d8935`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.24-nanoserver-1809`

```console
$ docker pull nats@sha256:1ad695d981e825ae558a90d280eff8792fd369346b2ea64dff57c1d3ce8e5c28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.9.24-nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:73f5d1f23c60e8c64bea6d8e55905285d30fa448f7ade9f8597a2d00a3d27ce4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109832813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:760507fd1783c222411869a2c4984d6a7c25c9d95988192a123e33bd1c414f11`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Nov 2023 05:11:01 GMT
RUN cmd /S /C #(nop) COPY file:bb76bb5eb2960343e0d31314ed4649c426ed59ad3d060057e2c1038e39265b76 in C:\nats-server.exe 
# Thu, 16 Nov 2023 05:11:02 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Nov 2023 05:11:03 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Nov 2023 05:11:03 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Nov 2023 05:11:04 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ac187e96a930e789fbdb3f3db19e7bb86f976983a562cd0521cea11347081e`  
		Last Modified: Thu, 16 Nov 2023 05:12:32 GMT  
		Size: 5.3 MB (5328972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9411de359e9c869b82c760e0e711247a49a4f058e2af773d6dd88260a68676d1`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea6582c6c01cd47f9f93a5ab8ebdf0e7d2bb4e444102237dc7b1d065928549b`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166ef556e54aaa80a6793bd63fdb796202e73717cb42a0e92586c8359b032f79`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d79fe9949ea94463332152fddb029659945f9beb57010148579273228d8935`  
		Last Modified: Thu, 16 Nov 2023 05:12:31 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.24-scratch`

```console
$ docker pull nats@sha256:92f7e9aef076cfefd13b8ceee7d3c2e603be5a9751c4fa686b9e1595422d97a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.24-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ca5325d2a2c84eca8c4f3e3ba96a4fcf6dc91e97e3d3ebd3bae69f7a126c0e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5248367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea934ed1a17a93225092fac66c8b617c594ecec00debda4eb753479eeadedab2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:c3d82eee52a26292cc80755a2b88f8b80cef5c80fd438c99768cd1c33ca95a9d in /nats-server 
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:22:59 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:22:59 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:22:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44811b84801c95891b1ccde13fe7e76a1ffd8795cd2a066ac0630ee836c23c2e`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 5.2 MB (5247859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927d64e5da79549425963bee122f44117e41eaa442b01673188effd14c9b236`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d3ccb1b790e4433d69872d7ddb8377aac40d6f000a66fa5b2795a62122a4f54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4984842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f1a1ecd1b37c66268f966a88d26fa44b35f70909dedab19c60bfd5aca2035e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:401de119a9fad5bd89c70f5a4d5c70f110d490ae5ab9aa60a7f963686ab297ee in /nats-server 
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:49:29 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f1d2c1b6f013f4386e7235452bc47cebd8001115c3a6504b418ee5b90071492a`  
		Last Modified: Wed, 08 Nov 2023 19:50:14 GMT  
		Size: 5.0 MB (4984334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5fea0f4bcfa87853f77179e249f0a8a09723aeb1c53882e3036fa6250a4ff5`  
		Last Modified: Wed, 08 Nov 2023 19:50:13 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:c73b24d4fb1ad910ad2f2bdefe0d18bfec11431afb4da9e3cd2be176e4fd49b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4977978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfe5b4a001ee28a1308edc00242441032b2afb69148c7ba17f692f75e2c1dba`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:cd8c3bf2b10d14de1f76a0617be080153909dadcd658bb62cab16d41a650d3de in /nats-server 
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:57:47 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:57:47 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:57:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e2a0a8d03803b71ab2e1e3540de965b9430b493bbd15bb2cb1372a7dd564c76d`  
		Last Modified: Wed, 08 Nov 2023 19:58:32 GMT  
		Size: 5.0 MB (4977470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe9df0b73b8b228e9331792251ba43d36af5e4e898411b4f9b725bb8928231`  
		Last Modified: Wed, 08 Nov 2023 19:58:31 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.24-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:770e514bf6ca4d8b056bd9d16b7df5f56c45c587ce3c815515051b6588e38325
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4785043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75bc6347feea13831461567c92c52c13e9085417ef409fb74364cf63105e346`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:40:10 GMT
COPY file:209cf40c58f80a36d8d8c8060f48a598dcf03ae451d8d658f267d02f3ce7bddc in /nats-server 
# Wed, 08 Nov 2023 19:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:40:11 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:40:11 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:40:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b497fc8beff1c9fb319e3b4b62e22135e8e8d81506ede3ca51365887947a8571`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 4.8 MB (4784535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbc2e7980e0793ef96d07cc5a7d9418109519d7d6982ba49570b90d02b2932c`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.24-windowsservercore`

```console
$ docker pull nats@sha256:b1e446a786a171431a795c1fa47128cacda24f39e0a7573a81959cbf2af4701e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.9.24-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:738db334d9d9b1f12a02ea151d9c48e0979703e801563bcf4e10d409d2d84172
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063502948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c10ef44f34cf615be280ea2fb6a99b60935a13a82fd8594ff2a80647ac91f420`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Nov 2023 05:07:47 GMT
ENV NATS_SERVER=2.9.24
# Thu, 16 Nov 2023 05:07:48 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.24/nats-server-v2.9.24-windows-amd64.zip
# Thu, 16 Nov 2023 05:07:49 GMT
ENV NATS_SERVER_SHASUM=4caa027910bfa0a79f2d1c01739e356df37dae15f1336174d459d2fd3a0e10d2
# Thu, 16 Nov 2023 05:08:53 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Nov 2023 05:10:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Nov 2023 05:10:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Nov 2023 05:10:39 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Nov 2023 05:10:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Nov 2023 05:10:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c35ae5a263cc82b97d893eece2f8371e8a0ad891752ccd514458fe125e1295`  
		Last Modified: Thu, 16 Nov 2023 05:12:21 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a68baad997636ffebee461869c70b5306f4dd52f21331e0586fff15e010659`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e56791fa6e91c6a1f2cec1bd459b01a184383d5ffc47cfff520d64f78f909a`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d6b958512faa97adacdb786dc3b6b2801ddeff298fd54a9be9279a625c993a`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 443.1 KB (443149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400de512823b4dd5067aeae94ba2b310e89bed83ff1730276164c6345459dc75`  
		Last Modified: Thu, 16 Nov 2023 05:12:19 GMT  
		Size: 5.6 MB (5615206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f93aaac049b5611b016e56ddddc1aec80f677513bd2506b0df17819e591e114`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 2.0 KB (1981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e740c0ab523cb4e1f0e60000a1a8da03fb645e9219eaf4cbbc8744134d83be`  
		Last Modified: Thu, 16 Nov 2023 05:12:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63012bc0bbc7f34223f89862b35418d4c72c8cfb1b43e4c97c09bd83d1dc43`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aab02fc5cc3eed11d240652a86121dff960e443a8f2538ebfaa9abf846d48d`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.24-windowsservercore-1809`

```console
$ docker pull nats@sha256:b1e446a786a171431a795c1fa47128cacda24f39e0a7573a81959cbf2af4701e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.9.24-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:738db334d9d9b1f12a02ea151d9c48e0979703e801563bcf4e10d409d2d84172
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063502948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c10ef44f34cf615be280ea2fb6a99b60935a13a82fd8594ff2a80647ac91f420`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Nov 2023 05:07:47 GMT
ENV NATS_SERVER=2.9.24
# Thu, 16 Nov 2023 05:07:48 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.24/nats-server-v2.9.24-windows-amd64.zip
# Thu, 16 Nov 2023 05:07:49 GMT
ENV NATS_SERVER_SHASUM=4caa027910bfa0a79f2d1c01739e356df37dae15f1336174d459d2fd3a0e10d2
# Thu, 16 Nov 2023 05:08:53 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Nov 2023 05:10:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Nov 2023 05:10:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Nov 2023 05:10:39 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Nov 2023 05:10:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Nov 2023 05:10:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c35ae5a263cc82b97d893eece2f8371e8a0ad891752ccd514458fe125e1295`  
		Last Modified: Thu, 16 Nov 2023 05:12:21 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a68baad997636ffebee461869c70b5306f4dd52f21331e0586fff15e010659`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e56791fa6e91c6a1f2cec1bd459b01a184383d5ffc47cfff520d64f78f909a`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d6b958512faa97adacdb786dc3b6b2801ddeff298fd54a9be9279a625c993a`  
		Last Modified: Thu, 16 Nov 2023 05:12:20 GMT  
		Size: 443.1 KB (443149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400de512823b4dd5067aeae94ba2b310e89bed83ff1730276164c6345459dc75`  
		Last Modified: Thu, 16 Nov 2023 05:12:19 GMT  
		Size: 5.6 MB (5615206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f93aaac049b5611b016e56ddddc1aec80f677513bd2506b0df17819e591e114`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 2.0 KB (1981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e740c0ab523cb4e1f0e60000a1a8da03fb645e9219eaf4cbbc8744134d83be`  
		Last Modified: Thu, 16 Nov 2023 05:12:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63012bc0bbc7f34223f89862b35418d4c72c8cfb1b43e4c97c09bd83d1dc43`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aab02fc5cc3eed11d240652a86121dff960e443a8f2538ebfaa9abf846d48d`  
		Last Modified: Thu, 16 Nov 2023 05:12:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:b196b3729c3c8ceb8c4b7192d7be08520dfd17c42377322a4027b889bcb61d50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:280f97fc32445b7fbf78d249c8e08a78508600838b36b8633b08eed6c8e11b4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9516956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13309d27201a23f166d402964c2bc26937570c70c1ef85ba960d3e4171b6bb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 22:22:47 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:22:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 22:22:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 22:22:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3e725fa689593464ef203de1b06f2e55491fa077b59b693fd9e1ef8c249dd`  
		Last Modified: Fri, 01 Dec 2023 22:23:35 GMT  
		Size: 6.1 MB (6113534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ede37fe98c391207efb9e57a4e29197e178cd9afdafac3140fcf8e44aecc62b`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9177007628f506dd880c66a174348504e4589a3cd156d8377b4278242ffefb9c`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f9a012265e9ab4e95584f7ea9f4f78234e048366873dcef81b1b46359e22d9f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce4db94168c70869897e9c0941e0567f3ce732d60f92f80ef605d765d9c9686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:49:22 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:49:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:49:25 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9345d2089731ee6f2e92bf32245d1665e8357fecf55c50e9a428966a109c4ed`  
		Last Modified: Fri, 01 Dec 2023 21:50:01 GMT  
		Size: 5.8 MB (5827544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569cb676c86b2aeb776ffd80a904ac5e9bdcda8bea7c0684872fba5efc4b8007`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23edb8dc9637ca24330de881d8e57e7f369ebd6b7b100db2dbae3aff15d50f29`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d6be8cbc263e2393e2d5f07d4b579c143dada13fe2dd8966097c11e9a1ddc178
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c00554cdbce58cc9a6a11ca1b37f5b90932f2c7bc9b55f096f26b93ba240a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:57:27 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:57:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:57:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8756919eccb97dc6990af357a87c8ba743e3a3ee7ad6d8c8c3dc108620e3c`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 5.8 MB (5818288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55307c3335ece26e2e60bb611f614f94af63814be706d6b3394d9691f55e7f82`  
		Last Modified: Fri, 01 Dec 2023 21:58:15 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7195a7938dcaa9bf7c4b89602950f827640c5bbecbb4a4f858b6a846f6719b`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ecd307e2f9675cf866313820a53a82b1a1459cf04a50da39b145b79360877119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9018304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e350d93fb277376b154a1cc0e44e75d36e34a479bea66c1186b2ef6ce5ec9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:39:48 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:39:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:39:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099335ae91609137f74432a77e75ffc1877279b74582260fc094104662cc3707`  
		Last Modified: Fri, 01 Dec 2023 21:40:50 GMT  
		Size: 5.7 MB (5684273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10e033372c9ea54711e4453250cd168911b0b43394e197c03164fcab8331f7`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9486420e5d0bd9ffaf1e3828a6eec84d98d97415b6fe70f65534ff451b2c61`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.18`

```console
$ docker pull nats@sha256:b196b3729c3c8ceb8c4b7192d7be08520dfd17c42377322a4027b889bcb61d50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:280f97fc32445b7fbf78d249c8e08a78508600838b36b8633b08eed6c8e11b4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9516956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13309d27201a23f166d402964c2bc26937570c70c1ef85ba960d3e4171b6bb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 22:22:47 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:22:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 22:22:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 22:22:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 22:22:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3e725fa689593464ef203de1b06f2e55491fa077b59b693fd9e1ef8c249dd`  
		Last Modified: Fri, 01 Dec 2023 22:23:35 GMT  
		Size: 6.1 MB (6113534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ede37fe98c391207efb9e57a4e29197e178cd9afdafac3140fcf8e44aecc62b`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9177007628f506dd880c66a174348504e4589a3cd156d8377b4278242ffefb9c`  
		Last Modified: Fri, 01 Dec 2023 22:23:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:f9a012265e9ab4e95584f7ea9f4f78234e048366873dcef81b1b46359e22d9f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce4db94168c70869897e9c0941e0567f3ce732d60f92f80ef605d765d9c9686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:49:22 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:49:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:49:25 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9345d2089731ee6f2e92bf32245d1665e8357fecf55c50e9a428966a109c4ed`  
		Last Modified: Fri, 01 Dec 2023 21:50:01 GMT  
		Size: 5.8 MB (5827544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569cb676c86b2aeb776ffd80a904ac5e9bdcda8bea7c0684872fba5efc4b8007`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23edb8dc9637ca24330de881d8e57e7f369ebd6b7b100db2dbae3aff15d50f29`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:d6be8cbc263e2393e2d5f07d4b579c143dada13fe2dd8966097c11e9a1ddc178
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c00554cdbce58cc9a6a11ca1b37f5b90932f2c7bc9b55f096f26b93ba240a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:57:27 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:57:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:57:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8756919eccb97dc6990af357a87c8ba743e3a3ee7ad6d8c8c3dc108620e3c`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 5.8 MB (5818288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55307c3335ece26e2e60bb611f614f94af63814be706d6b3394d9691f55e7f82`  
		Last Modified: Fri, 01 Dec 2023 21:58:15 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7195a7938dcaa9bf7c4b89602950f827640c5bbecbb4a4f858b6a846f6719b`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ecd307e2f9675cf866313820a53a82b1a1459cf04a50da39b145b79360877119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9018304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e350d93fb277376b154a1cc0e44e75d36e34a479bea66c1186b2ef6ce5ec9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:39:48 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:39:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:39:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099335ae91609137f74432a77e75ffc1877279b74582260fc094104662cc3707`  
		Last Modified: Fri, 01 Dec 2023 21:40:50 GMT  
		Size: 5.7 MB (5684273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10e033372c9ea54711e4453250cd168911b0b43394e197c03164fcab8331f7`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9486420e5d0bd9ffaf1e3828a6eec84d98d97415b6fe70f65534ff451b2c61`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:195df15e1f52f94fd5ca9120c099d64f7ed1ced5f2f7941ed658263e5c2c7530
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.5122; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:ca5325d2a2c84eca8c4f3e3ba96a4fcf6dc91e97e3d3ebd3bae69f7a126c0e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5248367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea934ed1a17a93225092fac66c8b617c594ecec00debda4eb753479eeadedab2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:c3d82eee52a26292cc80755a2b88f8b80cef5c80fd438c99768cd1c33ca95a9d in /nats-server 
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:22:59 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:22:59 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:22:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44811b84801c95891b1ccde13fe7e76a1ffd8795cd2a066ac0630ee836c23c2e`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 5.2 MB (5247859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927d64e5da79549425963bee122f44117e41eaa442b01673188effd14c9b236`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d3ccb1b790e4433d69872d7ddb8377aac40d6f000a66fa5b2795a62122a4f54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4984842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f1a1ecd1b37c66268f966a88d26fa44b35f70909dedab19c60bfd5aca2035e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:401de119a9fad5bd89c70f5a4d5c70f110d490ae5ab9aa60a7f963686ab297ee in /nats-server 
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:49:29 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f1d2c1b6f013f4386e7235452bc47cebd8001115c3a6504b418ee5b90071492a`  
		Last Modified: Wed, 08 Nov 2023 19:50:14 GMT  
		Size: 5.0 MB (4984334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5fea0f4bcfa87853f77179e249f0a8a09723aeb1c53882e3036fa6250a4ff5`  
		Last Modified: Wed, 08 Nov 2023 19:50:13 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:c73b24d4fb1ad910ad2f2bdefe0d18bfec11431afb4da9e3cd2be176e4fd49b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4977978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfe5b4a001ee28a1308edc00242441032b2afb69148c7ba17f692f75e2c1dba`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:cd8c3bf2b10d14de1f76a0617be080153909dadcd658bb62cab16d41a650d3de in /nats-server 
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:57:47 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:57:47 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:57:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e2a0a8d03803b71ab2e1e3540de965b9430b493bbd15bb2cb1372a7dd564c76d`  
		Last Modified: Wed, 08 Nov 2023 19:58:32 GMT  
		Size: 5.0 MB (4977470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe9df0b73b8b228e9331792251ba43d36af5e4e898411b4f9b725bb8928231`  
		Last Modified: Wed, 08 Nov 2023 19:58:31 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:770e514bf6ca4d8b056bd9d16b7df5f56c45c587ce3c815515051b6588e38325
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4785043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75bc6347feea13831461567c92c52c13e9085417ef409fb74364cf63105e346`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:40:10 GMT
COPY file:209cf40c58f80a36d8d8c8060f48a598dcf03ae451d8d658f267d02f3ce7bddc in /nats-server 
# Wed, 08 Nov 2023 19:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:40:11 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:40:11 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:40:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b497fc8beff1c9fb319e3b4b62e22135e8e8d81506ede3ca51365887947a8571`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 4.8 MB (4784535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbc2e7980e0793ef96d07cc5a7d9418109519d7d6982ba49570b90d02b2932c`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:87853cd90752f3d33c3a31b152a11a2b9a7736f4a736218a570495225fcbecba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:cb6e962ac8351dd9c57425e277ee4df9a1891ceb36b91f96de71bcb32e5b7f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:cb6e962ac8351dd9c57425e277ee4df9a1891ceb36b91f96de71bcb32e5b7f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:87853cd90752f3d33c3a31b152a11a2b9a7736f4a736218a570495225fcbecba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:08736b7bca092c65364463111c9e7ba1fa37c595535b6cee6f69399710b9ab64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5491281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb6445a6b2655117a39791c0c613a9359a39b7813f989e2dbb7858da97fed0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:433da15adc36332f81e7a6d340f8c6f7cfba5f7ec245f69b806b0daf2cc596f6 in /nats-server 
# Fri, 01 Dec 2023 22:23:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 22:23:09 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:23:09 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 22:23:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:76e55d4ff48d1bffd139ee6ffa81e1edd9b815ffc3157b448c352ecf7d29750e`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 5.5 MB (5490773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc83c20ac9045f4cc04f9c3b20bf8eb44b63ce0655d42c074ff0643045aac853`  
		Last Modified: Fri, 01 Dec 2023 22:23:58 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:2635baef88f485e3e6c943dab77da02ccdfbaa09a4cf45a6cade2b95132aa291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:a615001ea716034c1ae2e5cbb7989e5d4b89aa83346c9bfa2c353194009f4c2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063764344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d4d13ef10f01fd53dab0e60ac169100d104101183a8b7564de4a935c98ce88`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:15:41 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:15:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.6/nats-server-v2.10.6-windows-amd64.zip
# Fri, 01 Dec 2023 22:15:43 GMT
ENV NATS_SERVER_SHASUM=8084fc5fc16fa099fae0bb2f74dcf077ab644310918cc16e68b9909330ac798b
# Fri, 01 Dec 2023 22:16:45 GMT
RUN Set-PSDebug -Trace 2
# Fri, 01 Dec 2023 22:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 01 Dec 2023 22:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482d1334c03f2dfeab20b372b19d03e4af7be1261b4b2c858cfa969d0f17c33f`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7056bd68c3f6a5bc1bfdfe4fd9aba9d36b5fa4490e1fa5856be9a04ae3e44a`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c875fab524e257138d947d0cc33bc83d5f79ddf950d886b48f307180daa7d3`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fecdb4839d326ad445940782e3c9036f5487a2f47c185e8682652ec5e049b32`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 437.1 KB (437133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc25e0a531b65458953a005d8f1426da0383911a7e6129de254b037f7a60244b`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 5.9 MB (5882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd9cd8a4c0fd879700f6adde2f07b9c978036ed06509a537e8e9e2327d1974`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5f74a80810732f5daca2a35b749a9c1e0fc520a8fb994930694a05ae073fa2`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cac74b0b7cc9e03fb9c78c17f45ed3e4153089be3dba95e03d5230d8e6336c4`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d9d2aa7f0e9065f683eaa5fcf692b200162ecce3161afef9e766e9a332ed53`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:2635baef88f485e3e6c943dab77da02ccdfbaa09a4cf45a6cade2b95132aa291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:a615001ea716034c1ae2e5cbb7989e5d4b89aa83346c9bfa2c353194009f4c2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063764344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d4d13ef10f01fd53dab0e60ac169100d104101183a8b7564de4a935c98ce88`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:04:35 GMT
ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:15:41 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 22:15:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.6/nats-server-v2.10.6-windows-amd64.zip
# Fri, 01 Dec 2023 22:15:43 GMT
ENV NATS_SERVER_SHASUM=8084fc5fc16fa099fae0bb2f74dcf077ab644310918cc16e68b9909330ac798b
# Fri, 01 Dec 2023 22:16:45 GMT
RUN Set-PSDebug -Trace 2
# Fri, 01 Dec 2023 22:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 01 Dec 2023 22:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b0af12f04914a99bd0e5616b75c205f8a22c3c23bb3e13ea8fb557b765ec1`  
		Last Modified: Thu, 16 Nov 2023 05:11:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482d1334c03f2dfeab20b372b19d03e4af7be1261b4b2c858cfa969d0f17c33f`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7056bd68c3f6a5bc1bfdfe4fd9aba9d36b5fa4490e1fa5856be9a04ae3e44a`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c875fab524e257138d947d0cc33bc83d5f79ddf950d886b48f307180daa7d3`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fecdb4839d326ad445940782e3c9036f5487a2f47c185e8682652ec5e049b32`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 437.1 KB (437133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc25e0a531b65458953a005d8f1426da0383911a7e6129de254b037f7a60244b`  
		Last Modified: Fri, 01 Dec 2023 22:19:42 GMT  
		Size: 5.9 MB (5882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd9cd8a4c0fd879700f6adde2f07b9c978036ed06509a537e8e9e2327d1974`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5f74a80810732f5daca2a35b749a9c1e0fc520a8fb994930694a05ae073fa2`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cac74b0b7cc9e03fb9c78c17f45ed3e4153089be3dba95e03d5230d8e6336c4`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d9d2aa7f0e9065f683eaa5fcf692b200162ecce3161afef9e766e9a332ed53`  
		Last Modified: Fri, 01 Dec 2023 22:19:40 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
