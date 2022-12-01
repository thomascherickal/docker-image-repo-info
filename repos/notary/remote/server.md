## `notary:server`

```console
$ docker pull notary@sha256:f3f84d5f7afe21737791d069153932095867585f11a002dfc40212593e01afe7
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
$ docker pull notary@sha256:58bc5ef265e62ab7a2ae7e1a10a5b22380d7af0f5f104365512086ef322d44cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7952175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3167a0e1f8bcc0ff32c074e2321892e5652bd9802076ce92ca4d71a60309a6`
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
# Thu, 01 Dec 2022 21:08:44 GMT
COPY /notary-server ./ # buildkit
# Thu, 01 Dec 2022 21:08:45 GMT
RUN ./notary-server --version # buildkit
# Thu, 01 Dec 2022 21:08:45 GMT
COPY ./server-config.json . # buildkit
# Thu, 01 Dec 2022 21:08:45 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 01 Dec 2022 21:08:45 GMT
USER notary
# Thu, 01 Dec 2022 21:08:45 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Dec 2022 21:08:45 GMT
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
	-	`sha256:e1669a5657192b7591b8c93445a6af51a358d524ea446360f8c335f6ecf1d227`  
		Last Modified: Thu, 01 Dec 2022 21:09:03 GMT  
		Size: 5.1 MB (5143671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4ea97e159f009357d49f630574aca0b8c5806ff63620fe7f3a36ad29be3de4`  
		Last Modified: Thu, 01 Dec 2022 21:09:02 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6efe6729ab745a5926bfe4f16a3e6f5dbc064518b572b515be3ed0a1c3e046`  
		Last Modified: Thu, 01 Dec 2022 21:09:02 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40f9adfedcf2f2c2128ae6c102c48cb868d6e982a0f0331e9b1da304b1182e5`  
		Last Modified: Thu, 01 Dec 2022 21:09:02 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:8d8a1dd6ee5145dc225136e949d33be02829998678ab255572e6ab8ef3254e62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7505612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81472a503fcf990f31d46859094a7126ce3194bf712cb419ff499c9d7de868fc`
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
# Thu, 01 Dec 2022 21:29:49 GMT
COPY /notary-server ./ # buildkit
# Thu, 01 Dec 2022 21:29:49 GMT
RUN ./notary-server --version # buildkit
# Thu, 01 Dec 2022 21:29:49 GMT
COPY ./server-config.json . # buildkit
# Thu, 01 Dec 2022 21:29:50 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 01 Dec 2022 21:29:50 GMT
USER notary
# Thu, 01 Dec 2022 21:29:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Dec 2022 21:29:50 GMT
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
	-	`sha256:03931c55e6c9467510c658de352fc3d440933ce1b875add15973ad4926e089a2`  
		Last Modified: Thu, 01 Dec 2022 21:30:23 GMT  
		Size: 4.9 MB (4888310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ada81a7b17cb6304bf451a594dcadee8f42e345844b0a0363574e2f8fe18fcb`  
		Last Modified: Thu, 01 Dec 2022 21:30:22 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088666050c46bbc2e0d257e2fc2fe1937809a0a1e43f8452bd8da290aec3ca1d`  
		Last Modified: Thu, 01 Dec 2022 21:30:22 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc05f0f93e9db20e9c5d608de4a6080d2cc37d20f391b5e8440acd19425b820f`  
		Last Modified: Thu, 01 Dec 2022 21:30:22 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:6d1c91559b1a3fa9b99d0a26fbd8d353ce2643ee8cbf414fbab11a0bf91221c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7441471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c51c6583708b7f5c5375ade6c4155ac45dadc8c744c2d6faf5ad92d4457db900`
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
# Thu, 01 Dec 2022 21:25:01 GMT
COPY /notary-server ./ # buildkit
# Thu, 01 Dec 2022 21:25:02 GMT
RUN ./notary-server --version # buildkit
# Thu, 01 Dec 2022 21:25:02 GMT
COPY ./server-config.json . # buildkit
# Thu, 01 Dec 2022 21:25:02 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 01 Dec 2022 21:25:02 GMT
USER notary
# Thu, 01 Dec 2022 21:25:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Dec 2022 21:25:02 GMT
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
	-	`sha256:df89c28a607657c6db51dd765b4275074016fbe91701a6ec9e8116b436210268`  
		Last Modified: Thu, 01 Dec 2022 21:25:20 GMT  
		Size: 4.7 MB (4731484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d023b24f9587158dd752045a76d04f54d2fad5b7fc3436e7f0167da186a261`  
		Last Modified: Thu, 01 Dec 2022 21:25:19 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37acca650392c767479659c3a34eb3a50e4521ef6a931280fa2c1c3964fc9074`  
		Last Modified: Thu, 01 Dec 2022 21:25:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7486e0c1fa93bc01acddcabce35a565b0a64dcf1f77c323a3dc22f81ebb4c283`  
		Last Modified: Thu, 01 Dec 2022 21:25:19 GMT  
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
$ docker pull notary@sha256:481080f933fdd3d11a53d397dbc0a2682c2810a744e0f74a75b8ad26ef218f89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7437008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdd0a8c2f680ac5609ad99568d67113a0b32798d487c1e4391e1432951a30f9a`
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
# Thu, 01 Dec 2022 21:13:27 GMT
COPY /notary-server ./ # buildkit
# Thu, 01 Dec 2022 21:13:28 GMT
RUN ./notary-server --version # buildkit
# Thu, 01 Dec 2022 21:13:28 GMT
COPY ./server-config.json . # buildkit
# Thu, 01 Dec 2022 21:13:28 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 01 Dec 2022 21:13:28 GMT
USER notary
# Thu, 01 Dec 2022 21:13:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Dec 2022 21:13:28 GMT
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
	-	`sha256:74bad62533e55e9af5ca46e4488f0c4339bf288bf7266b6c61712c2960e25383`  
		Last Modified: Thu, 01 Dec 2022 21:14:01 GMT  
		Size: 4.6 MB (4633223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc7376d3793b1dee5f34afe1fc88eb7f0f592c90bf7e5faae346cc9a65771d0`  
		Last Modified: Thu, 01 Dec 2022 21:14:00 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee47e12779a3e539741186bcbef2e9f6fc69f0486c2e621786f709d5d45cb6f`  
		Last Modified: Thu, 01 Dec 2022 21:14:00 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca0eb1fc30161164b6ff68a049bc6625e85b4bfbb5688c3b45acc7d53801953`  
		Last Modified: Thu, 01 Dec 2022 21:13:59 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:440ccaeba070f526eec025ceca2d78a017bcb7150ab1d54d65f0c26b737a9843
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7562092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52ae88acc1fc3f444febc651b9c089bfda6d451c178f4ee439f4360293e8a82`
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
# Thu, 01 Dec 2022 21:33:44 GMT
COPY /notary-server ./ # buildkit
# Thu, 01 Dec 2022 21:33:45 GMT
RUN ./notary-server --version # buildkit
# Thu, 01 Dec 2022 21:33:45 GMT
COPY ./server-config.json . # buildkit
# Thu, 01 Dec 2022 21:33:45 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 01 Dec 2022 21:33:45 GMT
USER notary
# Thu, 01 Dec 2022 21:33:45 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Dec 2022 21:33:45 GMT
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
	-	`sha256:2ca9fe47baeaa63d6e98b88f0efe6bd243f32113042769a11a0926f506eb1bae`  
		Last Modified: Thu, 01 Dec 2022 21:34:18 GMT  
		Size: 5.0 MB (4968733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9fc0dc309f527f60bbec45fe5da7bd8904f8c3ca26eb96d5d8185b52024261`  
		Last Modified: Thu, 01 Dec 2022 21:34:17 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59633cbd4d45296699b2fad8dde298dd60466c888b3f4c8b7fbeb4abb449b19`  
		Last Modified: Thu, 01 Dec 2022 21:34:17 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01fe8b01794b9f20daa0c86ac241000234ac1f62971e0a083bf4dd6c7eb3836`  
		Last Modified: Thu, 01 Dec 2022 21:34:17 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
