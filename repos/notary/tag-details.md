<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.7.0`](#notaryserver-070)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.7.0`](#notarysigner-070)

## `notary:server`

```console
$ docker pull notary@sha256:5c5fd1b76591050114ec63fc9b03cc3ea6d44f7869039586b703915c6fb28af5
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
$ docker pull notary@sha256:604804139526f61006ecaed57b24fd71298759cb029176b7f462e4958b8d2d5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7957067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25990f5bee6ca64a8080d14dc3d002e1261a2b6fa5bf0cd6ce37796eda026e9e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:15:51 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 10:15:51 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 11 Feb 2023 10:15:51 GMT
ENV INSTALLDIR=/notary/server
# Sat, 11 Feb 2023 10:15:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 11 Feb 2023 10:15:51 GMT
WORKDIR /notary/server
# Wed, 08 Mar 2023 00:49:15 GMT
COPY /notary-server ./ # buildkit
# Wed, 08 Mar 2023 00:49:15 GMT
RUN ./notary-server --version # buildkit
# Wed, 08 Mar 2023 00:49:15 GMT
COPY ./server-config.json . # buildkit
# Wed, 08 Mar 2023 00:49:15 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:49:15 GMT
USER notary
# Wed, 08 Mar 2023 00:49:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:49:15 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a8bf9348133d1e770b90e9991d3f65c555075470962fb5e1321cf7201947a6`  
		Last Modified: Sat, 11 Feb 2023 10:16:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760faad2c97be8ade88979e95e3256e1d5d0866d3a50a935d789b03b24e6415`  
		Last Modified: Sat, 11 Feb 2023 10:16:23 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2df55172ca943aea44947a07407532c65ec992355ac8f63e2b62af1fc9407da`  
		Last Modified: Wed, 08 Mar 2023 00:49:32 GMT  
		Size: 5.1 MB (5147069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc53564397309052ac64f81f4aaf11752f427caefc737d7144be9a35a37d1bd1`  
		Last Modified: Wed, 08 Mar 2023 00:49:32 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab4a116adb5f5b80fda19935d7ce203ac6d2a495b9b108b064a0922484843cc`  
		Last Modified: Wed, 08 Mar 2023 00:49:32 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41160ed84ebf6a530e72036c3bfed555cd739ed0b93a1a70196f9a1d4d623f53`  
		Last Modified: Wed, 08 Mar 2023 00:49:31 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:ee501b399bd902cc8474e1c86f8948bed8fcab0616f734a15509d833a2d0ccae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7510958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a61490d8286b1d114bf6563aaf5f8e45b675ff88a1b8c8f3a6b57372d3a936`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:16:13 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 08 Mar 2023 00:16:13 GMT
EXPOSE map[4443/tcp:{}]
# Wed, 08 Mar 2023 00:16:13 GMT
ENV INSTALLDIR=/notary/server
# Wed, 08 Mar 2023 00:16:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 08 Mar 2023 00:16:13 GMT
WORKDIR /notary/server
# Mon, 13 Mar 2023 22:40:32 GMT
COPY /notary-server ./ # buildkit
# Mon, 13 Mar 2023 22:40:32 GMT
RUN ./notary-server --version # buildkit
# Mon, 13 Mar 2023 22:40:32 GMT
COPY ./server-config.json . # buildkit
# Mon, 13 Mar 2023 22:40:32 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 13 Mar 2023 22:40:32 GMT
USER notary
# Mon, 13 Mar 2023 22:40:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 13 Mar 2023 22:40:32 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b05793ac14c68387ad3a34fa8d5d4136f040e8b820b1eee3595d30529d87e46`  
		Last Modified: Wed, 08 Mar 2023 00:17:02 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214377c027ebc3bfa8cf5d9c6adfe42cde43421c65fc600f490de087016f240c`  
		Last Modified: Wed, 08 Mar 2023 00:17:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c71e9ab430b4c5bcd0d967ba3a562a2fc4ff95a3e08cd21985f55976e01c48b`  
		Last Modified: Mon, 13 Mar 2023 22:40:59 GMT  
		Size: 4.9 MB (4891948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f150020030a5ab0bc12d84770554a7e85e6084ab46764f34f4516a16d076d6`  
		Last Modified: Mon, 13 Mar 2023 22:40:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3706a58a941854c47a87a64bef0ea94c008454a5248287746bd81e3dad0be5`  
		Last Modified: Mon, 13 Mar 2023 22:40:58 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f171ebb22f11fd496bf6df25a11cde2c824b6908306a249bea91629356e627ce`  
		Last Modified: Mon, 13 Mar 2023 22:40:58 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:4d250233fdf58742bdb366e836b7c60b619743a347de6b6f7c9eb1cc55e5fe65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f4b0f380c3527d88d2da48ea19e6ea3ce16ba397ac87fcaec377c66070603c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:01:39 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 02:01:39 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 11 Feb 2023 02:01:39 GMT
ENV INSTALLDIR=/notary/server
# Sat, 11 Feb 2023 02:01:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 11 Feb 2023 02:01:39 GMT
WORKDIR /notary/server
# Wed, 08 Mar 2023 00:05:23 GMT
COPY /notary-server ./ # buildkit
# Wed, 08 Mar 2023 00:05:24 GMT
RUN ./notary-server --version # buildkit
# Wed, 08 Mar 2023 00:05:24 GMT
COPY ./server-config.json . # buildkit
# Wed, 08 Mar 2023 00:05:24 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:05:24 GMT
USER notary
# Wed, 08 Mar 2023 00:05:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:05:24 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b9e3dceb52b5f1909f74e5761d8b0968630630d4c5d37134133ff1529d57ca`  
		Last Modified: Sat, 11 Feb 2023 02:02:10 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9362a2b1100a2d3d12c1fa9941ef61cde36540c7d918725c75f1730eaaed51e`  
		Last Modified: Sat, 11 Feb 2023 02:02:09 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af65511d2d3fd0c0a35b03af44b1d1549f49896f89e6a0c119e7bae191923d5c`  
		Last Modified: Wed, 08 Mar 2023 00:05:41 GMT  
		Size: 4.7 MB (4732808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3fbc8df4b893167b6524a94b784f83d8c9f2ddf16bdab1b646f4b1dcec8b8e`  
		Last Modified: Wed, 08 Mar 2023 00:05:41 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ad95bb804cb93a324515db8c684035512869aa854e7de02a01f1f39828bd52`  
		Last Modified: Wed, 08 Mar 2023 00:05:41 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac29e62b8f7c59b3957f88ba49961df75e4ce160f28a9b39dfef2a05b846322`  
		Last Modified: Wed, 08 Mar 2023 00:05:41 GMT  
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
$ docker pull notary@sha256:2db26874d36ba99b64f33312719e187dd9980b7328b0aa7543780185eef1675f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74b96c5feff45ae934526e57edab7769bfad0411a9cfe5b74b723371fa48e2b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:31:58 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 09:31:58 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 11 Feb 2023 09:31:58 GMT
ENV INSTALLDIR=/notary/server
# Sat, 11 Feb 2023 09:31:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 11 Feb 2023 09:31:58 GMT
WORKDIR /notary/server
# Wed, 08 Mar 2023 00:51:02 GMT
COPY /notary-server ./ # buildkit
# Wed, 08 Mar 2023 00:51:03 GMT
RUN ./notary-server --version # buildkit
# Wed, 08 Mar 2023 00:51:03 GMT
COPY ./server-config.json . # buildkit
# Wed, 08 Mar 2023 00:51:04 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:51:04 GMT
USER notary
# Wed, 08 Mar 2023 00:51:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:51:04 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d271c42b70a8c82b552b2772787a6cac62d60cdc88c599bd983e06b4b1199`  
		Last Modified: Sat, 11 Feb 2023 09:33:10 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17b8bc3dd04442591c8af362c063ac63f5cf8890143e98399dcc289f1979b12`  
		Last Modified: Sat, 11 Feb 2023 09:33:08 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db80eee1c1a3a4255721bcde302a3be6a3d5ee5a02ebea316b4345ec5ab5b436`  
		Last Modified: Wed, 08 Mar 2023 00:51:35 GMT  
		Size: 4.6 MB (4637497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cda42b97cb66a057cfa129de14d6c87b4c772de9821c98f5a2dd8f87ec5466`  
		Last Modified: Wed, 08 Mar 2023 00:51:34 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3329ec8c5aec01bef13887ae95dfc28fbe8d3e35c11b095bacc1c37d8ab8231b`  
		Last Modified: Wed, 08 Mar 2023 00:51:34 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0da99db09af96b4eab45370e4f3b5092445f0efd78d2fa60d38dfa23216d4e9`  
		Last Modified: Wed, 08 Mar 2023 00:51:34 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:6b5bc6be35eeabe7a415151f034fe195a46bd2360b727c1f2f3003c9f3837323
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51aee0bdef2f021f739d812aae3c78fa6ecbaf2ef8a7053bb0c7047642fdba85`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:38:26 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 03:38:26 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 11 Feb 2023 03:38:26 GMT
ENV INSTALLDIR=/notary/server
# Sat, 11 Feb 2023 03:38:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 11 Feb 2023 03:38:26 GMT
WORKDIR /notary/server
# Wed, 08 Mar 2023 00:11:49 GMT
COPY /notary-server ./ # buildkit
# Wed, 08 Mar 2023 00:11:49 GMT
RUN ./notary-server --version # buildkit
# Wed, 08 Mar 2023 00:11:49 GMT
COPY ./server-config.json . # buildkit
# Wed, 08 Mar 2023 00:11:50 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:11:50 GMT
USER notary
# Wed, 08 Mar 2023 00:11:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:11:50 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf825008c0747d1db1e6a08e31a5fa2a33c8e0f8a5fe8b2f86af75110c97e790`  
		Last Modified: Sat, 11 Feb 2023 03:39:15 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdd04f22f8d5c18f264048c202d6471e42bdd87d0431faf250d202652262e4e`  
		Last Modified: Sat, 11 Feb 2023 03:39:14 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc71a9b066760efc29c5477dcc54043fe02f65015de6816216648e4068070734`  
		Last Modified: Wed, 08 Mar 2023 00:12:19 GMT  
		Size: 5.0 MB (4974127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419ab3690a5801a73dded94eb55932354ef19f810c84f2dc8a1d8c012c13ab23`  
		Last Modified: Wed, 08 Mar 2023 00:12:19 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16532dfb75d7758f05901914350d05e44b0cd71c53551a5e84711fa80b897374`  
		Last Modified: Wed, 08 Mar 2023 00:12:18 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eae4b075547e304461b5a812d813829aac1510e460d96e99ad5c3f02f4f8de`  
		Last Modified: Wed, 08 Mar 2023 00:12:18 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:5c5fd1b76591050114ec63fc9b03cc3ea6d44f7869039586b703915c6fb28af5
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
$ docker pull notary@sha256:604804139526f61006ecaed57b24fd71298759cb029176b7f462e4958b8d2d5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7957067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25990f5bee6ca64a8080d14dc3d002e1261a2b6fa5bf0cd6ce37796eda026e9e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:15:51 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 10:15:51 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 11 Feb 2023 10:15:51 GMT
ENV INSTALLDIR=/notary/server
# Sat, 11 Feb 2023 10:15:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 11 Feb 2023 10:15:51 GMT
WORKDIR /notary/server
# Wed, 08 Mar 2023 00:49:15 GMT
COPY /notary-server ./ # buildkit
# Wed, 08 Mar 2023 00:49:15 GMT
RUN ./notary-server --version # buildkit
# Wed, 08 Mar 2023 00:49:15 GMT
COPY ./server-config.json . # buildkit
# Wed, 08 Mar 2023 00:49:15 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:49:15 GMT
USER notary
# Wed, 08 Mar 2023 00:49:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:49:15 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a8bf9348133d1e770b90e9991d3f65c555075470962fb5e1321cf7201947a6`  
		Last Modified: Sat, 11 Feb 2023 10:16:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760faad2c97be8ade88979e95e3256e1d5d0866d3a50a935d789b03b24e6415`  
		Last Modified: Sat, 11 Feb 2023 10:16:23 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2df55172ca943aea44947a07407532c65ec992355ac8f63e2b62af1fc9407da`  
		Last Modified: Wed, 08 Mar 2023 00:49:32 GMT  
		Size: 5.1 MB (5147069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc53564397309052ac64f81f4aaf11752f427caefc737d7144be9a35a37d1bd1`  
		Last Modified: Wed, 08 Mar 2023 00:49:32 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab4a116adb5f5b80fda19935d7ce203ac6d2a495b9b108b064a0922484843cc`  
		Last Modified: Wed, 08 Mar 2023 00:49:32 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41160ed84ebf6a530e72036c3bfed555cd739ed0b93a1a70196f9a1d4d623f53`  
		Last Modified: Wed, 08 Mar 2023 00:49:31 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:ee501b399bd902cc8474e1c86f8948bed8fcab0616f734a15509d833a2d0ccae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7510958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a61490d8286b1d114bf6563aaf5f8e45b675ff88a1b8c8f3a6b57372d3a936`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:16:13 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 08 Mar 2023 00:16:13 GMT
EXPOSE map[4443/tcp:{}]
# Wed, 08 Mar 2023 00:16:13 GMT
ENV INSTALLDIR=/notary/server
# Wed, 08 Mar 2023 00:16:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 08 Mar 2023 00:16:13 GMT
WORKDIR /notary/server
# Mon, 13 Mar 2023 22:40:32 GMT
COPY /notary-server ./ # buildkit
# Mon, 13 Mar 2023 22:40:32 GMT
RUN ./notary-server --version # buildkit
# Mon, 13 Mar 2023 22:40:32 GMT
COPY ./server-config.json . # buildkit
# Mon, 13 Mar 2023 22:40:32 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 13 Mar 2023 22:40:32 GMT
USER notary
# Mon, 13 Mar 2023 22:40:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 13 Mar 2023 22:40:32 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b05793ac14c68387ad3a34fa8d5d4136f040e8b820b1eee3595d30529d87e46`  
		Last Modified: Wed, 08 Mar 2023 00:17:02 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214377c027ebc3bfa8cf5d9c6adfe42cde43421c65fc600f490de087016f240c`  
		Last Modified: Wed, 08 Mar 2023 00:17:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c71e9ab430b4c5bcd0d967ba3a562a2fc4ff95a3e08cd21985f55976e01c48b`  
		Last Modified: Mon, 13 Mar 2023 22:40:59 GMT  
		Size: 4.9 MB (4891948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f150020030a5ab0bc12d84770554a7e85e6084ab46764f34f4516a16d076d6`  
		Last Modified: Mon, 13 Mar 2023 22:40:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3706a58a941854c47a87a64bef0ea94c008454a5248287746bd81e3dad0be5`  
		Last Modified: Mon, 13 Mar 2023 22:40:58 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f171ebb22f11fd496bf6df25a11cde2c824b6908306a249bea91629356e627ce`  
		Last Modified: Mon, 13 Mar 2023 22:40:58 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:4d250233fdf58742bdb366e836b7c60b619743a347de6b6f7c9eb1cc55e5fe65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f4b0f380c3527d88d2da48ea19e6ea3ce16ba397ac87fcaec377c66070603c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:01:39 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 02:01:39 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 11 Feb 2023 02:01:39 GMT
ENV INSTALLDIR=/notary/server
# Sat, 11 Feb 2023 02:01:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 11 Feb 2023 02:01:39 GMT
WORKDIR /notary/server
# Wed, 08 Mar 2023 00:05:23 GMT
COPY /notary-server ./ # buildkit
# Wed, 08 Mar 2023 00:05:24 GMT
RUN ./notary-server --version # buildkit
# Wed, 08 Mar 2023 00:05:24 GMT
COPY ./server-config.json . # buildkit
# Wed, 08 Mar 2023 00:05:24 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:05:24 GMT
USER notary
# Wed, 08 Mar 2023 00:05:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:05:24 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b9e3dceb52b5f1909f74e5761d8b0968630630d4c5d37134133ff1529d57ca`  
		Last Modified: Sat, 11 Feb 2023 02:02:10 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9362a2b1100a2d3d12c1fa9941ef61cde36540c7d918725c75f1730eaaed51e`  
		Last Modified: Sat, 11 Feb 2023 02:02:09 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af65511d2d3fd0c0a35b03af44b1d1549f49896f89e6a0c119e7bae191923d5c`  
		Last Modified: Wed, 08 Mar 2023 00:05:41 GMT  
		Size: 4.7 MB (4732808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3fbc8df4b893167b6524a94b784f83d8c9f2ddf16bdab1b646f4b1dcec8b8e`  
		Last Modified: Wed, 08 Mar 2023 00:05:41 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ad95bb804cb93a324515db8c684035512869aa854e7de02a01f1f39828bd52`  
		Last Modified: Wed, 08 Mar 2023 00:05:41 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac29e62b8f7c59b3957f88ba49961df75e4ce160f28a9b39dfef2a05b846322`  
		Last Modified: Wed, 08 Mar 2023 00:05:41 GMT  
		Size: 384.0 B  
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
$ docker pull notary@sha256:2db26874d36ba99b64f33312719e187dd9980b7328b0aa7543780185eef1675f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74b96c5feff45ae934526e57edab7769bfad0411a9cfe5b74b723371fa48e2b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:31:58 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 09:31:58 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 11 Feb 2023 09:31:58 GMT
ENV INSTALLDIR=/notary/server
# Sat, 11 Feb 2023 09:31:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 11 Feb 2023 09:31:58 GMT
WORKDIR /notary/server
# Wed, 08 Mar 2023 00:51:02 GMT
COPY /notary-server ./ # buildkit
# Wed, 08 Mar 2023 00:51:03 GMT
RUN ./notary-server --version # buildkit
# Wed, 08 Mar 2023 00:51:03 GMT
COPY ./server-config.json . # buildkit
# Wed, 08 Mar 2023 00:51:04 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:51:04 GMT
USER notary
# Wed, 08 Mar 2023 00:51:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:51:04 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d271c42b70a8c82b552b2772787a6cac62d60cdc88c599bd983e06b4b1199`  
		Last Modified: Sat, 11 Feb 2023 09:33:10 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17b8bc3dd04442591c8af362c063ac63f5cf8890143e98399dcc289f1979b12`  
		Last Modified: Sat, 11 Feb 2023 09:33:08 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db80eee1c1a3a4255721bcde302a3be6a3d5ee5a02ebea316b4345ec5ab5b436`  
		Last Modified: Wed, 08 Mar 2023 00:51:35 GMT  
		Size: 4.6 MB (4637497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cda42b97cb66a057cfa129de14d6c87b4c772de9821c98f5a2dd8f87ec5466`  
		Last Modified: Wed, 08 Mar 2023 00:51:34 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3329ec8c5aec01bef13887ae95dfc28fbe8d3e35c11b095bacc1c37d8ab8231b`  
		Last Modified: Wed, 08 Mar 2023 00:51:34 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0da99db09af96b4eab45370e4f3b5092445f0efd78d2fa60d38dfa23216d4e9`  
		Last Modified: Wed, 08 Mar 2023 00:51:34 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:6b5bc6be35eeabe7a415151f034fe195a46bd2360b727c1f2f3003c9f3837323
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51aee0bdef2f021f739d812aae3c78fa6ecbaf2ef8a7053bb0c7047642fdba85`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:38:26 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 03:38:26 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 11 Feb 2023 03:38:26 GMT
ENV INSTALLDIR=/notary/server
# Sat, 11 Feb 2023 03:38:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 11 Feb 2023 03:38:26 GMT
WORKDIR /notary/server
# Wed, 08 Mar 2023 00:11:49 GMT
COPY /notary-server ./ # buildkit
# Wed, 08 Mar 2023 00:11:49 GMT
RUN ./notary-server --version # buildkit
# Wed, 08 Mar 2023 00:11:49 GMT
COPY ./server-config.json . # buildkit
# Wed, 08 Mar 2023 00:11:50 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:11:50 GMT
USER notary
# Wed, 08 Mar 2023 00:11:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:11:50 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf825008c0747d1db1e6a08e31a5fa2a33c8e0f8a5fe8b2f86af75110c97e790`  
		Last Modified: Sat, 11 Feb 2023 03:39:15 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdd04f22f8d5c18f264048c202d6471e42bdd87d0431faf250d202652262e4e`  
		Last Modified: Sat, 11 Feb 2023 03:39:14 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc71a9b066760efc29c5477dcc54043fe02f65015de6816216648e4068070734`  
		Last Modified: Wed, 08 Mar 2023 00:12:19 GMT  
		Size: 5.0 MB (4974127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419ab3690a5801a73dded94eb55932354ef19f810c84f2dc8a1d8c012c13ab23`  
		Last Modified: Wed, 08 Mar 2023 00:12:19 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16532dfb75d7758f05901914350d05e44b0cd71c53551a5e84711fa80b897374`  
		Last Modified: Wed, 08 Mar 2023 00:12:18 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eae4b075547e304461b5a812d813829aac1510e460d96e99ad5c3f02f4f8de`  
		Last Modified: Wed, 08 Mar 2023 00:12:18 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer`

```console
$ docker pull notary@sha256:814804d74affec15f0d06a952ee8cc77452498ea6a2273cce04853127054f657
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
$ docker pull notary@sha256:c251779f1417ae5a5ee417d2d30e686eabbbb8de059978fa36f37aad9946b69f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7571275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b0be1197a26a971e5761cf8ccd7b56756b8d45fcaccf0193ffd72e852d107f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:15:51 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 10:16:14 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 10:16:14 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 10:16:14 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 10:16:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 10:16:14 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:49:22 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
USER notary
# Wed, 08 Mar 2023 00:49:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:49:23 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a8bf9348133d1e770b90e9991d3f65c555075470962fb5e1321cf7201947a6`  
		Last Modified: Sat, 11 Feb 2023 10:16:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0208e6d213823747dbf355ecd6e4879b414b1413e219476f0ffa3791d92aade7`  
		Last Modified: Sat, 11 Feb 2023 10:16:33 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d4813226483e6e0e68e4703b12d04bf207dd1e73af737985a819e977cf180b`  
		Last Modified: Wed, 08 Mar 2023 00:49:41 GMT  
		Size: 4.8 MB (4761343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fe5ef8141b6313f5d7afeb9c50c6567fe00bd4c6c5525f0b083735b3735dd6`  
		Last Modified: Wed, 08 Mar 2023 00:49:40 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18688d46ffe85cf58379eff4073d0f279e209261cb80dcc23b613698bacc134`  
		Last Modified: Wed, 08 Mar 2023 00:49:40 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e0a2298e2263fef9565a3cf84018cadde98b1f0ec959259993a6654fcc6579`  
		Last Modified: Wed, 08 Mar 2023 00:49:40 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:6216b68394c7b4e65f20eb11cad25ac367c0478004def016247f5d7597da696c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f92b4b68b3a717c29b9a43adbaa0bee16844e3aa91f027fd94fd9aa0b8037262`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:16:13 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 08 Mar 2023 00:16:43 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 08 Mar 2023 00:16:43 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 08 Mar 2023 00:16:43 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 08 Mar 2023 00:16:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 08 Mar 2023 00:16:43 GMT
WORKDIR /notary/signer
# Mon, 13 Mar 2023 22:40:43 GMT
COPY /notary-signer ./ # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
RUN ./notary-signer --version # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
COPY ./signer-config.json . # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
USER notary
# Mon, 13 Mar 2023 22:40:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 13 Mar 2023 22:40:43 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b05793ac14c68387ad3a34fa8d5d4136f040e8b820b1eee3595d30529d87e46`  
		Last Modified: Wed, 08 Mar 2023 00:17:02 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8867bd3aa695c936397740852a2a23245f7a8147431da0dea7ea79cb52c3fb7`  
		Last Modified: Wed, 08 Mar 2023 00:17:12 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9d6f44471853d748615de79835f860dbaf6a96899425bfe41892a55b8bbc82`  
		Last Modified: Mon, 13 Mar 2023 22:41:10 GMT  
		Size: 4.5 MB (4524257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a29049d4e5f31919a6825670eff28003d1d6a5e8a1a0db07cb80c508d56339`  
		Last Modified: Mon, 13 Mar 2023 22:41:09 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0e82b1ac8c1d3b1d7406e09d51ada3c9d5eef0b16c90412117a62e19a79f64`  
		Last Modified: Mon, 13 Mar 2023 22:41:09 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97710136b3555e60fb404524d8523f81cc0860b525a91fa4bef04700c7b55915`  
		Last Modified: Mon, 13 Mar 2023 22:41:09 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:926e06c706fe49616d9cc65fb3fc800f72c379ac63bb1533ebc92c19b9b5227a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7101769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f95704c1a8b8cf1b5c35f8c60600a55bd4e16456cf1996e14c199d5a3bd1ed`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:01:39 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 02:01:58 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 02:01:58 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 02:01:58 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 02:01:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 02:01:58 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:05:31 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:05:31 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:05:31 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:05:31 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:05:31 GMT
USER notary
# Wed, 08 Mar 2023 00:05:31 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:05:31 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b9e3dceb52b5f1909f74e5761d8b0968630630d4c5d37134133ff1529d57ca`  
		Last Modified: Sat, 11 Feb 2023 02:02:10 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9044747e4fd585aae1a06ddae8513379f85e397343798bc36f0e5504eaa9863f`  
		Last Modified: Sat, 11 Feb 2023 02:02:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37e617a66458e3ef4cc167492040ccc44e181a925937ae2855939d2780abb36`  
		Last Modified: Wed, 08 Mar 2023 00:05:51 GMT  
		Size: 4.4 MB (4390100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7741f3fe119ab783dd0fc9d701e877326371112f6be0f0f217bd515948be20fa`  
		Last Modified: Wed, 08 Mar 2023 00:05:50 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe4596223bf9430c304a6c7dcfad77fd3dc07c3d7f662be26b2989d9d9f6dfe`  
		Last Modified: Wed, 08 Mar 2023 00:05:50 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd11a87326463f869d1ba6c1bca519d2d6d4d5f84dfbe7b5eb36c194c7e614e`  
		Last Modified: Wed, 08 Mar 2023 00:05:50 GMT  
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
$ docker pull notary@sha256:606c37e1d97f4e68ec67ee57439cbcefd35416825bbee5a8438fea16cf305ab1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7102909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d66c8f75871355a84a407a350373d37201ae2aabe85cf2690b4d651da520a1c2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:31:58 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 09:32:48 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 09:32:48 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 09:32:48 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 09:32:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 09:32:48 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:51:17 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
USER notary
# Wed, 08 Mar 2023 00:51:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:51:18 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d271c42b70a8c82b552b2772787a6cac62d60cdc88c599bd983e06b4b1199`  
		Last Modified: Sat, 11 Feb 2023 09:33:10 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11d0b9967527e3e2fe9a387dd1b08ba83b7816d9e3863fb0f3e9c0a13f0225d`  
		Last Modified: Sat, 11 Feb 2023 09:33:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02a9326979cee7618aa2b342258e4cbc31c56b91a4e7e8e89eff264c67e95f6`  
		Last Modified: Wed, 08 Mar 2023 00:51:47 GMT  
		Size: 4.3 MB (4296112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808f46240e2aaa0c8f9fcfd65d773fc98ad9c37bd27eb1aeb70ce112edf1ea7b`  
		Last Modified: Wed, 08 Mar 2023 00:51:46 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfc68a2dc7ed5e20299b9ec5b2c868071a1ab4f3aaee290a0da97297b5d30e3`  
		Last Modified: Wed, 08 Mar 2023 00:51:46 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9b06a55652879187796edbb714b3d74db89083480a9347c81e1573381e9eef`  
		Last Modified: Wed, 08 Mar 2023 00:51:46 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:abfdfe9dbde3305247e776f74ae5d4099b7c5219de959bc45f17b176e6e98dd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7201015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d2c656f5776c347bac9afaa7f72464bdbb3b96dab6e81f650def3f08fe52c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:38:26 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 03:38:57 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 03:38:57 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 03:38:57 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 03:38:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 03:38:57 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:12:03 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:12:03 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:12:04 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:12:04 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:12:04 GMT
USER notary
# Wed, 08 Mar 2023 00:12:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:12:04 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf825008c0747d1db1e6a08e31a5fa2a33c8e0f8a5fe8b2f86af75110c97e790`  
		Last Modified: Sat, 11 Feb 2023 03:39:15 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47b3001bbc3d992bc8bd18f0274d2c096ab38122bfe91ebb713a068610faf80`  
		Last Modified: Sat, 11 Feb 2023 03:39:21 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabbaa0ac8ed6dfd08e91e9308501b5f3fa7aa8d1daf1f4a29f94ed70b293e76`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 4.6 MB (4605262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6168f2066015c6e1d056de0590b9058c7af98779aff58a8fe380fd458a4ed`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b309adaebe295395e40d60e06633c7bf6897b14e3b191a69619b8b19cbe4c03a`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc5983824d5ba6398ee6e275f8ebbc82284ec48ed5f55ab1ebb58db0a9e6177`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer-0.7.0`

```console
$ docker pull notary@sha256:814804d74affec15f0d06a952ee8cc77452498ea6a2273cce04853127054f657
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
$ docker pull notary@sha256:c251779f1417ae5a5ee417d2d30e686eabbbb8de059978fa36f37aad9946b69f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7571275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b0be1197a26a971e5761cf8ccd7b56756b8d45fcaccf0193ffd72e852d107f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:15:51 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 10:16:14 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 10:16:14 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 10:16:14 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 10:16:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 10:16:14 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:49:22 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
USER notary
# Wed, 08 Mar 2023 00:49:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:49:23 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a8bf9348133d1e770b90e9991d3f65c555075470962fb5e1321cf7201947a6`  
		Last Modified: Sat, 11 Feb 2023 10:16:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0208e6d213823747dbf355ecd6e4879b414b1413e219476f0ffa3791d92aade7`  
		Last Modified: Sat, 11 Feb 2023 10:16:33 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d4813226483e6e0e68e4703b12d04bf207dd1e73af737985a819e977cf180b`  
		Last Modified: Wed, 08 Mar 2023 00:49:41 GMT  
		Size: 4.8 MB (4761343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fe5ef8141b6313f5d7afeb9c50c6567fe00bd4c6c5525f0b083735b3735dd6`  
		Last Modified: Wed, 08 Mar 2023 00:49:40 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18688d46ffe85cf58379eff4073d0f279e209261cb80dcc23b613698bacc134`  
		Last Modified: Wed, 08 Mar 2023 00:49:40 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e0a2298e2263fef9565a3cf84018cadde98b1f0ec959259993a6654fcc6579`  
		Last Modified: Wed, 08 Mar 2023 00:49:40 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:6216b68394c7b4e65f20eb11cad25ac367c0478004def016247f5d7597da696c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f92b4b68b3a717c29b9a43adbaa0bee16844e3aa91f027fd94fd9aa0b8037262`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:16:13 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 08 Mar 2023 00:16:43 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 08 Mar 2023 00:16:43 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 08 Mar 2023 00:16:43 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 08 Mar 2023 00:16:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 08 Mar 2023 00:16:43 GMT
WORKDIR /notary/signer
# Mon, 13 Mar 2023 22:40:43 GMT
COPY /notary-signer ./ # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
RUN ./notary-signer --version # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
COPY ./signer-config.json . # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
USER notary
# Mon, 13 Mar 2023 22:40:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 13 Mar 2023 22:40:43 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b05793ac14c68387ad3a34fa8d5d4136f040e8b820b1eee3595d30529d87e46`  
		Last Modified: Wed, 08 Mar 2023 00:17:02 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8867bd3aa695c936397740852a2a23245f7a8147431da0dea7ea79cb52c3fb7`  
		Last Modified: Wed, 08 Mar 2023 00:17:12 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9d6f44471853d748615de79835f860dbaf6a96899425bfe41892a55b8bbc82`  
		Last Modified: Mon, 13 Mar 2023 22:41:10 GMT  
		Size: 4.5 MB (4524257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a29049d4e5f31919a6825670eff28003d1d6a5e8a1a0db07cb80c508d56339`  
		Last Modified: Mon, 13 Mar 2023 22:41:09 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0e82b1ac8c1d3b1d7406e09d51ada3c9d5eef0b16c90412117a62e19a79f64`  
		Last Modified: Mon, 13 Mar 2023 22:41:09 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97710136b3555e60fb404524d8523f81cc0860b525a91fa4bef04700c7b55915`  
		Last Modified: Mon, 13 Mar 2023 22:41:09 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:926e06c706fe49616d9cc65fb3fc800f72c379ac63bb1533ebc92c19b9b5227a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7101769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f95704c1a8b8cf1b5c35f8c60600a55bd4e16456cf1996e14c199d5a3bd1ed`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:01:39 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 02:01:58 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 02:01:58 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 02:01:58 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 02:01:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 02:01:58 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:05:31 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:05:31 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:05:31 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:05:31 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:05:31 GMT
USER notary
# Wed, 08 Mar 2023 00:05:31 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:05:31 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b9e3dceb52b5f1909f74e5761d8b0968630630d4c5d37134133ff1529d57ca`  
		Last Modified: Sat, 11 Feb 2023 02:02:10 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9044747e4fd585aae1a06ddae8513379f85e397343798bc36f0e5504eaa9863f`  
		Last Modified: Sat, 11 Feb 2023 02:02:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37e617a66458e3ef4cc167492040ccc44e181a925937ae2855939d2780abb36`  
		Last Modified: Wed, 08 Mar 2023 00:05:51 GMT  
		Size: 4.4 MB (4390100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7741f3fe119ab783dd0fc9d701e877326371112f6be0f0f217bd515948be20fa`  
		Last Modified: Wed, 08 Mar 2023 00:05:50 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe4596223bf9430c304a6c7dcfad77fd3dc07c3d7f662be26b2989d9d9f6dfe`  
		Last Modified: Wed, 08 Mar 2023 00:05:50 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd11a87326463f869d1ba6c1bca519d2d6d4d5f84dfbe7b5eb36c194c7e614e`  
		Last Modified: Wed, 08 Mar 2023 00:05:50 GMT  
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
$ docker pull notary@sha256:606c37e1d97f4e68ec67ee57439cbcefd35416825bbee5a8438fea16cf305ab1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7102909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d66c8f75871355a84a407a350373d37201ae2aabe85cf2690b4d651da520a1c2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:31:58 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 09:32:48 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 09:32:48 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 09:32:48 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 09:32:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 09:32:48 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:51:17 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
USER notary
# Wed, 08 Mar 2023 00:51:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:51:18 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d271c42b70a8c82b552b2772787a6cac62d60cdc88c599bd983e06b4b1199`  
		Last Modified: Sat, 11 Feb 2023 09:33:10 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11d0b9967527e3e2fe9a387dd1b08ba83b7816d9e3863fb0f3e9c0a13f0225d`  
		Last Modified: Sat, 11 Feb 2023 09:33:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02a9326979cee7618aa2b342258e4cbc31c56b91a4e7e8e89eff264c67e95f6`  
		Last Modified: Wed, 08 Mar 2023 00:51:47 GMT  
		Size: 4.3 MB (4296112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808f46240e2aaa0c8f9fcfd65d773fc98ad9c37bd27eb1aeb70ce112edf1ea7b`  
		Last Modified: Wed, 08 Mar 2023 00:51:46 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfc68a2dc7ed5e20299b9ec5b2c868071a1ab4f3aaee290a0da97297b5d30e3`  
		Last Modified: Wed, 08 Mar 2023 00:51:46 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9b06a55652879187796edbb714b3d74db89083480a9347c81e1573381e9eef`  
		Last Modified: Wed, 08 Mar 2023 00:51:46 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:abfdfe9dbde3305247e776f74ae5d4099b7c5219de959bc45f17b176e6e98dd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7201015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d2c656f5776c347bac9afaa7f72464bdbb3b96dab6e81f650def3f08fe52c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:38:26 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 03:38:57 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 03:38:57 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 03:38:57 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 03:38:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 03:38:57 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:12:03 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:12:03 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:12:04 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:12:04 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:12:04 GMT
USER notary
# Wed, 08 Mar 2023 00:12:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:12:04 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf825008c0747d1db1e6a08e31a5fa2a33c8e0f8a5fe8b2f86af75110c97e790`  
		Last Modified: Sat, 11 Feb 2023 03:39:15 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47b3001bbc3d992bc8bd18f0274d2c096ab38122bfe91ebb713a068610faf80`  
		Last Modified: Sat, 11 Feb 2023 03:39:21 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabbaa0ac8ed6dfd08e91e9308501b5f3fa7aa8d1daf1f4a29f94ed70b293e76`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 4.6 MB (4605262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6168f2066015c6e1d056de0590b9058c7af98779aff58a8fe380fd458a4ed`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b309adaebe295395e40d60e06633c7bf6897b14e3b191a69619b8b19cbe4c03a`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc5983824d5ba6398ee6e275f8ebbc82284ec48ed5f55ab1ebb58db0a9e6177`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
