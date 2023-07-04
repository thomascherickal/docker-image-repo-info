## `debian:experimental`

```console
$ docker pull debian@sha256:acb853fe3bab46bdef81f5eaa02b94d193c631e49ac9a12573362918380cdf9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:542c7506fae412a82407cfe7ca48880d866b844827a98c763fa0823d68fc05fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49552187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1dcc4959ad085eed9a306cf1320fe542290293144169ea7e495813bd2c4be5d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:24:13 GMT
ADD file:1b41b99fed8ff2eeb6430593fe15af3ee98c3cc381c92244a8a08d1287b1066b in / 
# Mon, 12 Jun 2023 23:24:13 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:24:28 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4383743d159a89fbf27437c90c820edaec7efa5c350cf220957b8bf9853dace9`  
		Last Modified: Mon, 12 Jun 2023 23:30:37 GMT  
		Size: 49.6 MB (49551969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4822191ae077c9e650f0c69c009f37b1ef730439ea6adad945ccfcc42b36a797`  
		Last Modified: Mon, 12 Jun 2023 23:30:58 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:8c0a40eb00289d699534f5b060d1c9e9bb61b508c6d5fc662606ba1f250b07c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47322694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883bff7d7307e93e117c0640650f6717d50ba33c539fecd83d3e1638c5d7f5a1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:50:15 GMT
ADD file:0d73a7183a38c56858e61e53f0c64ae6eaf9d58311df1be7af3b37f1e1769dd2 in / 
# Tue, 04 Jul 2023 00:50:16 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:50:26 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:eb46e2b513bf023b4297bc46404f96d3a604f8f913dffe3d1f9e5c5c530e9caf`  
		Last Modified: Tue, 04 Jul 2023 00:55:44 GMT  
		Size: 47.3 MB (47322476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b079d533182e62457871a1cdecd8b7307dda1c497fda642b534f1738b904b1aa`  
		Last Modified: Tue, 04 Jul 2023 00:56:07 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:8e140ce88bd505eebe36c6aebac98f5303b50a067126409f0fc4831ad06b5bc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45124201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e332aa22a3f6fe878a99005e2a42ca5ff1c89e17e08b81d9010ed364042cab74`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:01:20 GMT
ADD file:a7c3220804fb0e3fd658c0492b5338ba9fc6c132f28282486bbae9622138fd0e in / 
# Tue, 04 Jul 2023 01:01:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:01:31 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0807315011437359206e59c75af82e26e89ba45ae9281fa33df5e8dda8de17a2`  
		Last Modified: Tue, 04 Jul 2023 01:07:56 GMT  
		Size: 45.1 MB (45123977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c69a5003d0ef8f39c11e33430cc1570553f8fa01a641e6fb1694acb22e771`  
		Last Modified: Tue, 04 Jul 2023 01:08:17 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:85b513c6a706209d51c0de052a2c1f50fc896065c350f6b477c2f40909ca1ced
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49592319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfbd256d97fcf96e7a894f00c19e65affa300affbd3243e7985e96581bd22fb3`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:42:53 GMT
ADD file:0aac014f1e1bde85101016ecc21c6ce394e7952ee93b2d890561254d2d94d498 in / 
# Mon, 12 Jun 2023 23:42:54 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:43:05 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:11c5785280392c7af20e50b01a59b28f54f8bc1bd64dd9f1d03e55b37d6a2127`  
		Last Modified: Mon, 12 Jun 2023 23:48:28 GMT  
		Size: 49.6 MB (49592100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fb264c6f7ad2d75149a3427fa00db70f8fac6625743988e34fcd81f4dc3ec6`  
		Last Modified: Mon, 12 Jun 2023 23:48:48 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:f109ab1319ba9f1ce7e0941afc1b29fc091f91672ef5687b2c9c9d3a570ead8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50562930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0b58f40534abf2f4843c25bd411bb978b9e615bb6a95fc7cd7eb4b5a24f5ed`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:44:39 GMT
ADD file:e8571637c4281674e6afc663a8ea3f1b772973b3446c84754360925882b61b73 in / 
# Mon, 12 Jun 2023 23:44:40 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:45:01 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9694989688ceda75b79a06cc1c8b58846dbcbbb8de07c1813eba0848993d77cc`  
		Last Modified: Mon, 12 Jun 2023 23:51:50 GMT  
		Size: 50.6 MB (50562712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ddf6c9cce72277a49750f39b0e153859e3622c97fed812d0d830813ed9c94c`  
		Last Modified: Mon, 12 Jun 2023 23:52:13 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:ca090bdb7aa13f1806e6c6e3f306f45692ec55e03c9cd2387596f3143bf2c5f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49561515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:498f3ef3deaf06343059b24f9759c9239b0f30bb4c48b034bde3f4c2d1c08e58`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:19:15 GMT
ADD file:29fe2010c70b61fc3710bf2ff523db4da234cfb8f6f1ce41462c20ee633d4f38 in / 
# Tue, 13 Jun 2023 00:19:20 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:20:14 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8e4aec601636f48d5335bebb0d32ab0024a74fc7e9c66eeb1815fe381cb62bba`  
		Last Modified: Tue, 13 Jun 2023 00:30:48 GMT  
		Size: 49.6 MB (49561295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23796659896c9ecbbba4f1cb3718396a0633440ddc8560d928365e06b434a9a9`  
		Last Modified: Tue, 13 Jun 2023 00:31:27 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:9c8a77bd6580e08a8275e380c06cef809d56571e9444f39ea1adfc970b3e2bc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53558728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d72655bf006ab0f44a31a1e4f9c3cab6b1c350fec139cdd0027be3da6c0e7cb`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:22:17 GMT
ADD file:e156fc6652b06579a450e9b39d936d4ac451cf8c59eb24eedde04768b96f999e in / 
# Mon, 12 Jun 2023 23:22:19 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:22:41 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:feca272a05571ffbf463bdd359810009ffab2d778ca679b5442365cc60ee23c5`  
		Last Modified: Mon, 12 Jun 2023 23:29:12 GMT  
		Size: 53.6 MB (53558509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd200ed56bc8305093c6e3e9d292008a5057c3485c3750d8708d99712c534106`  
		Last Modified: Mon, 12 Jun 2023 23:29:40 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:fd8164a7bd9565294d8f433d478adcc1f7371e0ad3431c78beb30d80bbaf2aae
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45695712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3db54503fa0f89e6f3eee133d4dec5dc6027fdaf9f340fdb7affc4e93354b751`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:10:32 GMT
ADD file:bacf5c7bb4f9db293679962e5936b1037a72a2e667da59236cda267c866ad8e2 in / 
# Tue, 04 Jul 2023 01:10:34 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:11:21 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:892c64510625aa4b95222221c8d62ebbab44da937d39c14956f6e6697a5c4c80`  
		Last Modified: Tue, 04 Jul 2023 01:13:59 GMT  
		Size: 45.7 MB (45695485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58595682130886a8914b61a3a37dc1da553893a9cf3815062133cff2dfff8ee6`  
		Last Modified: Tue, 04 Jul 2023 01:14:45 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:c041a2267754cf89d0d808905f579ade6632e2d78454ac4e88f6f114e6ebcba2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47920814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d8049a13735f22e4137804fd1e7e5362e511a575670fd420b9ec5be834183e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:32:56 GMT
ADD file:c70c29e6cad97a539b70a653712f53cf941eea890fac34915cecddaf2408d469 in / 
# Tue, 13 Jun 2023 04:32:59 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:33:16 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e8889c007cdf39d47aac32355ac4e468a69920720510572fb59d81f6751a5846`  
		Last Modified: Tue, 13 Jun 2023 04:36:55 GMT  
		Size: 47.9 MB (47920596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0088f95a72cb2a6eac9c0dc0ab7f10f17ebac1f0c2589e503a276d5f16b663`  
		Last Modified: Tue, 13 Jun 2023 04:37:08 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
