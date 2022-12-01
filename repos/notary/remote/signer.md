## `notary:signer`

```console
$ docker pull notary@sha256:711810630cad732fa106b899cad15046201728a798f56c0f2503ad052113efa5
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
$ docker pull notary@sha256:c11517aaea8a82ff2dbf952d868402c793c5c20d68826fa2f20dfdb81a302509
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecad18a8b6de6c609392d14f6a7242047bbdc09a86a0a1f040902d0222cd497`
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
# Thu, 01 Dec 2022 21:08:51 GMT
COPY /notary-signer ./ # buildkit
# Thu, 01 Dec 2022 21:08:51 GMT
RUN ./notary-signer --version # buildkit
# Thu, 01 Dec 2022 21:08:51 GMT
COPY ./signer-config.json . # buildkit
# Thu, 01 Dec 2022 21:08:51 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 01 Dec 2022 21:08:51 GMT
USER notary
# Thu, 01 Dec 2022 21:08:51 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Dec 2022 21:08:51 GMT
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
	-	`sha256:d4fcb221fdf865f6cdc05eedd7cb2326b97a6c3f51830aa543e7edd017f8a968`  
		Last Modified: Thu, 01 Dec 2022 21:09:12 GMT  
		Size: 4.8 MB (4756811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7932f3ec7ad728cfdaededd5389441a85d29786cb206430e20b644eb162fcc20`  
		Last Modified: Thu, 01 Dec 2022 21:09:07 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706ad547c6e08933a817c68f21759f0de1563285f9bcfdb7bb84cb5b7655aa45`  
		Last Modified: Thu, 01 Dec 2022 21:09:11 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f1d2a5d728d1aef5c3e78ab76a21a37ab9868910e85fdaf4f11aa7f4113f49`  
		Last Modified: Thu, 01 Dec 2022 21:09:11 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:418023b51ad52b21eab841550c8e6c97ef74c04c919cbc434c9ad1358830548c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7135977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1806e6a47cfd1cfb95bc26c23cfaf907b66202e11ff3a62df7e6b94e5f5bb12d`
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
# Thu, 01 Dec 2022 21:30:02 GMT
COPY /notary-signer ./ # buildkit
# Thu, 01 Dec 2022 21:30:03 GMT
RUN ./notary-signer --version # buildkit
# Thu, 01 Dec 2022 21:30:03 GMT
COPY ./signer-config.json . # buildkit
# Thu, 01 Dec 2022 21:30:03 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 01 Dec 2022 21:30:03 GMT
USER notary
# Thu, 01 Dec 2022 21:30:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Dec 2022 21:30:03 GMT
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
	-	`sha256:47f31ee80a1b38f3eadc067071311d8ef42f6b198ddd35280fdb2b269ad796b0`  
		Last Modified: Thu, 01 Dec 2022 21:30:34 GMT  
		Size: 4.5 MB (4518738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6078e3c566b82b517eaef8817a8d991671d791e4b96312c016e49c64142dc3b3`  
		Last Modified: Thu, 01 Dec 2022 21:30:33 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db93ff20b065c26c587c7aac06f93e86b6f65e39e018cedcf37d2eaeac01de4`  
		Last Modified: Thu, 01 Dec 2022 21:30:34 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c57bf704776476a9fe3ff4fe9cc9775ae0c76a6de0f68c070e4bb8e6ec300c7`  
		Last Modified: Thu, 01 Dec 2022 21:30:33 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:442c73839cdce9519e7ebea7c489c41990bc102f411efd08293d346c5963c8a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7093232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d9416f7a095d7b8e5c701e2470408c531228a20c0ff9acd4ea3105fb8d2d34b`
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
# Thu, 01 Dec 2022 21:25:09 GMT
COPY /notary-signer ./ # buildkit
# Thu, 01 Dec 2022 21:25:09 GMT
RUN ./notary-signer --version # buildkit
# Thu, 01 Dec 2022 21:25:09 GMT
COPY ./signer-config.json . # buildkit
# Thu, 01 Dec 2022 21:25:09 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 01 Dec 2022 21:25:09 GMT
USER notary
# Thu, 01 Dec 2022 21:25:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Dec 2022 21:25:09 GMT
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
	-	`sha256:c0d747f5a02de8e8156e9a69040cf496e67243de40fa51d0ad0bf0b0eacd2f1a`  
		Last Modified: Thu, 01 Dec 2022 21:25:29 GMT  
		Size: 4.4 MB (4383307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0fb6d3c3272da919a75b61accaf1ed576f9a19b5ac842d56320ce7c3a11c76`  
		Last Modified: Thu, 01 Dec 2022 21:25:29 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c8a9973bf1f1434a71ed3995e277d383ab39dd5253eaa3e9716dd1917a2b30`  
		Last Modified: Thu, 01 Dec 2022 21:25:28 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1829ca2fb067e29d84a678cf4ca3ed2ef23c3ee6bd6123d81f67513d862cf22c`  
		Last Modified: Thu, 01 Dec 2022 21:25:28 GMT  
		Size: 383.0 B  
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
$ docker pull notary@sha256:db495a6accd22967fef651d6febd95e0186fb13381811a5b779a9068acc31bad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7096122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da19b3d00ce821131fc790288ea78d60acffa543d61b16c598273a392a3dc90`
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
# Thu, 01 Dec 2022 21:13:41 GMT
COPY /notary-signer ./ # buildkit
# Thu, 01 Dec 2022 21:13:42 GMT
RUN ./notary-signer --version # buildkit
# Thu, 01 Dec 2022 21:13:42 GMT
COPY ./signer-config.json . # buildkit
# Thu, 01 Dec 2022 21:13:42 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 01 Dec 2022 21:13:42 GMT
USER notary
# Thu, 01 Dec 2022 21:13:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Dec 2022 21:13:42 GMT
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
	-	`sha256:0cb86751e35e98f72eb0f6a8d0d66200b86c05d55e6cbaca52e384eb37159cc1`  
		Last Modified: Thu, 01 Dec 2022 21:14:13 GMT  
		Size: 4.3 MB (4292400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bb8243e2f0171fe93c273c3edb7ebe36f343874d9755c9ab6058bab1338083`  
		Last Modified: Thu, 01 Dec 2022 21:14:12 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cd23d8094cf142f72f9cb0c71c9855b6e5d34bc9d1296d0ba847f2cb0ad1fb`  
		Last Modified: Thu, 01 Dec 2022 21:14:12 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410a5ab2a349cbe402b9155468b8179e514bf7f4d3ee21cd5f9c94b0fed11d0d`  
		Last Modified: Thu, 01 Dec 2022 21:14:12 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:41d5614bdf524bce78a3dbd2f1cebc02a117b8dfa3f0f43e5ec52d6a22f3e7bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7194501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d864f5f81cf14a466605565e9505dd2e6fabefca8a34c59adf3c5a9aabc562`
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
# Thu, 01 Dec 2022 21:34:00 GMT
COPY /notary-signer ./ # buildkit
# Thu, 01 Dec 2022 21:34:00 GMT
RUN ./notary-signer --version # buildkit
# Thu, 01 Dec 2022 21:34:00 GMT
COPY ./signer-config.json . # buildkit
# Thu, 01 Dec 2022 21:34:00 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 01 Dec 2022 21:34:00 GMT
USER notary
# Thu, 01 Dec 2022 21:34:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Dec 2022 21:34:00 GMT
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
	-	`sha256:e255c766b68e7e8637de1198ef2a28e99218a61034439c929e728df84e5e6ed4`  
		Last Modified: Thu, 01 Dec 2022 21:34:25 GMT  
		Size: 4.6 MB (4601206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cb257c7619298f400163df54ba5a72ca18d5fe4427aa158485930ee21f7b15`  
		Last Modified: Thu, 01 Dec 2022 21:34:24 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630f48c4cfad126908e3b27326f761b012733498003f6e9a4778a6db53dd171b`  
		Last Modified: Thu, 01 Dec 2022 21:34:24 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d35d1a828a35c6803868dade9a927525fbf9dcfe04fbc62cb55cd22c9619a`  
		Last Modified: Thu, 01 Dec 2022 21:34:24 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
