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
-	[`nats:2.10.7`](#nats2107)
-	[`nats:2.10.7-alpine`](#nats2107-alpine)
-	[`nats:2.10.7-alpine3.18`](#nats2107-alpine318)
-	[`nats:2.10.7-linux`](#nats2107-linux)
-	[`nats:2.10.7-nanoserver`](#nats2107-nanoserver)
-	[`nats:2.10.7-nanoserver-1809`](#nats2107-nanoserver-1809)
-	[`nats:2.10.7-scratch`](#nats2107-scratch)
-	[`nats:2.10.7-windowsservercore`](#nats2107-windowsservercore)
-	[`nats:2.10.7-windowsservercore-1809`](#nats2107-windowsservercore-1809)
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
$ docker pull nats@sha256:fa3249082b1d9848f63052b9b34e32560363ddc7dc60ca495ceaa123f6398682
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
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
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
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
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
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
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
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
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
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:1bcddab51b8099aad943e1e558d9aa7e91000ebc6e08e308e8e95fa3b50a000b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:e69ea3ea129b75663ef1fbf6f6b66c6065924b8648ceaff49fc1a6d243c07e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9513446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0ce66e0a46e1088055a51a8dae2234f13808213f4a7fae6f9c2475d3989849`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:19:48 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:19:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:19:50 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:19:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd45941c5ec4c89954590450598e97bff29acdd357abb9550c2a4225bf2919b`  
		Last Modified: Thu, 07 Dec 2023 01:20:28 GMT  
		Size: 6.1 MB (6110026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05a83670934c18d8eac79cf05ec48cb635976d0c5b05a80d36624b3ed45de0f`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc87433b72bc5915d420aeb8d253e934c34c2cf9c799c6b7e284c51828d3d5bc`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5646f5ce83a2cd0809dd62b9103aba3eff6bca2666965032ae01c1425f4c01c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17c0157045551d25e73637159044fae84067bde183e05d0099b9b806299b456`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:49:19 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:49:22 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:49:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b743b5e93d5fde059f514131d51e22a1a4eef1fe4e71d4e42c7fdfc960da9`  
		Last Modified: Thu, 07 Dec 2023 00:49:56 GMT  
		Size: 5.8 MB (5827875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3b83a38bf1009764f2673fbcfe66e38ba7d57492c7838790e767319e64c961`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b6d8395d698e101d9e4936dee08916549133753cd0672eceac8ddf1190193a`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:319339bfeb0f92227088c3f5cfd3e56981fa3b186d5116cfdf4226d2460a35fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d237f0362b1780eafc23b2167a400bc9263e907cee8681711608e8a81f74cd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:57:29 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:57:32 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:57:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d98699d8052dfaae7fe949909d4441e7ffa65f121292863ba744dcb835df5`  
		Last Modified: Thu, 07 Dec 2023 00:58:14 GMT  
		Size: 5.8 MB (5818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754b91893810a1324476d59ae9f561401be2dd7ae77503a7d84e5e7a5056f8d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4969653e0f6db6b3f49cb0add7efde0f957fd2bc0fdd0f1511497bdc1a319e5d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b15737ca63cfd9058c019e1e3629c6655614f31e714e9fd84486db46e329898a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9017177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8125695217877ea76b44823e899852e278bde87b6be46df0e6e7b4f102523b85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:39:45 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:39:48 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70b7823ba2376fcc84abc44ad7f9720179b98305c2017783138c0f06808474`  
		Last Modified: Thu, 07 Dec 2023 01:40:17 GMT  
		Size: 5.7 MB (5683145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e121e16458b01c2d4edc959e8e775003249211345b7232cb2e75addf9c7e8c9`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ee96be4397da1a71d6c88c196a0533aaac25fa9ccd07978c09185d1ff3be3f`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.18`

```console
$ docker pull nats@sha256:1bcddab51b8099aad943e1e558d9aa7e91000ebc6e08e308e8e95fa3b50a000b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:e69ea3ea129b75663ef1fbf6f6b66c6065924b8648ceaff49fc1a6d243c07e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9513446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0ce66e0a46e1088055a51a8dae2234f13808213f4a7fae6f9c2475d3989849`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:19:48 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:19:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:19:50 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:19:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd45941c5ec4c89954590450598e97bff29acdd357abb9550c2a4225bf2919b`  
		Last Modified: Thu, 07 Dec 2023 01:20:28 GMT  
		Size: 6.1 MB (6110026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05a83670934c18d8eac79cf05ec48cb635976d0c5b05a80d36624b3ed45de0f`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc87433b72bc5915d420aeb8d253e934c34c2cf9c799c6b7e284c51828d3d5bc`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:5646f5ce83a2cd0809dd62b9103aba3eff6bca2666965032ae01c1425f4c01c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17c0157045551d25e73637159044fae84067bde183e05d0099b9b806299b456`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:49:19 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:49:22 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:49:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b743b5e93d5fde059f514131d51e22a1a4eef1fe4e71d4e42c7fdfc960da9`  
		Last Modified: Thu, 07 Dec 2023 00:49:56 GMT  
		Size: 5.8 MB (5827875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3b83a38bf1009764f2673fbcfe66e38ba7d57492c7838790e767319e64c961`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b6d8395d698e101d9e4936dee08916549133753cd0672eceac8ddf1190193a`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:319339bfeb0f92227088c3f5cfd3e56981fa3b186d5116cfdf4226d2460a35fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d237f0362b1780eafc23b2167a400bc9263e907cee8681711608e8a81f74cd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:57:29 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:57:32 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:57:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d98699d8052dfaae7fe949909d4441e7ffa65f121292863ba744dcb835df5`  
		Last Modified: Thu, 07 Dec 2023 00:58:14 GMT  
		Size: 5.8 MB (5818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754b91893810a1324476d59ae9f561401be2dd7ae77503a7d84e5e7a5056f8d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4969653e0f6db6b3f49cb0add7efde0f957fd2bc0fdd0f1511497bdc1a319e5d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b15737ca63cfd9058c019e1e3629c6655614f31e714e9fd84486db46e329898a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9017177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8125695217877ea76b44823e899852e278bde87b6be46df0e6e7b4f102523b85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:39:45 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:39:48 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70b7823ba2376fcc84abc44ad7f9720179b98305c2017783138c0f06808474`  
		Last Modified: Thu, 07 Dec 2023 01:40:17 GMT  
		Size: 5.7 MB (5683145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e121e16458b01c2d4edc959e8e775003249211345b7232cb2e75addf9c7e8c9`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ee96be4397da1a71d6c88c196a0533aaac25fa9ccd07978c09185d1ff3be3f`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:931a11845ed5070cb0168a7fd3a00d4644d2209377bcc56f24f9303e666d8bbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:7e5a1765845a818e657063bc693b2890b02f7860c7355f18618ecc568d6632a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:7e5a1765845a818e657063bc693b2890b02f7860c7355f18618ecc568d6632a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:931a11845ed5070cb0168a7fd3a00d4644d2209377bcc56f24f9303e666d8bbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:2b40aace744d62020f81af24776d9ea3dd7b2db51349c5406ad523e1b9652377
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:0a7b1f4d4d84dcdc6cc26f0f7b36bbad44f1d76f893f5099388b3e7dbf79c04d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063795480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c0fd2ef82c44707660bb251a3bafe1a35f1b97545d74473ede708e72ce0db3`
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
# Thu, 07 Dec 2023 01:15:40 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.7/nats-server-v2.10.7-windows-amd64.zip
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_SHASUM=92c4883cdf608c1e096feabcc9a0f46935ba34fce72210520ba2e66207968630
# Thu, 07 Dec 2023 01:16:51 GMT
RUN Set-PSDebug -Trace 2
# Thu, 07 Dec 2023 01:18:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 07 Dec 2023 01:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:18:49 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:18:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:18:51 GMT
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
	-	`sha256:3c1b29fa38804640fd014da40f6bb75e1de186bb66e503d6dc478ac64d39d6a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae886b25b11d9b870221360719245f3035fab76cf0faaa9f35b83c5a988c076`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4f14d97a99af78f3a54e018e6e5b82fb0f3b679f827268ce64af2bccc10a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7562be7e5170234e29efc9b395bab01b599634555475888b80d9fe17eb7b8ce5`  
		Last Modified: Thu, 07 Dec 2023 01:20:02 GMT  
		Size: 456.2 KB (456182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c819e27d814e20a85d82d3ffdaa135668d42fe458c0c92bf7bbb1996f9e0f7f`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 5.9 MB (5894412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0c017084ce6a109713ed27b606a834949b8cba3a8ce1dee07f9b6040efdcc4`  
		Last Modified: Thu, 07 Dec 2023 01:20:00 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ff897097cbb7915114d4ef345cbc328556d21d0fbbe23fefd0a35c6be46c4d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70c738db124696f5d5cfa249a781c74abbac5f2b3e007322c51e816fd21a87c`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe385c6d134add097dfcf0b0ed86918e1e63a23233004c6db0f5da4656de18d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:2b40aace744d62020f81af24776d9ea3dd7b2db51349c5406ad523e1b9652377
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:0a7b1f4d4d84dcdc6cc26f0f7b36bbad44f1d76f893f5099388b3e7dbf79c04d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063795480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c0fd2ef82c44707660bb251a3bafe1a35f1b97545d74473ede708e72ce0db3`
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
# Thu, 07 Dec 2023 01:15:40 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.7/nats-server-v2.10.7-windows-amd64.zip
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_SHASUM=92c4883cdf608c1e096feabcc9a0f46935ba34fce72210520ba2e66207968630
# Thu, 07 Dec 2023 01:16:51 GMT
RUN Set-PSDebug -Trace 2
# Thu, 07 Dec 2023 01:18:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 07 Dec 2023 01:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:18:49 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:18:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:18:51 GMT
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
	-	`sha256:3c1b29fa38804640fd014da40f6bb75e1de186bb66e503d6dc478ac64d39d6a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae886b25b11d9b870221360719245f3035fab76cf0faaa9f35b83c5a988c076`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4f14d97a99af78f3a54e018e6e5b82fb0f3b679f827268ce64af2bccc10a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7562be7e5170234e29efc9b395bab01b599634555475888b80d9fe17eb7b8ce5`  
		Last Modified: Thu, 07 Dec 2023 01:20:02 GMT  
		Size: 456.2 KB (456182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c819e27d814e20a85d82d3ffdaa135668d42fe458c0c92bf7bbb1996f9e0f7f`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 5.9 MB (5894412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0c017084ce6a109713ed27b606a834949b8cba3a8ce1dee07f9b6040efdcc4`  
		Last Modified: Thu, 07 Dec 2023 01:20:00 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ff897097cbb7915114d4ef345cbc328556d21d0fbbe23fefd0a35c6be46c4d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70c738db124696f5d5cfa249a781c74abbac5f2b3e007322c51e816fd21a87c`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe385c6d134add097dfcf0b0ed86918e1e63a23233004c6db0f5da4656de18d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10`

```console
$ docker pull nats@sha256:ec867ed0651048d6bbda1688fc0f8c409a74c571e7ee4b0763e2b31ed4e8685c
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
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-alpine`

```console
$ docker pull nats@sha256:1bcddab51b8099aad943e1e558d9aa7e91000ebc6e08e308e8e95fa3b50a000b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-alpine` - linux; amd64

```console
$ docker pull nats@sha256:e69ea3ea129b75663ef1fbf6f6b66c6065924b8648ceaff49fc1a6d243c07e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9513446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0ce66e0a46e1088055a51a8dae2234f13808213f4a7fae6f9c2475d3989849`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:19:48 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:19:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:19:50 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:19:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd45941c5ec4c89954590450598e97bff29acdd357abb9550c2a4225bf2919b`  
		Last Modified: Thu, 07 Dec 2023 01:20:28 GMT  
		Size: 6.1 MB (6110026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05a83670934c18d8eac79cf05ec48cb635976d0c5b05a80d36624b3ed45de0f`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc87433b72bc5915d420aeb8d253e934c34c2cf9c799c6b7e284c51828d3d5bc`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5646f5ce83a2cd0809dd62b9103aba3eff6bca2666965032ae01c1425f4c01c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17c0157045551d25e73637159044fae84067bde183e05d0099b9b806299b456`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:49:19 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:49:22 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:49:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b743b5e93d5fde059f514131d51e22a1a4eef1fe4e71d4e42c7fdfc960da9`  
		Last Modified: Thu, 07 Dec 2023 00:49:56 GMT  
		Size: 5.8 MB (5827875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3b83a38bf1009764f2673fbcfe66e38ba7d57492c7838790e767319e64c961`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b6d8395d698e101d9e4936dee08916549133753cd0672eceac8ddf1190193a`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:319339bfeb0f92227088c3f5cfd3e56981fa3b186d5116cfdf4226d2460a35fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d237f0362b1780eafc23b2167a400bc9263e907cee8681711608e8a81f74cd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:57:29 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:57:32 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:57:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d98699d8052dfaae7fe949909d4441e7ffa65f121292863ba744dcb835df5`  
		Last Modified: Thu, 07 Dec 2023 00:58:14 GMT  
		Size: 5.8 MB (5818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754b91893810a1324476d59ae9f561401be2dd7ae77503a7d84e5e7a5056f8d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4969653e0f6db6b3f49cb0add7efde0f957fd2bc0fdd0f1511497bdc1a319e5d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b15737ca63cfd9058c019e1e3629c6655614f31e714e9fd84486db46e329898a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9017177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8125695217877ea76b44823e899852e278bde87b6be46df0e6e7b4f102523b85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:39:45 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:39:48 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70b7823ba2376fcc84abc44ad7f9720179b98305c2017783138c0f06808474`  
		Last Modified: Thu, 07 Dec 2023 01:40:17 GMT  
		Size: 5.7 MB (5683145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e121e16458b01c2d4edc959e8e775003249211345b7232cb2e75addf9c7e8c9`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ee96be4397da1a71d6c88c196a0533aaac25fa9ccd07978c09185d1ff3be3f`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-alpine3.18`

```console
$ docker pull nats@sha256:1bcddab51b8099aad943e1e558d9aa7e91000ebc6e08e308e8e95fa3b50a000b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:e69ea3ea129b75663ef1fbf6f6b66c6065924b8648ceaff49fc1a6d243c07e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9513446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0ce66e0a46e1088055a51a8dae2234f13808213f4a7fae6f9c2475d3989849`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:19:48 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:19:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:19:50 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:19:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd45941c5ec4c89954590450598e97bff29acdd357abb9550c2a4225bf2919b`  
		Last Modified: Thu, 07 Dec 2023 01:20:28 GMT  
		Size: 6.1 MB (6110026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05a83670934c18d8eac79cf05ec48cb635976d0c5b05a80d36624b3ed45de0f`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc87433b72bc5915d420aeb8d253e934c34c2cf9c799c6b7e284c51828d3d5bc`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:5646f5ce83a2cd0809dd62b9103aba3eff6bca2666965032ae01c1425f4c01c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17c0157045551d25e73637159044fae84067bde183e05d0099b9b806299b456`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:49:19 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:49:22 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:49:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b743b5e93d5fde059f514131d51e22a1a4eef1fe4e71d4e42c7fdfc960da9`  
		Last Modified: Thu, 07 Dec 2023 00:49:56 GMT  
		Size: 5.8 MB (5827875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3b83a38bf1009764f2673fbcfe66e38ba7d57492c7838790e767319e64c961`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b6d8395d698e101d9e4936dee08916549133753cd0672eceac8ddf1190193a`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:319339bfeb0f92227088c3f5cfd3e56981fa3b186d5116cfdf4226d2460a35fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d237f0362b1780eafc23b2167a400bc9263e907cee8681711608e8a81f74cd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:57:29 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:57:32 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:57:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d98699d8052dfaae7fe949909d4441e7ffa65f121292863ba744dcb835df5`  
		Last Modified: Thu, 07 Dec 2023 00:58:14 GMT  
		Size: 5.8 MB (5818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754b91893810a1324476d59ae9f561401be2dd7ae77503a7d84e5e7a5056f8d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4969653e0f6db6b3f49cb0add7efde0f957fd2bc0fdd0f1511497bdc1a319e5d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b15737ca63cfd9058c019e1e3629c6655614f31e714e9fd84486db46e329898a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9017177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8125695217877ea76b44823e899852e278bde87b6be46df0e6e7b4f102523b85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:39:45 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:39:48 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70b7823ba2376fcc84abc44ad7f9720179b98305c2017783138c0f06808474`  
		Last Modified: Thu, 07 Dec 2023 01:40:17 GMT  
		Size: 5.7 MB (5683145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e121e16458b01c2d4edc959e8e775003249211345b7232cb2e75addf9c7e8c9`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ee96be4397da1a71d6c88c196a0533aaac25fa9ccd07978c09185d1ff3be3f`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-linux`

```console
$ docker pull nats@sha256:931a11845ed5070cb0168a7fd3a00d4644d2209377bcc56f24f9303e666d8bbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-linux` - linux; amd64

```console
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-nanoserver`

```console
$ docker pull nats@sha256:7e5a1765845a818e657063bc693b2890b02f7860c7355f18618ecc568d6632a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10-nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-nanoserver-1809`

```console
$ docker pull nats@sha256:7e5a1765845a818e657063bc693b2890b02f7860c7355f18618ecc568d6632a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10-nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-scratch`

```console
$ docker pull nats@sha256:931a11845ed5070cb0168a7fd3a00d4644d2209377bcc56f24f9303e666d8bbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-scratch` - linux; amd64

```console
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-windowsservercore`

```console
$ docker pull nats@sha256:2b40aace744d62020f81af24776d9ea3dd7b2db51349c5406ad523e1b9652377
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:0a7b1f4d4d84dcdc6cc26f0f7b36bbad44f1d76f893f5099388b3e7dbf79c04d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063795480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c0fd2ef82c44707660bb251a3bafe1a35f1b97545d74473ede708e72ce0db3`
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
# Thu, 07 Dec 2023 01:15:40 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.7/nats-server-v2.10.7-windows-amd64.zip
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_SHASUM=92c4883cdf608c1e096feabcc9a0f46935ba34fce72210520ba2e66207968630
# Thu, 07 Dec 2023 01:16:51 GMT
RUN Set-PSDebug -Trace 2
# Thu, 07 Dec 2023 01:18:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 07 Dec 2023 01:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:18:49 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:18:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:18:51 GMT
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
	-	`sha256:3c1b29fa38804640fd014da40f6bb75e1de186bb66e503d6dc478ac64d39d6a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae886b25b11d9b870221360719245f3035fab76cf0faaa9f35b83c5a988c076`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4f14d97a99af78f3a54e018e6e5b82fb0f3b679f827268ce64af2bccc10a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7562be7e5170234e29efc9b395bab01b599634555475888b80d9fe17eb7b8ce5`  
		Last Modified: Thu, 07 Dec 2023 01:20:02 GMT  
		Size: 456.2 KB (456182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c819e27d814e20a85d82d3ffdaa135668d42fe458c0c92bf7bbb1996f9e0f7f`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 5.9 MB (5894412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0c017084ce6a109713ed27b606a834949b8cba3a8ce1dee07f9b6040efdcc4`  
		Last Modified: Thu, 07 Dec 2023 01:20:00 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ff897097cbb7915114d4ef345cbc328556d21d0fbbe23fefd0a35c6be46c4d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70c738db124696f5d5cfa249a781c74abbac5f2b3e007322c51e816fd21a87c`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe385c6d134add097dfcf0b0ed86918e1e63a23233004c6db0f5da4656de18d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-windowsservercore-1809`

```console
$ docker pull nats@sha256:2b40aace744d62020f81af24776d9ea3dd7b2db51349c5406ad523e1b9652377
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:0a7b1f4d4d84dcdc6cc26f0f7b36bbad44f1d76f893f5099388b3e7dbf79c04d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063795480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c0fd2ef82c44707660bb251a3bafe1a35f1b97545d74473ede708e72ce0db3`
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
# Thu, 07 Dec 2023 01:15:40 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.7/nats-server-v2.10.7-windows-amd64.zip
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_SHASUM=92c4883cdf608c1e096feabcc9a0f46935ba34fce72210520ba2e66207968630
# Thu, 07 Dec 2023 01:16:51 GMT
RUN Set-PSDebug -Trace 2
# Thu, 07 Dec 2023 01:18:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 07 Dec 2023 01:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:18:49 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:18:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:18:51 GMT
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
	-	`sha256:3c1b29fa38804640fd014da40f6bb75e1de186bb66e503d6dc478ac64d39d6a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae886b25b11d9b870221360719245f3035fab76cf0faaa9f35b83c5a988c076`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4f14d97a99af78f3a54e018e6e5b82fb0f3b679f827268ce64af2bccc10a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7562be7e5170234e29efc9b395bab01b599634555475888b80d9fe17eb7b8ce5`  
		Last Modified: Thu, 07 Dec 2023 01:20:02 GMT  
		Size: 456.2 KB (456182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c819e27d814e20a85d82d3ffdaa135668d42fe458c0c92bf7bbb1996f9e0f7f`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 5.9 MB (5894412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0c017084ce6a109713ed27b606a834949b8cba3a8ce1dee07f9b6040efdcc4`  
		Last Modified: Thu, 07 Dec 2023 01:20:00 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ff897097cbb7915114d4ef345cbc328556d21d0fbbe23fefd0a35c6be46c4d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70c738db124696f5d5cfa249a781c74abbac5f2b3e007322c51e816fd21a87c`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe385c6d134add097dfcf0b0ed86918e1e63a23233004c6db0f5da4656de18d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.7`

```console
$ docker pull nats@sha256:ec867ed0651048d6bbda1688fc0f8c409a74c571e7ee4b0763e2b31ed4e8685c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10.7` - linux; amd64

```console
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.7-alpine`

```console
$ docker pull nats@sha256:1bcddab51b8099aad943e1e558d9aa7e91000ebc6e08e308e8e95fa3b50a000b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.7-alpine` - linux; amd64

```console
$ docker pull nats@sha256:e69ea3ea129b75663ef1fbf6f6b66c6065924b8648ceaff49fc1a6d243c07e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9513446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0ce66e0a46e1088055a51a8dae2234f13808213f4a7fae6f9c2475d3989849`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:19:48 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:19:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:19:50 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:19:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd45941c5ec4c89954590450598e97bff29acdd357abb9550c2a4225bf2919b`  
		Last Modified: Thu, 07 Dec 2023 01:20:28 GMT  
		Size: 6.1 MB (6110026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05a83670934c18d8eac79cf05ec48cb635976d0c5b05a80d36624b3ed45de0f`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc87433b72bc5915d420aeb8d253e934c34c2cf9c799c6b7e284c51828d3d5bc`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5646f5ce83a2cd0809dd62b9103aba3eff6bca2666965032ae01c1425f4c01c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17c0157045551d25e73637159044fae84067bde183e05d0099b9b806299b456`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:49:19 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:49:22 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:49:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b743b5e93d5fde059f514131d51e22a1a4eef1fe4e71d4e42c7fdfc960da9`  
		Last Modified: Thu, 07 Dec 2023 00:49:56 GMT  
		Size: 5.8 MB (5827875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3b83a38bf1009764f2673fbcfe66e38ba7d57492c7838790e767319e64c961`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b6d8395d698e101d9e4936dee08916549133753cd0672eceac8ddf1190193a`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:319339bfeb0f92227088c3f5cfd3e56981fa3b186d5116cfdf4226d2460a35fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d237f0362b1780eafc23b2167a400bc9263e907cee8681711608e8a81f74cd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:57:29 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:57:32 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:57:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d98699d8052dfaae7fe949909d4441e7ffa65f121292863ba744dcb835df5`  
		Last Modified: Thu, 07 Dec 2023 00:58:14 GMT  
		Size: 5.8 MB (5818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754b91893810a1324476d59ae9f561401be2dd7ae77503a7d84e5e7a5056f8d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4969653e0f6db6b3f49cb0add7efde0f957fd2bc0fdd0f1511497bdc1a319e5d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b15737ca63cfd9058c019e1e3629c6655614f31e714e9fd84486db46e329898a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9017177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8125695217877ea76b44823e899852e278bde87b6be46df0e6e7b4f102523b85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:39:45 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:39:48 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70b7823ba2376fcc84abc44ad7f9720179b98305c2017783138c0f06808474`  
		Last Modified: Thu, 07 Dec 2023 01:40:17 GMT  
		Size: 5.7 MB (5683145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e121e16458b01c2d4edc959e8e775003249211345b7232cb2e75addf9c7e8c9`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ee96be4397da1a71d6c88c196a0533aaac25fa9ccd07978c09185d1ff3be3f`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.7-alpine3.18`

```console
$ docker pull nats@sha256:1bcddab51b8099aad943e1e558d9aa7e91000ebc6e08e308e8e95fa3b50a000b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.7-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:e69ea3ea129b75663ef1fbf6f6b66c6065924b8648ceaff49fc1a6d243c07e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9513446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0ce66e0a46e1088055a51a8dae2234f13808213f4a7fae6f9c2475d3989849`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:19:48 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:19:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:19:50 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:19:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd45941c5ec4c89954590450598e97bff29acdd357abb9550c2a4225bf2919b`  
		Last Modified: Thu, 07 Dec 2023 01:20:28 GMT  
		Size: 6.1 MB (6110026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05a83670934c18d8eac79cf05ec48cb635976d0c5b05a80d36624b3ed45de0f`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc87433b72bc5915d420aeb8d253e934c34c2cf9c799c6b7e284c51828d3d5bc`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:5646f5ce83a2cd0809dd62b9103aba3eff6bca2666965032ae01c1425f4c01c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17c0157045551d25e73637159044fae84067bde183e05d0099b9b806299b456`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:49:19 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:49:22 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:49:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b743b5e93d5fde059f514131d51e22a1a4eef1fe4e71d4e42c7fdfc960da9`  
		Last Modified: Thu, 07 Dec 2023 00:49:56 GMT  
		Size: 5.8 MB (5827875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3b83a38bf1009764f2673fbcfe66e38ba7d57492c7838790e767319e64c961`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b6d8395d698e101d9e4936dee08916549133753cd0672eceac8ddf1190193a`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:319339bfeb0f92227088c3f5cfd3e56981fa3b186d5116cfdf4226d2460a35fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d237f0362b1780eafc23b2167a400bc9263e907cee8681711608e8a81f74cd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:57:29 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:57:32 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:57:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d98699d8052dfaae7fe949909d4441e7ffa65f121292863ba744dcb835df5`  
		Last Modified: Thu, 07 Dec 2023 00:58:14 GMT  
		Size: 5.8 MB (5818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754b91893810a1324476d59ae9f561401be2dd7ae77503a7d84e5e7a5056f8d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4969653e0f6db6b3f49cb0add7efde0f957fd2bc0fdd0f1511497bdc1a319e5d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b15737ca63cfd9058c019e1e3629c6655614f31e714e9fd84486db46e329898a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9017177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8125695217877ea76b44823e899852e278bde87b6be46df0e6e7b4f102523b85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:39:45 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:39:48 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70b7823ba2376fcc84abc44ad7f9720179b98305c2017783138c0f06808474`  
		Last Modified: Thu, 07 Dec 2023 01:40:17 GMT  
		Size: 5.7 MB (5683145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e121e16458b01c2d4edc959e8e775003249211345b7232cb2e75addf9c7e8c9`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ee96be4397da1a71d6c88c196a0533aaac25fa9ccd07978c09185d1ff3be3f`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.7-linux`

```console
$ docker pull nats@sha256:931a11845ed5070cb0168a7fd3a00d4644d2209377bcc56f24f9303e666d8bbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.7-linux` - linux; amd64

```console
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.7-nanoserver`

```console
$ docker pull nats@sha256:7e5a1765845a818e657063bc693b2890b02f7860c7355f18618ecc568d6632a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10.7-nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.7-nanoserver-1809`

```console
$ docker pull nats@sha256:7e5a1765845a818e657063bc693b2890b02f7860c7355f18618ecc568d6632a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10.7-nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.7-scratch`

```console
$ docker pull nats@sha256:931a11845ed5070cb0168a7fd3a00d4644d2209377bcc56f24f9303e666d8bbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.7-scratch` - linux; amd64

```console
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.7-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.7-windowsservercore`

```console
$ docker pull nats@sha256:2b40aace744d62020f81af24776d9ea3dd7b2db51349c5406ad523e1b9652377
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10.7-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:0a7b1f4d4d84dcdc6cc26f0f7b36bbad44f1d76f893f5099388b3e7dbf79c04d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063795480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c0fd2ef82c44707660bb251a3bafe1a35f1b97545d74473ede708e72ce0db3`
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
# Thu, 07 Dec 2023 01:15:40 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.7/nats-server-v2.10.7-windows-amd64.zip
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_SHASUM=92c4883cdf608c1e096feabcc9a0f46935ba34fce72210520ba2e66207968630
# Thu, 07 Dec 2023 01:16:51 GMT
RUN Set-PSDebug -Trace 2
# Thu, 07 Dec 2023 01:18:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 07 Dec 2023 01:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:18:49 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:18:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:18:51 GMT
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
	-	`sha256:3c1b29fa38804640fd014da40f6bb75e1de186bb66e503d6dc478ac64d39d6a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae886b25b11d9b870221360719245f3035fab76cf0faaa9f35b83c5a988c076`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4f14d97a99af78f3a54e018e6e5b82fb0f3b679f827268ce64af2bccc10a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7562be7e5170234e29efc9b395bab01b599634555475888b80d9fe17eb7b8ce5`  
		Last Modified: Thu, 07 Dec 2023 01:20:02 GMT  
		Size: 456.2 KB (456182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c819e27d814e20a85d82d3ffdaa135668d42fe458c0c92bf7bbb1996f9e0f7f`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 5.9 MB (5894412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0c017084ce6a109713ed27b606a834949b8cba3a8ce1dee07f9b6040efdcc4`  
		Last Modified: Thu, 07 Dec 2023 01:20:00 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ff897097cbb7915114d4ef345cbc328556d21d0fbbe23fefd0a35c6be46c4d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70c738db124696f5d5cfa249a781c74abbac5f2b3e007322c51e816fd21a87c`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe385c6d134add097dfcf0b0ed86918e1e63a23233004c6db0f5da4656de18d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.7-windowsservercore-1809`

```console
$ docker pull nats@sha256:2b40aace744d62020f81af24776d9ea3dd7b2db51349c5406ad523e1b9652377
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2.10.7-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:0a7b1f4d4d84dcdc6cc26f0f7b36bbad44f1d76f893f5099388b3e7dbf79c04d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063795480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c0fd2ef82c44707660bb251a3bafe1a35f1b97545d74473ede708e72ce0db3`
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
# Thu, 07 Dec 2023 01:15:40 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.7/nats-server-v2.10.7-windows-amd64.zip
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_SHASUM=92c4883cdf608c1e096feabcc9a0f46935ba34fce72210520ba2e66207968630
# Thu, 07 Dec 2023 01:16:51 GMT
RUN Set-PSDebug -Trace 2
# Thu, 07 Dec 2023 01:18:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 07 Dec 2023 01:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:18:49 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:18:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:18:51 GMT
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
	-	`sha256:3c1b29fa38804640fd014da40f6bb75e1de186bb66e503d6dc478ac64d39d6a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae886b25b11d9b870221360719245f3035fab76cf0faaa9f35b83c5a988c076`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4f14d97a99af78f3a54e018e6e5b82fb0f3b679f827268ce64af2bccc10a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7562be7e5170234e29efc9b395bab01b599634555475888b80d9fe17eb7b8ce5`  
		Last Modified: Thu, 07 Dec 2023 01:20:02 GMT  
		Size: 456.2 KB (456182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c819e27d814e20a85d82d3ffdaa135668d42fe458c0c92bf7bbb1996f9e0f7f`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 5.9 MB (5894412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0c017084ce6a109713ed27b606a834949b8cba3a8ce1dee07f9b6040efdcc4`  
		Last Modified: Thu, 07 Dec 2023 01:20:00 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ff897097cbb7915114d4ef345cbc328556d21d0fbbe23fefd0a35c6be46c4d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70c738db124696f5d5cfa249a781c74abbac5f2b3e007322c51e816fd21a87c`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe385c6d134add097dfcf0b0ed86918e1e63a23233004c6db0f5da4656de18d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1415 bytes)  
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
$ docker pull nats@sha256:1bcddab51b8099aad943e1e558d9aa7e91000ebc6e08e308e8e95fa3b50a000b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:e69ea3ea129b75663ef1fbf6f6b66c6065924b8648ceaff49fc1a6d243c07e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9513446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0ce66e0a46e1088055a51a8dae2234f13808213f4a7fae6f9c2475d3989849`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:19:48 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:19:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:19:50 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:19:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd45941c5ec4c89954590450598e97bff29acdd357abb9550c2a4225bf2919b`  
		Last Modified: Thu, 07 Dec 2023 01:20:28 GMT  
		Size: 6.1 MB (6110026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05a83670934c18d8eac79cf05ec48cb635976d0c5b05a80d36624b3ed45de0f`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc87433b72bc5915d420aeb8d253e934c34c2cf9c799c6b7e284c51828d3d5bc`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5646f5ce83a2cd0809dd62b9103aba3eff6bca2666965032ae01c1425f4c01c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17c0157045551d25e73637159044fae84067bde183e05d0099b9b806299b456`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:49:19 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:49:22 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:49:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b743b5e93d5fde059f514131d51e22a1a4eef1fe4e71d4e42c7fdfc960da9`  
		Last Modified: Thu, 07 Dec 2023 00:49:56 GMT  
		Size: 5.8 MB (5827875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3b83a38bf1009764f2673fbcfe66e38ba7d57492c7838790e767319e64c961`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b6d8395d698e101d9e4936dee08916549133753cd0672eceac8ddf1190193a`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:319339bfeb0f92227088c3f5cfd3e56981fa3b186d5116cfdf4226d2460a35fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d237f0362b1780eafc23b2167a400bc9263e907cee8681711608e8a81f74cd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:57:29 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:57:32 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:57:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d98699d8052dfaae7fe949909d4441e7ffa65f121292863ba744dcb835df5`  
		Last Modified: Thu, 07 Dec 2023 00:58:14 GMT  
		Size: 5.8 MB (5818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754b91893810a1324476d59ae9f561401be2dd7ae77503a7d84e5e7a5056f8d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4969653e0f6db6b3f49cb0add7efde0f957fd2bc0fdd0f1511497bdc1a319e5d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b15737ca63cfd9058c019e1e3629c6655614f31e714e9fd84486db46e329898a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9017177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8125695217877ea76b44823e899852e278bde87b6be46df0e6e7b4f102523b85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:39:45 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:39:48 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70b7823ba2376fcc84abc44ad7f9720179b98305c2017783138c0f06808474`  
		Last Modified: Thu, 07 Dec 2023 01:40:17 GMT  
		Size: 5.7 MB (5683145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e121e16458b01c2d4edc959e8e775003249211345b7232cb2e75addf9c7e8c9`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ee96be4397da1a71d6c88c196a0533aaac25fa9ccd07978c09185d1ff3be3f`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.18`

```console
$ docker pull nats@sha256:1bcddab51b8099aad943e1e558d9aa7e91000ebc6e08e308e8e95fa3b50a000b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:e69ea3ea129b75663ef1fbf6f6b66c6065924b8648ceaff49fc1a6d243c07e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9513446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0ce66e0a46e1088055a51a8dae2234f13808213f4a7fae6f9c2475d3989849`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:19:48 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:19:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:19:50 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:19:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd45941c5ec4c89954590450598e97bff29acdd357abb9550c2a4225bf2919b`  
		Last Modified: Thu, 07 Dec 2023 01:20:28 GMT  
		Size: 6.1 MB (6110026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05a83670934c18d8eac79cf05ec48cb635976d0c5b05a80d36624b3ed45de0f`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc87433b72bc5915d420aeb8d253e934c34c2cf9c799c6b7e284c51828d3d5bc`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:5646f5ce83a2cd0809dd62b9103aba3eff6bca2666965032ae01c1425f4c01c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17c0157045551d25e73637159044fae84067bde183e05d0099b9b806299b456`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:49:19 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:49:22 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:49:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b743b5e93d5fde059f514131d51e22a1a4eef1fe4e71d4e42c7fdfc960da9`  
		Last Modified: Thu, 07 Dec 2023 00:49:56 GMT  
		Size: 5.8 MB (5827875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3b83a38bf1009764f2673fbcfe66e38ba7d57492c7838790e767319e64c961`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b6d8395d698e101d9e4936dee08916549133753cd0672eceac8ddf1190193a`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:319339bfeb0f92227088c3f5cfd3e56981fa3b186d5116cfdf4226d2460a35fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d237f0362b1780eafc23b2167a400bc9263e907cee8681711608e8a81f74cd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:57:29 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:57:32 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:57:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d98699d8052dfaae7fe949909d4441e7ffa65f121292863ba744dcb835df5`  
		Last Modified: Thu, 07 Dec 2023 00:58:14 GMT  
		Size: 5.8 MB (5818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754b91893810a1324476d59ae9f561401be2dd7ae77503a7d84e5e7a5056f8d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4969653e0f6db6b3f49cb0add7efde0f957fd2bc0fdd0f1511497bdc1a319e5d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b15737ca63cfd9058c019e1e3629c6655614f31e714e9fd84486db46e329898a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9017177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8125695217877ea76b44823e899852e278bde87b6be46df0e6e7b4f102523b85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:39:45 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:39:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:39:48 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70b7823ba2376fcc84abc44ad7f9720179b98305c2017783138c0f06808474`  
		Last Modified: Thu, 07 Dec 2023 01:40:17 GMT  
		Size: 5.7 MB (5683145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e121e16458b01c2d4edc959e8e775003249211345b7232cb2e75addf9c7e8c9`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ee96be4397da1a71d6c88c196a0533aaac25fa9ccd07978c09185d1ff3be3f`  
		Last Modified: Thu, 07 Dec 2023 01:40:16 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:fa3249082b1d9848f63052b9b34e32560363ddc7dc60ca495ceaa123f6398682
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
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
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
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
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
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
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
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
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
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:931a11845ed5070cb0168a7fd3a00d4644d2209377bcc56f24f9303e666d8bbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:7e5a1765845a818e657063bc693b2890b02f7860c7355f18618ecc568d6632a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:7e5a1765845a818e657063bc693b2890b02f7860c7355f18618ecc568d6632a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
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
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:931a11845ed5070cb0168a7fd3a00d4644d2209377bcc56f24f9303e666d8bbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b6a923aee5d78b9b8b5e4eeb09452b3edaf3642ae35a59455facff45f793f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343c71f3573323a4b242c46ec6c2695a48253d2b780228dfe808b67f7abe1aa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:f502e92ba8123dd48ead979d04dfc1fb4663dfad53872af83e60f0c4603fe401 in /nats-server 
# Thu, 07 Dec 2023 01:39:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:39:57 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:39:57 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:39:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ef3ea53a5227485a41dbaf974522b336c40cb9486b14d5dd8152c92e47cf81e`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 5.1 MB (5058584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74d8ac82df699df7ec97d365121249620dec9f35a7dc9f0f19e0147e4db105`  
		Last Modified: Thu, 07 Dec 2023 01:40:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:2b40aace744d62020f81af24776d9ea3dd7b2db51349c5406ad523e1b9652377
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:0a7b1f4d4d84dcdc6cc26f0f7b36bbad44f1d76f893f5099388b3e7dbf79c04d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063795480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c0fd2ef82c44707660bb251a3bafe1a35f1b97545d74473ede708e72ce0db3`
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
# Thu, 07 Dec 2023 01:15:40 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.7/nats-server-v2.10.7-windows-amd64.zip
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_SHASUM=92c4883cdf608c1e096feabcc9a0f46935ba34fce72210520ba2e66207968630
# Thu, 07 Dec 2023 01:16:51 GMT
RUN Set-PSDebug -Trace 2
# Thu, 07 Dec 2023 01:18:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 07 Dec 2023 01:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:18:49 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:18:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:18:51 GMT
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
	-	`sha256:3c1b29fa38804640fd014da40f6bb75e1de186bb66e503d6dc478ac64d39d6a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae886b25b11d9b870221360719245f3035fab76cf0faaa9f35b83c5a988c076`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4f14d97a99af78f3a54e018e6e5b82fb0f3b679f827268ce64af2bccc10a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7562be7e5170234e29efc9b395bab01b599634555475888b80d9fe17eb7b8ce5`  
		Last Modified: Thu, 07 Dec 2023 01:20:02 GMT  
		Size: 456.2 KB (456182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c819e27d814e20a85d82d3ffdaa135668d42fe458c0c92bf7bbb1996f9e0f7f`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 5.9 MB (5894412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0c017084ce6a109713ed27b606a834949b8cba3a8ce1dee07f9b6040efdcc4`  
		Last Modified: Thu, 07 Dec 2023 01:20:00 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ff897097cbb7915114d4ef345cbc328556d21d0fbbe23fefd0a35c6be46c4d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70c738db124696f5d5cfa249a781c74abbac5f2b3e007322c51e816fd21a87c`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe385c6d134add097dfcf0b0ed86918e1e63a23233004c6db0f5da4656de18d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:2b40aace744d62020f81af24776d9ea3dd7b2db51349c5406ad523e1b9652377
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:0a7b1f4d4d84dcdc6cc26f0f7b36bbad44f1d76f893f5099388b3e7dbf79c04d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2063795480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c0fd2ef82c44707660bb251a3bafe1a35f1b97545d74473ede708e72ce0db3`
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
# Thu, 07 Dec 2023 01:15:40 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.7/nats-server-v2.10.7-windows-amd64.zip
# Thu, 07 Dec 2023 01:15:41 GMT
ENV NATS_SERVER_SHASUM=92c4883cdf608c1e096feabcc9a0f46935ba34fce72210520ba2e66207968630
# Thu, 07 Dec 2023 01:16:51 GMT
RUN Set-PSDebug -Trace 2
# Thu, 07 Dec 2023 01:18:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 07 Dec 2023 01:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:18:49 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:18:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:18:51 GMT
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
	-	`sha256:3c1b29fa38804640fd014da40f6bb75e1de186bb66e503d6dc478ac64d39d6a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae886b25b11d9b870221360719245f3035fab76cf0faaa9f35b83c5a988c076`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4f14d97a99af78f3a54e018e6e5b82fb0f3b679f827268ce64af2bccc10a9`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7562be7e5170234e29efc9b395bab01b599634555475888b80d9fe17eb7b8ce5`  
		Last Modified: Thu, 07 Dec 2023 01:20:02 GMT  
		Size: 456.2 KB (456182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c819e27d814e20a85d82d3ffdaa135668d42fe458c0c92bf7bbb1996f9e0f7f`  
		Last Modified: Thu, 07 Dec 2023 01:20:01 GMT  
		Size: 5.9 MB (5894412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0c017084ce6a109713ed27b606a834949b8cba3a8ce1dee07f9b6040efdcc4`  
		Last Modified: Thu, 07 Dec 2023 01:20:00 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ff897097cbb7915114d4ef345cbc328556d21d0fbbe23fefd0a35c6be46c4d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70c738db124696f5d5cfa249a781c74abbac5f2b3e007322c51e816fd21a87c`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe385c6d134add097dfcf0b0ed86918e1e63a23233004c6db0f5da4656de18d`  
		Last Modified: Thu, 07 Dec 2023 01:19:59 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
