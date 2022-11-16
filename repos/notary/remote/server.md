## `notary:server`

```console
$ docker pull notary@sha256:426066af779782c9d4139558ac2c46129627a6af05c08aa373bb8dacafdc26a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server` - linux; amd64

```console
$ docker pull notary@sha256:f325cf40c50cad78a0fa29c4b2e2adfbeed0f763c2593c613771e67b702936a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7952154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11391e480d8657a3757d25840d853d88b860f3354daf7067f4757e44169cdbf1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 06:38:02 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 06:38:02 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 06:38:02 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 06:38:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 06:38:02 GMT
WORKDIR /notary/server
# Wed, 16 Nov 2022 21:31:54 GMT
COPY /notary-server ./ # buildkit
# Wed, 16 Nov 2022 21:31:54 GMT
RUN ./notary-server --version # buildkit
# Wed, 16 Nov 2022 21:31:54 GMT
COPY ./server-config.json . # buildkit
# Wed, 16 Nov 2022 21:31:54 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 16 Nov 2022 21:31:54 GMT
USER notary
# Wed, 16 Nov 2022 21:31:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Nov 2022 21:31:54 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab556644ad7457163fa974396862be0db6a3e9b2a288041b04e6009ae65f4ed`  
		Last Modified: Sat, 12 Nov 2022 06:38:20 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed42602a65127618c555766dddb85795b2a28b21875015cc78f009e503b964d`  
		Last Modified: Sat, 12 Nov 2022 06:38:18 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f203748d2265829ea20f5086242998544e1dee5ba69e81e3fcae343022832`  
		Last Modified: Wed, 16 Nov 2022 21:32:14 GMT  
		Size: 5.1 MB (5143656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85af102e4358babe07884c886ba9d6374e3ed2fac11bb96056ad526b52ce161`  
		Last Modified: Wed, 16 Nov 2022 21:32:13 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52419ad609ab0abad265bfbc64ca2c4d1d885529c3a4435339804aaa31c87b03`  
		Last Modified: Wed, 16 Nov 2022 21:32:13 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbbd95d882a2b54ee5abbe4dca7816fbe20f55ae342d0c99416b1ff2604e972`  
		Last Modified: Wed, 16 Nov 2022 21:32:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:adb342817bd59647215f1c76dbcc374ed38312fb617336a4df8489c6d4280ed7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7505612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9572a430f711f301acad1e66215624009bcbeb685957f2628ba7cabdbd8e6b88`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:53:33 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:53:33 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 04:53:33 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 04:53:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 04:53:33 GMT
WORKDIR /notary/server
# Wed, 16 Nov 2022 20:32:08 GMT
COPY /notary-server ./ # buildkit
# Wed, 16 Nov 2022 20:32:09 GMT
RUN ./notary-server --version # buildkit
# Wed, 16 Nov 2022 20:32:09 GMT
COPY ./server-config.json . # buildkit
# Wed, 16 Nov 2022 20:32:09 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 16 Nov 2022 20:32:09 GMT
USER notary
# Wed, 16 Nov 2022 20:32:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Nov 2022 20:32:09 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f84bc6be5fe2d32e4441665bf4590588a5e805f0f4dc59ca7f20062278a1a`  
		Last Modified: Sat, 12 Nov 2022 04:54:08 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33090c22b1906904caf40830c2082f01799849efbaa3e099979f076f82c8b3a1`  
		Last Modified: Sat, 12 Nov 2022 04:54:05 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defdc1b690f33d4d1e8c51255c017f013012613de6dfc1d0d1cc54c380a5d637`  
		Last Modified: Wed, 16 Nov 2022 20:32:48 GMT  
		Size: 4.9 MB (4888305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae819094715d1226901c8c62e16f592b1693d5d3b504bc82f413fcf7836fb782`  
		Last Modified: Wed, 16 Nov 2022 20:32:47 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9077aa6940ac10e715894e5bf97df159727a844eac8cf07fcbfd1a3cd6f532b3`  
		Last Modified: Wed, 16 Nov 2022 20:32:47 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07cb2e2ddf815cb914da3f7e9f27c0cd294f39dcc1f123007d06bc0b75ee5d0`  
		Last Modified: Wed, 16 Nov 2022 20:32:48 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:000524f15adf640235589fd539b16dbf23011194d054c4d7598689c616404342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7441477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bcc67d244172ffd0bf8b4f65431979ab1b9a33892a8b5b312415a26e5591843`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:36:49 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 04:36:49 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 04:36:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 04:36:49 GMT
WORKDIR /notary/server
# Wed, 16 Nov 2022 20:25:13 GMT
COPY /notary-server ./ # buildkit
# Wed, 16 Nov 2022 20:25:14 GMT
RUN ./notary-server --version # buildkit
# Wed, 16 Nov 2022 20:25:14 GMT
COPY ./server-config.json . # buildkit
# Wed, 16 Nov 2022 20:25:14 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 16 Nov 2022 20:25:14 GMT
USER notary
# Wed, 16 Nov 2022 20:25:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Nov 2022 20:25:14 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d302558fe89c8fe780469f0b8d23bc5062a020060a765fb3f2fbf0d7504a640`  
		Last Modified: Sat, 12 Nov 2022 04:37:07 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e2765c49d0f6fd3ccbc844595f80ded29859b5546f880e4c2a30817ec85cf3`  
		Last Modified: Sat, 12 Nov 2022 04:37:05 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abaaf5aa4251b3c135c762a84119833b1f453dfe0e944810c16460467344109`  
		Last Modified: Wed, 16 Nov 2022 20:25:31 GMT  
		Size: 4.7 MB (4731488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ea8eea6c2fb2d2c4daf657247791ddba76fa6a3d9da7c1b30dd6c7a9eb0e76`  
		Last Modified: Wed, 16 Nov 2022 20:25:30 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07b8f0e1f0c23c4b7318cff3d3e31557a072cf03cad029420927cb0fc2a46c4`  
		Last Modified: Wed, 16 Nov 2022 20:25:30 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094fdc3a29fd50e74af3baf39631e83ec609e6269dafc83359d9856643b38460`  
		Last Modified: Wed, 16 Nov 2022 20:25:30 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; 386

```console
$ docker pull notary@sha256:0051a396f9f855c79af832411477a4c7d2378269fc49944bff0715d4fd0eccba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7754948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:230c21477b98b5a11af0491ebeeb38d1b540df1682e89ee33b1fa8d429f64a0a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:57:54 GMT
RUN adduser -D -H -g "" notary
# Sat, 12 Nov 2022 04:57:55 GMT
EXPOSE 4443
# Sat, 12 Nov 2022 04:57:56 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 04:57:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 04:57:58 GMT
WORKDIR /notary/server
# Wed, 16 Nov 2022 20:11:14 GMT
COPY file:a4c6c805f5f0a0a5415c68f8471cb31bca1747a0f8e35cf5005cea98e0fba5b5 in ./ 
# Wed, 16 Nov 2022 20:11:14 GMT
RUN ./notary-server --version
# Wed, 16 Nov 2022 20:11:16 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Wed, 16 Nov 2022 20:11:17 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Wed, 16 Nov 2022 20:11:17 GMT
USER notary
# Wed, 16 Nov 2022 20:11:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Nov 2022 20:11:19 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e2a37344f15c9c47f28fb76d0bbfae6f9adb65b4d686216a9a5881505ed0ec`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9866a73f72dbc8d55f6da18666277753336525decc6cf3f5862f64f9aede0bb4`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babe522935d5c7619a31b2dbe314aa999f9638f58cfd681d4ead6cf30174456e`  
		Last Modified: Wed, 16 Nov 2022 20:11:48 GMT  
		Size: 4.9 MB (4944492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cba96d642e8b023076db8e169e56c622fd46d71523562be43e6488fde467c1f`  
		Last Modified: Wed, 16 Nov 2022 20:11:47 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2526f0d6947677f3d4316cad2f10abb51443194ed1ba4f3d3b757a812041fd13`  
		Last Modified: Wed, 16 Nov 2022 20:11:47 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:a3978dfff04ce1c14c9a6490df71b510ca903420f6f4b47282b0ca8461d410ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7437011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a8591aa44b08a6bd89f8804d32696541f8124083ef21e59e60a786ffc29147e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:12:27 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 07:12:27 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 07:12:27 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 07:12:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 07:12:27 GMT
WORKDIR /notary/server
# Wed, 16 Nov 2022 21:41:53 GMT
COPY /notary-server ./ # buildkit
# Wed, 16 Nov 2022 21:41:53 GMT
RUN ./notary-server --version # buildkit
# Wed, 16 Nov 2022 21:41:53 GMT
COPY ./server-config.json . # buildkit
# Wed, 16 Nov 2022 21:41:54 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 16 Nov 2022 21:41:54 GMT
USER notary
# Wed, 16 Nov 2022 21:41:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Nov 2022 21:41:54 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15023fe5082ace3d77a3ca4c98a9b31b5bef60a4835bddce618606ee9f17cf6`  
		Last Modified: Sat, 12 Nov 2022 07:13:02 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f15b402da893576104d72bedce0b38fd79217c0335b5c4ce1a6076cebbb1b8a`  
		Last Modified: Sat, 12 Nov 2022 07:12:59 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f138d0c353b049908f7b8d0cb32143e6c3e01fa17402e04b14ee1d73deefd96`  
		Last Modified: Wed, 16 Nov 2022 21:42:28 GMT  
		Size: 4.6 MB (4633226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161902d761c2a3c7a33b660dc171044013ec7e12d8d4b2ba0b6aa510db11f1ec`  
		Last Modified: Wed, 16 Nov 2022 21:42:27 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34e0311411137dbb59885962090043674b00dd997b180e45ccad85899a1299b`  
		Last Modified: Wed, 16 Nov 2022 21:42:27 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c4428ac21524a938872244c26fbef204d2296ed8fa0ae5fa32c855ba035a82`  
		Last Modified: Wed, 16 Nov 2022 21:42:27 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:249cb78d568f6a0c16961a2afe45a27a1ea1a07c5f5d134ad8af37a374e9bd17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7562094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c091a7a5dea5fcbec5c1baacee56e62cde977d9d88fa6a50cbde82b480f7e50`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:29:11 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 05:29:11 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 05:29:11 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 05:29:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 05:29:11 GMT
WORKDIR /notary/server
# Wed, 16 Nov 2022 20:22:45 GMT
COPY /notary-server ./ # buildkit
# Wed, 16 Nov 2022 20:22:45 GMT
RUN ./notary-server --version # buildkit
# Wed, 16 Nov 2022 20:22:45 GMT
COPY ./server-config.json . # buildkit
# Wed, 16 Nov 2022 20:22:45 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 16 Nov 2022 20:22:45 GMT
USER notary
# Wed, 16 Nov 2022 20:22:45 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Nov 2022 20:22:45 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4ef31691b8350e3f169efda08440ffc8f858999b921631575acdfd35d88225`  
		Last Modified: Sat, 12 Nov 2022 05:29:49 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba78ca725314efb5b67eb6424fd58fc99193e2ba05a043a971a5d7bb549454fa`  
		Last Modified: Sat, 12 Nov 2022 05:29:47 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3297d31e4fbc1dec5321b3782b07b7900cfecdf676886b41643f87b02bb9092`  
		Last Modified: Wed, 16 Nov 2022 20:23:17 GMT  
		Size: 5.0 MB (4968735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac79ce692df4b6a1b986f76d2309fda24b1f22febc4e478553e25f44356aabe`  
		Last Modified: Wed, 16 Nov 2022 20:23:16 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b875bd30b1928449edbe8a3ecfcc9cec33b62d7a43d197f52f6d2d7051b9613e`  
		Last Modified: Wed, 16 Nov 2022 20:23:16 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58765e48a937fac80cbdb3ca54c7144e24844e0ae2754c2b3cb3ca5a3292061a`  
		Last Modified: Wed, 16 Nov 2022 20:23:16 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
