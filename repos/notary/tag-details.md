<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.7.0`](#notaryserver-070)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.7.0`](#notarysigner-070)

## `notary:server`

```console
$ docker pull notary@sha256:56eed64d1fb8fbbaf79a4214fa0a5dde2cbf7959038e8f6a72bc0b5dc893634f
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
$ docker pull notary@sha256:d809cfdca8cd29d066fc221c2bfd82a0b2f38dfeae98ba131b4810531336314e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7952148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2976a4d707c376afac8a3692be198e81d833696f8c6a740c38c07958e00ac4b6`
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
# Wed, 07 Dec 2022 00:19:37 GMT
COPY /notary-server ./ # buildkit
# Wed, 07 Dec 2022 00:19:37 GMT
RUN ./notary-server --version # buildkit
# Wed, 07 Dec 2022 00:19:37 GMT
COPY ./server-config.json . # buildkit
# Wed, 07 Dec 2022 00:19:37 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 07 Dec 2022 00:19:37 GMT
USER notary
# Wed, 07 Dec 2022 00:19:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 07 Dec 2022 00:19:37 GMT
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
	-	`sha256:141f5624e22b20daf46f6758dd8007efb347be8cf624c1c746d09bf6ce7fa5e9`  
		Last Modified: Wed, 07 Dec 2022 00:19:55 GMT  
		Size: 5.1 MB (5143646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867de90abd571ebfaaf24ac0b459bd674b5e11d1ccdb69b2e2a03374aead60e0`  
		Last Modified: Wed, 07 Dec 2022 00:19:54 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bbb169f9532dc9c027bca4ff9c263c9df5e586b6bd9c2caa63c0577e70ea60`  
		Last Modified: Wed, 07 Dec 2022 00:19:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93950912b0bf63b250aaba4d037ffa20f0b777950f68aee515d9a4d8c62e77aa`  
		Last Modified: Wed, 07 Dec 2022 00:19:54 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:3146b5c8da4d09711ddd0816964521e23a6676f501e88ec1a7e5280e6fb6c3da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7506156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b595c4018f5c0f9f198478455f457bd2a87f12123d337367494e497b3537f8c`
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
# Tue, 06 Dec 2022 21:18:58 GMT
COPY /notary-server ./ # buildkit
# Tue, 06 Dec 2022 21:18:58 GMT
RUN ./notary-server --version # buildkit
# Tue, 06 Dec 2022 21:18:58 GMT
COPY ./server-config.json . # buildkit
# Tue, 06 Dec 2022 21:18:58 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:18:58 GMT
USER notary
# Tue, 06 Dec 2022 21:18:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:18:58 GMT
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
	-	`sha256:7f373478af2347219011c0a63ee63a10f99b52f8d1e4b83f02dca2691cf95bff`  
		Last Modified: Tue, 06 Dec 2022 21:19:35 GMT  
		Size: 4.9 MB (4888849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02428edbdcee48cb0bf71f76e386c61819ae4fce65ca829e50a0fd3ba61682bc`  
		Last Modified: Tue, 06 Dec 2022 21:19:34 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66362a79c0f28dce86af1f18d61313a41c72531aaa3359870d69a996b41ffae6`  
		Last Modified: Tue, 06 Dec 2022 21:19:34 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733fa05cbe8c1083a808d762f996214acab0377cddcebf49cb605830c2eace6b`  
		Last Modified: Tue, 06 Dec 2022 21:19:34 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:f05e8c5a28e1eaa92e1d08575df17069b1c8b40cba4fc9af94fccff61227204d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7441002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb806eabc1b3de405d164516cd49f831dec3216418e00241aea46ad4f6c26579`
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
# Tue, 06 Dec 2022 21:06:36 GMT
COPY /notary-server ./ # buildkit
# Tue, 06 Dec 2022 21:06:36 GMT
RUN ./notary-server --version # buildkit
# Tue, 06 Dec 2022 21:06:36 GMT
COPY ./server-config.json . # buildkit
# Tue, 06 Dec 2022 21:06:36 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:06:36 GMT
USER notary
# Tue, 06 Dec 2022 21:06:36 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:06:36 GMT
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
	-	`sha256:d8322efb1986526da186f315eb1c9217b454f528b438fb0ccbb9b2e26a6dd779`  
		Last Modified: Tue, 06 Dec 2022 21:06:55 GMT  
		Size: 4.7 MB (4731016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e469014c48d96eadbf5458c8c85dbfd82081dc8e52d889c151052649d3173076`  
		Last Modified: Tue, 06 Dec 2022 21:06:54 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927dd11231f23e8ed46141d2ddc4ce7ae5a6b71e05e2423d45012ddd0181437f`  
		Last Modified: Tue, 06 Dec 2022 21:06:54 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19af448572ae46b5e1af524723da74a570d244844541d80b166f543cfffe62`  
		Last Modified: Tue, 06 Dec 2022 21:06:54 GMT  
		Size: 382.0 B  
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
$ docker pull notary@sha256:403073aa80474f7d953a3148793eb27a7515dd57f6ffcbfdaf3bc7849edd290f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7437664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b38fc29374e009b8657529edd601356084ef98c21c2244987d0aac8dbcafc840`
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
# Tue, 06 Dec 2022 22:39:14 GMT
COPY /notary-server ./ # buildkit
# Tue, 06 Dec 2022 22:39:15 GMT
RUN ./notary-server --version # buildkit
# Tue, 06 Dec 2022 22:39:15 GMT
COPY ./server-config.json . # buildkit
# Tue, 06 Dec 2022 22:39:15 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 22:39:15 GMT
USER notary
# Tue, 06 Dec 2022 22:39:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 22:39:15 GMT
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
	-	`sha256:148138d700117e87a9bfd7e0ba761909205fe8de3a87e8095fbb97c77d047087`  
		Last Modified: Tue, 06 Dec 2022 22:39:48 GMT  
		Size: 4.6 MB (4633879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36784d9bee68980e3ae9480379ca663e5034db4973e55ee70b075fce0376548`  
		Last Modified: Tue, 06 Dec 2022 22:39:47 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b4d050257238bd859c8c5cea67fef3bea40f6974c3c0a58c875ed4762c45e4`  
		Last Modified: Tue, 06 Dec 2022 22:39:47 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d01c19f532bf882cd8c70fac3792308b77d0822e66e05845d3595e029d5aedd`  
		Last Modified: Tue, 06 Dec 2022 22:39:47 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:5ad68984308f4e58bae487ca7952af8a853e785260f504ac14cbecc2b6dfe3ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7563431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64e85201719660e9f6380da1b1fb6e5f962e93d1f922edf5140ff5f5e2796335`
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
# Tue, 06 Dec 2022 21:11:42 GMT
COPY /notary-server ./ # buildkit
# Tue, 06 Dec 2022 21:11:43 GMT
RUN ./notary-server --version # buildkit
# Tue, 06 Dec 2022 21:11:43 GMT
COPY ./server-config.json . # buildkit
# Tue, 06 Dec 2022 21:11:43 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:11:43 GMT
USER notary
# Tue, 06 Dec 2022 21:11:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:11:43 GMT
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
	-	`sha256:2551ed8601cbe43a55def52b8e69eda72eac7f885e2c7887f7c2fe356c3ed40c`  
		Last Modified: Tue, 06 Dec 2022 21:12:14 GMT  
		Size: 5.0 MB (4970070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a6d35a1a6dfca332775b11c7e795872b345e57ef74e2d993f7e265a6e5fa53`  
		Last Modified: Tue, 06 Dec 2022 21:12:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fb22baeef1a59d2f6f94f7ebf2c67b74cf62e078c7453b3133693d5c480a5b`  
		Last Modified: Tue, 06 Dec 2022 21:12:13 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604b38c3dfdfe07a93622e1f8c465cfd58a0bb2284df0fd332a3ddeffe44fa76`  
		Last Modified: Tue, 06 Dec 2022 21:12:13 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:56eed64d1fb8fbbaf79a4214fa0a5dde2cbf7959038e8f6a72bc0b5dc893634f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server-0.7.0` - linux; amd64

```console
$ docker pull notary@sha256:d809cfdca8cd29d066fc221c2bfd82a0b2f38dfeae98ba131b4810531336314e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7952148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2976a4d707c376afac8a3692be198e81d833696f8c6a740c38c07958e00ac4b6`
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
# Wed, 07 Dec 2022 00:19:37 GMT
COPY /notary-server ./ # buildkit
# Wed, 07 Dec 2022 00:19:37 GMT
RUN ./notary-server --version # buildkit
# Wed, 07 Dec 2022 00:19:37 GMT
COPY ./server-config.json . # buildkit
# Wed, 07 Dec 2022 00:19:37 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 07 Dec 2022 00:19:37 GMT
USER notary
# Wed, 07 Dec 2022 00:19:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 07 Dec 2022 00:19:37 GMT
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
	-	`sha256:141f5624e22b20daf46f6758dd8007efb347be8cf624c1c746d09bf6ce7fa5e9`  
		Last Modified: Wed, 07 Dec 2022 00:19:55 GMT  
		Size: 5.1 MB (5143646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867de90abd571ebfaaf24ac0b459bd674b5e11d1ccdb69b2e2a03374aead60e0`  
		Last Modified: Wed, 07 Dec 2022 00:19:54 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bbb169f9532dc9c027bca4ff9c263c9df5e586b6bd9c2caa63c0577e70ea60`  
		Last Modified: Wed, 07 Dec 2022 00:19:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93950912b0bf63b250aaba4d037ffa20f0b777950f68aee515d9a4d8c62e77aa`  
		Last Modified: Wed, 07 Dec 2022 00:19:54 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:3146b5c8da4d09711ddd0816964521e23a6676f501e88ec1a7e5280e6fb6c3da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7506156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b595c4018f5c0f9f198478455f457bd2a87f12123d337367494e497b3537f8c`
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
# Tue, 06 Dec 2022 21:18:58 GMT
COPY /notary-server ./ # buildkit
# Tue, 06 Dec 2022 21:18:58 GMT
RUN ./notary-server --version # buildkit
# Tue, 06 Dec 2022 21:18:58 GMT
COPY ./server-config.json . # buildkit
# Tue, 06 Dec 2022 21:18:58 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:18:58 GMT
USER notary
# Tue, 06 Dec 2022 21:18:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:18:58 GMT
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
	-	`sha256:7f373478af2347219011c0a63ee63a10f99b52f8d1e4b83f02dca2691cf95bff`  
		Last Modified: Tue, 06 Dec 2022 21:19:35 GMT  
		Size: 4.9 MB (4888849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02428edbdcee48cb0bf71f76e386c61819ae4fce65ca829e50a0fd3ba61682bc`  
		Last Modified: Tue, 06 Dec 2022 21:19:34 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66362a79c0f28dce86af1f18d61313a41c72531aaa3359870d69a996b41ffae6`  
		Last Modified: Tue, 06 Dec 2022 21:19:34 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733fa05cbe8c1083a808d762f996214acab0377cddcebf49cb605830c2eace6b`  
		Last Modified: Tue, 06 Dec 2022 21:19:34 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:f05e8c5a28e1eaa92e1d08575df17069b1c8b40cba4fc9af94fccff61227204d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7441002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb806eabc1b3de405d164516cd49f831dec3216418e00241aea46ad4f6c26579`
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
# Tue, 06 Dec 2022 21:06:36 GMT
COPY /notary-server ./ # buildkit
# Tue, 06 Dec 2022 21:06:36 GMT
RUN ./notary-server --version # buildkit
# Tue, 06 Dec 2022 21:06:36 GMT
COPY ./server-config.json . # buildkit
# Tue, 06 Dec 2022 21:06:36 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:06:36 GMT
USER notary
# Tue, 06 Dec 2022 21:06:36 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:06:36 GMT
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
	-	`sha256:d8322efb1986526da186f315eb1c9217b454f528b438fb0ccbb9b2e26a6dd779`  
		Last Modified: Tue, 06 Dec 2022 21:06:55 GMT  
		Size: 4.7 MB (4731016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e469014c48d96eadbf5458c8c85dbfd82081dc8e52d889c151052649d3173076`  
		Last Modified: Tue, 06 Dec 2022 21:06:54 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927dd11231f23e8ed46141d2ddc4ce7ae5a6b71e05e2423d45012ddd0181437f`  
		Last Modified: Tue, 06 Dec 2022 21:06:54 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19af448572ae46b5e1af524723da74a570d244844541d80b166f543cfffe62`  
		Last Modified: Tue, 06 Dec 2022 21:06:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; 386

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

### `notary:server-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:403073aa80474f7d953a3148793eb27a7515dd57f6ffcbfdaf3bc7849edd290f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7437664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b38fc29374e009b8657529edd601356084ef98c21c2244987d0aac8dbcafc840`
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
# Tue, 06 Dec 2022 22:39:14 GMT
COPY /notary-server ./ # buildkit
# Tue, 06 Dec 2022 22:39:15 GMT
RUN ./notary-server --version # buildkit
# Tue, 06 Dec 2022 22:39:15 GMT
COPY ./server-config.json . # buildkit
# Tue, 06 Dec 2022 22:39:15 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 22:39:15 GMT
USER notary
# Tue, 06 Dec 2022 22:39:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 22:39:15 GMT
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
	-	`sha256:148138d700117e87a9bfd7e0ba761909205fe8de3a87e8095fbb97c77d047087`  
		Last Modified: Tue, 06 Dec 2022 22:39:48 GMT  
		Size: 4.6 MB (4633879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36784d9bee68980e3ae9480379ca663e5034db4973e55ee70b075fce0376548`  
		Last Modified: Tue, 06 Dec 2022 22:39:47 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b4d050257238bd859c8c5cea67fef3bea40f6974c3c0a58c875ed4762c45e4`  
		Last Modified: Tue, 06 Dec 2022 22:39:47 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d01c19f532bf882cd8c70fac3792308b77d0822e66e05845d3595e029d5aedd`  
		Last Modified: Tue, 06 Dec 2022 22:39:47 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:5ad68984308f4e58bae487ca7952af8a853e785260f504ac14cbecc2b6dfe3ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7563431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64e85201719660e9f6380da1b1fb6e5f962e93d1f922edf5140ff5f5e2796335`
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
# Tue, 06 Dec 2022 21:11:42 GMT
COPY /notary-server ./ # buildkit
# Tue, 06 Dec 2022 21:11:43 GMT
RUN ./notary-server --version # buildkit
# Tue, 06 Dec 2022 21:11:43 GMT
COPY ./server-config.json . # buildkit
# Tue, 06 Dec 2022 21:11:43 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:11:43 GMT
USER notary
# Tue, 06 Dec 2022 21:11:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:11:43 GMT
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
	-	`sha256:2551ed8601cbe43a55def52b8e69eda72eac7f885e2c7887f7c2fe356c3ed40c`  
		Last Modified: Tue, 06 Dec 2022 21:12:14 GMT  
		Size: 5.0 MB (4970070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a6d35a1a6dfca332775b11c7e795872b345e57ef74e2d993f7e265a6e5fa53`  
		Last Modified: Tue, 06 Dec 2022 21:12:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fb22baeef1a59d2f6f94f7ebf2c67b74cf62e078c7453b3133693d5c480a5b`  
		Last Modified: Tue, 06 Dec 2022 21:12:13 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604b38c3dfdfe07a93622e1f8c465cfd58a0bb2284df0fd332a3ddeffe44fa76`  
		Last Modified: Tue, 06 Dec 2022 21:12:13 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer`

```console
$ docker pull notary@sha256:54736635ff9dcb0b71b83270e20b516afa3c8d7e932c1e1565f9049792b0e18a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer` - linux; amd64

```console
$ docker pull notary@sha256:0875013a6d3a2be8fb40d401accbd45ebbc071389ee97e1a75e068b3e1bf6872
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7565741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fde673ba5abe3aa357e4518af9cdde5b51cb4d9384bf71bdab1f7d329edaf55a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 06:38:02 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 06:38:08 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 06:38:08 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 06:38:08 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 06:38:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 06:38:08 GMT
WORKDIR /notary/signer
# Wed, 07 Dec 2022 00:19:42 GMT
COPY /notary-signer ./ # buildkit
# Wed, 07 Dec 2022 00:19:42 GMT
RUN ./notary-signer --version # buildkit
# Wed, 07 Dec 2022 00:19:42 GMT
COPY ./signer-config.json . # buildkit
# Wed, 07 Dec 2022 00:19:43 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 07 Dec 2022 00:19:43 GMT
USER notary
# Wed, 07 Dec 2022 00:19:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 07 Dec 2022 00:19:43 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:8da59cda2c120691b5be31fdc1571f10856ae5c4527c577ae2f76cd70fcd4a05`  
		Last Modified: Sat, 12 Nov 2022 06:38:29 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcfed49199016f957dddc67d897e93757dcc6a76a282a9f206a3449455e307b`  
		Last Modified: Wed, 07 Dec 2022 00:20:05 GMT  
		Size: 4.8 MB (4757304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf85ebd2351e71c23253b4d0b8761c6972e1dc5df54962090f047a8ca5e1b6d`  
		Last Modified: Wed, 07 Dec 2022 00:20:03 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eefdf52ec5e0b4f5987080be2a3bb44bd4e340fad81a1ab4376407900063f11`  
		Last Modified: Wed, 07 Dec 2022 00:20:03 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42341ba3d013ebf80c6d9dcbfe35a61125631b1d1133962eb9c18ca67e3e40b6`  
		Last Modified: Wed, 07 Dec 2022 00:20:04 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:dc674ebdc96dd1934111b4d84f9d56c55d21fc26cb078ec2f8c9a1bb836b16be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55989575380ac94315193ca596d70959ac8e2ec1c39eabaccfeb1966454be668`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:53:33 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:53:47 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 04:53:47 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 04:53:47 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:53:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:53:47 GMT
WORKDIR /notary/signer
# Tue, 06 Dec 2022 21:19:15 GMT
COPY /notary-signer ./ # buildkit
# Tue, 06 Dec 2022 21:19:15 GMT
RUN ./notary-signer --version # buildkit
# Tue, 06 Dec 2022 21:19:15 GMT
COPY ./signer-config.json . # buildkit
# Tue, 06 Dec 2022 21:19:15 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:19:15 GMT
USER notary
# Tue, 06 Dec 2022 21:19:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:19:15 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:125649f53222ca94f2e22db8ba79ba38d7d33fee96be71c6f2a0e58b1045ac49`  
		Last Modified: Sat, 12 Nov 2022 04:54:19 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47283c38f888cf865442bbf36d4aec3f09de0a9c8d2dd33dc606b2e19564c423`  
		Last Modified: Tue, 06 Dec 2022 21:19:46 GMT  
		Size: 4.5 MB (4520351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d490b0891554a66e5b88052b709c3633c6ec5df6f0ffa0794bbe31cdfee103`  
		Last Modified: Tue, 06 Dec 2022 21:19:45 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0052e17712c732b0feec88e761587d4df1400f0966d0196c6f4892dcc9c66b97`  
		Last Modified: Tue, 06 Dec 2022 21:19:46 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4036cef39afcea28c4572740467d6b3547376c97afcb9339c1a794fd69f47f3`  
		Last Modified: Tue, 06 Dec 2022 21:19:45 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:b4a6261a1055e75c9d91f6a585ab49b0825302f0659a68f7dc9158fff485a923
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7094071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c822e290dfeb3acdab813d11c76673853584b53d7a87a2f926409a07286a28f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:36:49 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:36:54 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 04:36:54 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 04:36:54 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:36:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:36:54 GMT
WORKDIR /notary/signer
# Tue, 06 Dec 2022 21:06:42 GMT
COPY /notary-signer ./ # buildkit
# Tue, 06 Dec 2022 21:06:43 GMT
RUN ./notary-signer --version # buildkit
# Tue, 06 Dec 2022 21:06:43 GMT
COPY ./signer-config.json . # buildkit
# Tue, 06 Dec 2022 21:06:43 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:06:43 GMT
USER notary
# Tue, 06 Dec 2022 21:06:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:06:43 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:92adb73f02c38f4aa06f3e987ca18858a12b469b490a35a7fb86b341f2b68fb4`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab5895b8bad28249cbb19462356cd068ed56cef4d074111981055ca4e250721`  
		Last Modified: Tue, 06 Dec 2022 21:07:07 GMT  
		Size: 4.4 MB (4384147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf66df20e765e5893cbceca4bbacc24dd5f8a6054942f5cc62bd888854e1624b`  
		Last Modified: Tue, 06 Dec 2022 21:07:06 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceef232e5818ab3f78ee04a825d2a889394315063ad4b561f19bd70522e2df6`  
		Last Modified: Tue, 06 Dec 2022 21:07:07 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9818996f8c494fa753d10c185478433296b820ffc74fe10cf37e2c45e1bb2b49`  
		Last Modified: Tue, 06 Dec 2022 21:07:07 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:79b4c323f58cb5f6ea257c2af5204098abeea66bb6d3c60b46f4693e04741701
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7381566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ddf368d5d9c9179b534f7d9a67b82e27281f60554a17dc0820eabc3abfca32c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:57:54 GMT
RUN adduser -D -H -g "" notary
# Sat, 12 Nov 2022 04:58:12 GMT
EXPOSE 4444
# Sat, 12 Nov 2022 04:58:12 GMT
EXPOSE 7899
# Sat, 12 Nov 2022 04:58:13 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:58:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:58:15 GMT
WORKDIR /notary/signer
# Wed, 16 Nov 2022 20:11:26 GMT
COPY file:044b2b6099382d2e11ff09d47c7a63f7cf3796f05317a8a2bbfed5d98c843503 in ./ 
# Wed, 16 Nov 2022 20:11:26 GMT
RUN ./notary-signer --version
# Wed, 16 Nov 2022 20:11:28 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Wed, 16 Nov 2022 20:11:29 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Wed, 16 Nov 2022 20:11:29 GMT
USER notary
# Wed, 16 Nov 2022 20:11:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Nov 2022 20:11:31 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:e26472dc994c1e659b114a40b8becb18e4595de57079b3495843fe3ee077329d`  
		Last Modified: Sat, 12 Nov 2022 04:58:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77cc9f8b030709827b83734498c26e9c13fdcad73c1751041bf38760164b7c8`  
		Last Modified: Wed, 16 Nov 2022 20:11:58 GMT  
		Size: 4.6 MB (4571177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d739be5aa3edcc7ba9f282a037921fc7c54d03aa47497444165ee21ada1487a6`  
		Last Modified: Wed, 16 Nov 2022 20:11:57 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f6cc98121c6d6e23c455cc4891ee75f1d872207a89e3ff24c67d8eedf86dac`  
		Last Modified: Wed, 16 Nov 2022 20:11:58 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:1bbd5f330277bbd9210f2e59aadb839e5835232d2e25276ecf557c50c43a827b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7096555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b36028bb5d3fca889fdea86f66126cfc8729e3491a8cd87fa30bd5f734c7c504`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:12:27 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 07:12:40 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 07:12:40 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 07:12:40 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 07:12:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 07:12:40 GMT
WORKDIR /notary/signer
# Tue, 06 Dec 2022 22:39:28 GMT
COPY /notary-signer ./ # buildkit
# Tue, 06 Dec 2022 22:39:29 GMT
RUN ./notary-signer --version # buildkit
# Tue, 06 Dec 2022 22:39:29 GMT
COPY ./signer-config.json . # buildkit
# Tue, 06 Dec 2022 22:39:30 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 22:39:30 GMT
USER notary
# Tue, 06 Dec 2022 22:39:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 22:39:30 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:6ca3c7abc8ed18b90618dae3d8ed39fa05a0357ae27fab896191fb471938ae78`  
		Last Modified: Sat, 12 Nov 2022 07:13:14 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f632f6d33140f2e49810b4f6a60512c22608edff7d44925891b00ea46ff0de`  
		Last Modified: Tue, 06 Dec 2022 22:39:59 GMT  
		Size: 4.3 MB (4292835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c606fcfa2e19c4f6d3a693676972656f2bc43efae9a9d54f864a770a2eafa414`  
		Last Modified: Tue, 06 Dec 2022 22:39:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66193bfc42da3bc86006fb987a16d17d0a4a2474345b0d2e368b491a46430f1`  
		Last Modified: Tue, 06 Dec 2022 22:39:58 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c6c82e57496f250c2f186949371758eaadcec7585343f26590d5c16a573b91`  
		Last Modified: Tue, 06 Dec 2022 22:39:58 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:498c86acef4e7f2834dd90e689801aef1b88b627d9e129f3a6189e0930ff0192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7194942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef80c38cb2ca79a82e9052b124f8d63f81817b8a8703daa01f5f4ecf663ffb3e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:29:11 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 05:29:25 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 05:29:25 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 05:29:25 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 05:29:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 05:29:25 GMT
WORKDIR /notary/signer
# Tue, 06 Dec 2022 21:11:56 GMT
COPY /notary-signer ./ # buildkit
# Tue, 06 Dec 2022 21:11:57 GMT
RUN ./notary-signer --version # buildkit
# Tue, 06 Dec 2022 21:11:57 GMT
COPY ./signer-config.json . # buildkit
# Tue, 06 Dec 2022 21:11:57 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:11:57 GMT
USER notary
# Tue, 06 Dec 2022 21:11:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:11:57 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:dab5959c551fe4b84515f58281a78c8105c856e6509e5d6d5f6140438605e776`  
		Last Modified: Sat, 12 Nov 2022 05:29:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b14d1b4267e479ad8f1fac7a64e07233bd7c89ee36b51b092df26b5acaf00a`  
		Last Modified: Tue, 06 Dec 2022 21:12:22 GMT  
		Size: 4.6 MB (4601650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f772838bb97e864711d746d9bf0775ae8af545a7bb7cd2ebbe21f964718dc23f`  
		Last Modified: Tue, 06 Dec 2022 21:12:21 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e1b90cbcbbc1c1469cdbe8696ac91e3fb1e2fc5c468c9ae2c7cb6cdd7e3457`  
		Last Modified: Tue, 06 Dec 2022 21:12:21 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dbe9d3143508321c172067cf85dba13d5c6ad5a2b54df08399d8a376cec5f9`  
		Last Modified: Tue, 06 Dec 2022 21:12:21 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer-0.7.0`

```console
$ docker pull notary@sha256:54736635ff9dcb0b71b83270e20b516afa3c8d7e932c1e1565f9049792b0e18a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer-0.7.0` - linux; amd64

```console
$ docker pull notary@sha256:0875013a6d3a2be8fb40d401accbd45ebbc071389ee97e1a75e068b3e1bf6872
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7565741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fde673ba5abe3aa357e4518af9cdde5b51cb4d9384bf71bdab1f7d329edaf55a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 06:38:02 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 06:38:08 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 06:38:08 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 06:38:08 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 06:38:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 06:38:08 GMT
WORKDIR /notary/signer
# Wed, 07 Dec 2022 00:19:42 GMT
COPY /notary-signer ./ # buildkit
# Wed, 07 Dec 2022 00:19:42 GMT
RUN ./notary-signer --version # buildkit
# Wed, 07 Dec 2022 00:19:42 GMT
COPY ./signer-config.json . # buildkit
# Wed, 07 Dec 2022 00:19:43 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 07 Dec 2022 00:19:43 GMT
USER notary
# Wed, 07 Dec 2022 00:19:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 07 Dec 2022 00:19:43 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:8da59cda2c120691b5be31fdc1571f10856ae5c4527c577ae2f76cd70fcd4a05`  
		Last Modified: Sat, 12 Nov 2022 06:38:29 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcfed49199016f957dddc67d897e93757dcc6a76a282a9f206a3449455e307b`  
		Last Modified: Wed, 07 Dec 2022 00:20:05 GMT  
		Size: 4.8 MB (4757304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf85ebd2351e71c23253b4d0b8761c6972e1dc5df54962090f047a8ca5e1b6d`  
		Last Modified: Wed, 07 Dec 2022 00:20:03 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eefdf52ec5e0b4f5987080be2a3bb44bd4e340fad81a1ab4376407900063f11`  
		Last Modified: Wed, 07 Dec 2022 00:20:03 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42341ba3d013ebf80c6d9dcbfe35a61125631b1d1133962eb9c18ca67e3e40b6`  
		Last Modified: Wed, 07 Dec 2022 00:20:04 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:dc674ebdc96dd1934111b4d84f9d56c55d21fc26cb078ec2f8c9a1bb836b16be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55989575380ac94315193ca596d70959ac8e2ec1c39eabaccfeb1966454be668`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:53:33 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:53:47 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 04:53:47 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 04:53:47 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:53:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:53:47 GMT
WORKDIR /notary/signer
# Tue, 06 Dec 2022 21:19:15 GMT
COPY /notary-signer ./ # buildkit
# Tue, 06 Dec 2022 21:19:15 GMT
RUN ./notary-signer --version # buildkit
# Tue, 06 Dec 2022 21:19:15 GMT
COPY ./signer-config.json . # buildkit
# Tue, 06 Dec 2022 21:19:15 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:19:15 GMT
USER notary
# Tue, 06 Dec 2022 21:19:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:19:15 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:125649f53222ca94f2e22db8ba79ba38d7d33fee96be71c6f2a0e58b1045ac49`  
		Last Modified: Sat, 12 Nov 2022 04:54:19 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47283c38f888cf865442bbf36d4aec3f09de0a9c8d2dd33dc606b2e19564c423`  
		Last Modified: Tue, 06 Dec 2022 21:19:46 GMT  
		Size: 4.5 MB (4520351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d490b0891554a66e5b88052b709c3633c6ec5df6f0ffa0794bbe31cdfee103`  
		Last Modified: Tue, 06 Dec 2022 21:19:45 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0052e17712c732b0feec88e761587d4df1400f0966d0196c6f4892dcc9c66b97`  
		Last Modified: Tue, 06 Dec 2022 21:19:46 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4036cef39afcea28c4572740467d6b3547376c97afcb9339c1a794fd69f47f3`  
		Last Modified: Tue, 06 Dec 2022 21:19:45 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:b4a6261a1055e75c9d91f6a585ab49b0825302f0659a68f7dc9158fff485a923
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7094071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c822e290dfeb3acdab813d11c76673853584b53d7a87a2f926409a07286a28f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:36:49 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:36:54 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 04:36:54 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 04:36:54 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:36:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:36:54 GMT
WORKDIR /notary/signer
# Tue, 06 Dec 2022 21:06:42 GMT
COPY /notary-signer ./ # buildkit
# Tue, 06 Dec 2022 21:06:43 GMT
RUN ./notary-signer --version # buildkit
# Tue, 06 Dec 2022 21:06:43 GMT
COPY ./signer-config.json . # buildkit
# Tue, 06 Dec 2022 21:06:43 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:06:43 GMT
USER notary
# Tue, 06 Dec 2022 21:06:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:06:43 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:92adb73f02c38f4aa06f3e987ca18858a12b469b490a35a7fb86b341f2b68fb4`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab5895b8bad28249cbb19462356cd068ed56cef4d074111981055ca4e250721`  
		Last Modified: Tue, 06 Dec 2022 21:07:07 GMT  
		Size: 4.4 MB (4384147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf66df20e765e5893cbceca4bbacc24dd5f8a6054942f5cc62bd888854e1624b`  
		Last Modified: Tue, 06 Dec 2022 21:07:06 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceef232e5818ab3f78ee04a825d2a889394315063ad4b561f19bd70522e2df6`  
		Last Modified: Tue, 06 Dec 2022 21:07:07 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9818996f8c494fa753d10c185478433296b820ffc74fe10cf37e2c45e1bb2b49`  
		Last Modified: Tue, 06 Dec 2022 21:07:07 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:79b4c323f58cb5f6ea257c2af5204098abeea66bb6d3c60b46f4693e04741701
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7381566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ddf368d5d9c9179b534f7d9a67b82e27281f60554a17dc0820eabc3abfca32c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:57:54 GMT
RUN adduser -D -H -g "" notary
# Sat, 12 Nov 2022 04:58:12 GMT
EXPOSE 4444
# Sat, 12 Nov 2022 04:58:12 GMT
EXPOSE 7899
# Sat, 12 Nov 2022 04:58:13 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:58:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:58:15 GMT
WORKDIR /notary/signer
# Wed, 16 Nov 2022 20:11:26 GMT
COPY file:044b2b6099382d2e11ff09d47c7a63f7cf3796f05317a8a2bbfed5d98c843503 in ./ 
# Wed, 16 Nov 2022 20:11:26 GMT
RUN ./notary-signer --version
# Wed, 16 Nov 2022 20:11:28 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Wed, 16 Nov 2022 20:11:29 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Wed, 16 Nov 2022 20:11:29 GMT
USER notary
# Wed, 16 Nov 2022 20:11:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Nov 2022 20:11:31 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:e26472dc994c1e659b114a40b8becb18e4595de57079b3495843fe3ee077329d`  
		Last Modified: Sat, 12 Nov 2022 04:58:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77cc9f8b030709827b83734498c26e9c13fdcad73c1751041bf38760164b7c8`  
		Last Modified: Wed, 16 Nov 2022 20:11:58 GMT  
		Size: 4.6 MB (4571177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d739be5aa3edcc7ba9f282a037921fc7c54d03aa47497444165ee21ada1487a6`  
		Last Modified: Wed, 16 Nov 2022 20:11:57 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f6cc98121c6d6e23c455cc4891ee75f1d872207a89e3ff24c67d8eedf86dac`  
		Last Modified: Wed, 16 Nov 2022 20:11:58 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:1bbd5f330277bbd9210f2e59aadb839e5835232d2e25276ecf557c50c43a827b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7096555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b36028bb5d3fca889fdea86f66126cfc8729e3491a8cd87fa30bd5f734c7c504`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:12:27 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 07:12:40 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 07:12:40 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 07:12:40 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 07:12:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 07:12:40 GMT
WORKDIR /notary/signer
# Tue, 06 Dec 2022 22:39:28 GMT
COPY /notary-signer ./ # buildkit
# Tue, 06 Dec 2022 22:39:29 GMT
RUN ./notary-signer --version # buildkit
# Tue, 06 Dec 2022 22:39:29 GMT
COPY ./signer-config.json . # buildkit
# Tue, 06 Dec 2022 22:39:30 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 22:39:30 GMT
USER notary
# Tue, 06 Dec 2022 22:39:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 22:39:30 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:6ca3c7abc8ed18b90618dae3d8ed39fa05a0357ae27fab896191fb471938ae78`  
		Last Modified: Sat, 12 Nov 2022 07:13:14 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f632f6d33140f2e49810b4f6a60512c22608edff7d44925891b00ea46ff0de`  
		Last Modified: Tue, 06 Dec 2022 22:39:59 GMT  
		Size: 4.3 MB (4292835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c606fcfa2e19c4f6d3a693676972656f2bc43efae9a9d54f864a770a2eafa414`  
		Last Modified: Tue, 06 Dec 2022 22:39:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66193bfc42da3bc86006fb987a16d17d0a4a2474345b0d2e368b491a46430f1`  
		Last Modified: Tue, 06 Dec 2022 22:39:58 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c6c82e57496f250c2f186949371758eaadcec7585343f26590d5c16a573b91`  
		Last Modified: Tue, 06 Dec 2022 22:39:58 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:498c86acef4e7f2834dd90e689801aef1b88b627d9e129f3a6189e0930ff0192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7194942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef80c38cb2ca79a82e9052b124f8d63f81817b8a8703daa01f5f4ecf663ffb3e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:29:11 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 05:29:25 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 05:29:25 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 05:29:25 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 05:29:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 05:29:25 GMT
WORKDIR /notary/signer
# Tue, 06 Dec 2022 21:11:56 GMT
COPY /notary-signer ./ # buildkit
# Tue, 06 Dec 2022 21:11:57 GMT
RUN ./notary-signer --version # buildkit
# Tue, 06 Dec 2022 21:11:57 GMT
COPY ./signer-config.json . # buildkit
# Tue, 06 Dec 2022 21:11:57 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 06 Dec 2022 21:11:57 GMT
USER notary
# Tue, 06 Dec 2022 21:11:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 06 Dec 2022 21:11:57 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:dab5959c551fe4b84515f58281a78c8105c856e6509e5d6d5f6140438605e776`  
		Last Modified: Sat, 12 Nov 2022 05:29:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b14d1b4267e479ad8f1fac7a64e07233bd7c89ee36b51b092df26b5acaf00a`  
		Last Modified: Tue, 06 Dec 2022 21:12:22 GMT  
		Size: 4.6 MB (4601650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f772838bb97e864711d746d9bf0775ae8af545a7bb7cd2ebbe21f964718dc23f`  
		Last Modified: Tue, 06 Dec 2022 21:12:21 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e1b90cbcbbc1c1469cdbe8696ac91e3fb1e2fc5c468c9ae2c7cb6cdd7e3457`  
		Last Modified: Tue, 06 Dec 2022 21:12:21 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dbe9d3143508321c172067cf85dba13d5c6ad5a2b54df08399d8a376cec5f9`  
		Last Modified: Tue, 06 Dec 2022 21:12:21 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
