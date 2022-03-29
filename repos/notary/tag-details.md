<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.6.1-2`](#notaryserver-061-2)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.6.1-2`](#notarysigner-061-2)

## `notary:server`

```console
$ docker pull notary@sha256:6d3ac1c73824c6f230f7ddb1a3578692ab5c15fbe963f5c87d0135ab6a122f4c
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
$ docker pull notary@sha256:9bd51ef6bb1ee2db62e8a09e72dde2280b82da3f118057d375d3c26a55a40f81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8208509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a624db1e5242733176fd0ebd88970b0d8beda8782d90965053c670164c8836ad`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:56:36 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 15:56:36 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 15:56:36 GMT
ENV INSTALLDIR=/notary/server
# Tue, 29 Mar 2022 15:56:36 GMT
EXPOSE 4443
# Tue, 29 Mar 2022 15:56:36 GMT
WORKDIR /notary/server
# Tue, 29 Mar 2022 15:56:51 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 29 Mar 2022 15:56:51 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 29 Mar 2022 15:56:52 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 29 Mar 2022 15:56:52 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 15:56:52 GMT
USER notary
# Tue, 29 Mar 2022 15:56:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 29 Mar 2022 15:56:52 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 15:56:52 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3564071aaeb01bf58ee10751858662e2165537b4f26e7d29e430f1cd114c9`  
		Last Modified: Tue, 29 Mar 2022 15:57:23 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a65146eddf2eca7417db0741ad2ea261a57e7050709a34eb753bb59f762d1f`  
		Last Modified: Tue, 29 Mar 2022 15:57:24 GMT  
		Size: 5.4 MB (5387173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92caab834b0b0ac9babe1eda11876990df36d3b5be408de6ce381c838eaf678a`  
		Last Modified: Tue, 29 Mar 2022 15:57:23 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7412f7a7c38d0b87f36f963b57d54b6915c39bb8a19f1fb57a49ea4c19079a5c`  
		Last Modified: Tue, 29 Mar 2022 15:57:23 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4620befa877f9d257e2a690fab768096cd04bef112cd561e71f32a154728085`  
		Last Modified: Tue, 29 Mar 2022 15:57:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:2aa8b9fcaf349469fc416895ecce25fd4239d240ea66a166fe8e15471eff3dee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a2039268f84d65dfdb2f37aa09a497b5d0bb91de57645a22fcf31dd984ac640`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:33:10 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 08:33:11 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 08:33:11 GMT
ENV INSTALLDIR=/notary/server
# Tue, 29 Mar 2022 08:33:12 GMT
EXPOSE 4443
# Tue, 29 Mar 2022 08:33:13 GMT
WORKDIR /notary/server
# Tue, 29 Mar 2022 08:33:41 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 29 Mar 2022 08:33:42 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 29 Mar 2022 08:33:42 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 29 Mar 2022 08:33:44 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 08:33:44 GMT
USER notary
# Tue, 29 Mar 2022 08:33:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 29 Mar 2022 08:33:45 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 08:33:46 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c1da5275a09ba650590ef2b53111ab5ed521700810f59e40650426112d540`  
		Last Modified: Tue, 29 Mar 2022 08:35:01 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a64a81b635f1085665b19b2228967bdaed77540c85328dd1b9cdcf1498a7406`  
		Last Modified: Tue, 29 Mar 2022 08:35:04 GMT  
		Size: 5.0 MB (5039548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e509047f943b526532a1ae08f949aba3c0d64e0c8906ebb788f0b25194d542`  
		Last Modified: Tue, 29 Mar 2022 08:35:01 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810fb26bbfd4082144aa83c79f575966b6d678e9a5ff9ab400274de091c6f957`  
		Last Modified: Tue, 29 Mar 2022 08:35:01 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbad6c882a79235140b1f2bc5497a678c5bab34851f67ee6415b4c8c76eab73`  
		Last Modified: Tue, 29 Mar 2022 08:35:01 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:f4e6b3233b17be8e85ecfbaf7f4e86ea0821319e697e8df86de86e6aa37e268a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7655419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44e1aaae065874c08d561a4980fd6301750b8fc8ccf034b5fe33ade656f4259`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:06:40 GMT
ENV TAG=v0.6.1
# Sat, 19 Mar 2022 01:06:41 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 19 Mar 2022 01:06:42 GMT
ENV INSTALLDIR=/notary/server
# Sat, 19 Mar 2022 01:06:43 GMT
EXPOSE 4443
# Sat, 19 Mar 2022 01:06:44 GMT
WORKDIR /notary/server
# Sat, 19 Mar 2022 01:06:55 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Sat, 19 Mar 2022 01:06:57 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Sat, 19 Mar 2022 01:06:58 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Sat, 19 Mar 2022 01:06:58 GMT
RUN adduser -D -H -g "" notary
# Sat, 19 Mar 2022 01:06:59 GMT
USER notary
# Sat, 19 Mar 2022 01:07:00 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 19 Mar 2022 01:07:01 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 19 Mar 2022 01:07:02 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df91ebdfbf2846f24d225ac5f917d63636854531e74cc368ec8d1940336b667`  
		Last Modified: Sat, 19 Mar 2022 01:07:46 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbf367055328bdabe93926865382994cc3fb719652bde98f7b19645cfa354e4`  
		Last Modified: Sat, 19 Mar 2022 01:07:47 GMT  
		Size: 4.9 MB (4934196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dfdeacdcaad458ed06182ff25b012ca9fc48c09fac4b5211fc0b8fb5abdf84`  
		Last Modified: Sat, 19 Mar 2022 01:07:46 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f99184962bfb866cd1451e9acb6d5ea4f70d9e6cbc5371f37b48de8d70e7610`  
		Last Modified: Sat, 19 Mar 2022 01:07:46 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f40e5af6cabb51ed6e2a29807efb5d5811b8145a4577753fcf15e0aef54d11`  
		Last Modified: Sat, 19 Mar 2022 01:07:46 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; 386

```console
$ docker pull notary@sha256:0abb8c58f4c8d91e5f4fac97ec822facb7476f92fa45898eb2eb88d4eaac3dae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7921725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf0b959bd6504d6036ef134cf9f0622589175fc630d6f6dd57719689094315b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:45 GMT
ADD file:f1abe5c2930209c2d735059c8e767e630c0818cc18a4fd10b0b90e6efbc675e2 in / 
# Tue, 29 Mar 2022 00:38:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 06:00:06 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 06:00:07 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 06:00:08 GMT
ENV INSTALLDIR=/notary/server
# Tue, 29 Mar 2022 06:00:09 GMT
EXPOSE 4443
# Tue, 29 Mar 2022 06:00:10 GMT
WORKDIR /notary/server
# Tue, 29 Mar 2022 06:00:22 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 29 Mar 2022 06:00:24 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 29 Mar 2022 06:00:25 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 29 Mar 2022 06:00:25 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 06:00:26 GMT
USER notary
# Tue, 29 Mar 2022 06:00:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 29 Mar 2022 06:00:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 06:00:29 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:dadad3128a09e6d507e89afe042cb1d48da14a72b28ca79dec7c6acf971bd9e6`  
		Last Modified: Tue, 29 Mar 2022 00:40:03 GMT  
		Size: 2.8 MB (2820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68fedfba76031367be31f30120970091b48e7dd8605927651a47208b250578f`  
		Last Modified: Tue, 29 Mar 2022 06:01:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e716e1ae372eec12a2303f6765c238dea810dbd3da66cfe1517d25c7f80696`  
		Last Modified: Tue, 29 Mar 2022 06:01:16 GMT  
		Size: 5.1 MB (5099251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7117d326b3b4b50aef490a0d073aedcc6e122163fb049cd54854e8b7e76cdbca`  
		Last Modified: Tue, 29 Mar 2022 06:01:16 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa7ef362ebc2237578f3eb9a91cb42adef5ec7410678439264fb0b685864afd`  
		Last Modified: Tue, 29 Mar 2022 06:01:15 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead48a446c7e7f6403bb6c577709582312af70aea4a4ca15024897ec79b50479`  
		Last Modified: Tue, 29 Mar 2022 06:01:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:985e6f478cb8ee7add51d3e9f8724aa2016c7a7236d579dde3392d7e9b4fded7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7618850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9e09095c5f1886a6deccbc8a54d4f2620bdd705f959addf4e611cafe02d082`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:40:53 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 12:40:54 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 12:40:57 GMT
ENV INSTALLDIR=/notary/server
# Tue, 29 Mar 2022 12:40:59 GMT
EXPOSE 4443
# Tue, 29 Mar 2022 12:41:00 GMT
WORKDIR /notary/server
# Tue, 29 Mar 2022 12:41:25 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 29 Mar 2022 12:41:26 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 29 Mar 2022 12:41:28 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 29 Mar 2022 12:41:39 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 12:41:42 GMT
USER notary
# Tue, 29 Mar 2022 12:41:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 29 Mar 2022 12:41:52 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 12:41:55 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c76495978927a7fe7c2be1d530d9bf734f689e3f34f34219015a15406969ba`  
		Last Modified: Tue, 29 Mar 2022 12:43:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd791a58b44dad9885c1e342e2ee6a6df8a2f56f61511ff5cb0ec82268a0297`  
		Last Modified: Tue, 29 Mar 2022 12:43:41 GMT  
		Size: 4.8 MB (4801885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd7d3843d345b5d6b230182ccf53b7a04638ccf43d3d01555fdc93c6c62a2ab`  
		Last Modified: Tue, 29 Mar 2022 12:43:40 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f6805b22c2a7210c35f9ad1684b9f8bbd7433d568d567fe9e08c504786531e`  
		Last Modified: Tue, 29 Mar 2022 12:43:40 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e1c442fd5e9a9521573101395114edb812d91cd7bcc3ee4cdef7eff1bcdb22`  
		Last Modified: Tue, 29 Mar 2022 12:43:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:9962ef3e77071068235a78fb84412920c4bb8f7eefe93481fa242f1a67400e92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7813164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a37d6d230d60291c2878a060f8a803c876b44fcbd81c1b06d96c1073342fd6b7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:45 GMT
ADD file:08b65c73088f2cc387829e0ce9aa160db404a3e5fa0e4fda048cdbc02d8f64c2 in / 
# Tue, 29 Mar 2022 00:41:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:18:16 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 11:18:16 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 11:18:17 GMT
ENV INSTALLDIR=/notary/server
# Tue, 29 Mar 2022 11:18:17 GMT
EXPOSE 4443
# Tue, 29 Mar 2022 11:18:17 GMT
WORKDIR /notary/server
# Tue, 29 Mar 2022 11:18:28 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 29 Mar 2022 11:18:29 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 29 Mar 2022 11:18:29 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 29 Mar 2022 11:18:29 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 11:18:30 GMT
USER notary
# Tue, 29 Mar 2022 11:18:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 29 Mar 2022 11:18:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 11:18:30 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:89a2ea5c1a3e1d541ae66fbd95d215b39b560c537460c3fc76ad6826582893fe`  
		Last Modified: Tue, 29 Mar 2022 00:47:35 GMT  
		Size: 2.6 MB (2605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2707cf8f836e5cb91bc63dd213fd715cf106987622ffdda1ec2f7dd2879a45b1`  
		Last Modified: Tue, 29 Mar 2022 11:19:41 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3427ae077b2708bf05570a9bc732a0fd2a681fc6bf87ce96addbdb0dd63fde45`  
		Last Modified: Tue, 29 Mar 2022 11:19:41 GMT  
		Size: 5.2 MB (5205968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17d90724c4d5f98449765b472873badaaa8fe6203568f82383fc34a44862a28`  
		Last Modified: Tue, 29 Mar 2022 11:19:37 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b799c4414787f245fccfb8f8794433549e206f3c0909b86460cc071fee9023aa`  
		Last Modified: Tue, 29 Mar 2022 11:19:41 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0319918d9e2797c7be605be95a34bef44f3ddf9c2a38ba99e4c207af10f64`  
		Last Modified: Tue, 29 Mar 2022 11:19:37 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:server-0.6.1-2`

```console
$ docker pull notary@sha256:6d3ac1c73824c6f230f7ddb1a3578692ab5c15fbe963f5c87d0135ab6a122f4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server-0.6.1-2` - linux; amd64

```console
$ docker pull notary@sha256:9bd51ef6bb1ee2db62e8a09e72dde2280b82da3f118057d375d3c26a55a40f81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8208509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a624db1e5242733176fd0ebd88970b0d8beda8782d90965053c670164c8836ad`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:56:36 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 15:56:36 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 15:56:36 GMT
ENV INSTALLDIR=/notary/server
# Tue, 29 Mar 2022 15:56:36 GMT
EXPOSE 4443
# Tue, 29 Mar 2022 15:56:36 GMT
WORKDIR /notary/server
# Tue, 29 Mar 2022 15:56:51 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 29 Mar 2022 15:56:51 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 29 Mar 2022 15:56:52 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 29 Mar 2022 15:56:52 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 15:56:52 GMT
USER notary
# Tue, 29 Mar 2022 15:56:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 29 Mar 2022 15:56:52 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 15:56:52 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3564071aaeb01bf58ee10751858662e2165537b4f26e7d29e430f1cd114c9`  
		Last Modified: Tue, 29 Mar 2022 15:57:23 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a65146eddf2eca7417db0741ad2ea261a57e7050709a34eb753bb59f762d1f`  
		Last Modified: Tue, 29 Mar 2022 15:57:24 GMT  
		Size: 5.4 MB (5387173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92caab834b0b0ac9babe1eda11876990df36d3b5be408de6ce381c838eaf678a`  
		Last Modified: Tue, 29 Mar 2022 15:57:23 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7412f7a7c38d0b87f36f963b57d54b6915c39bb8a19f1fb57a49ea4c19079a5c`  
		Last Modified: Tue, 29 Mar 2022 15:57:23 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4620befa877f9d257e2a690fab768096cd04bef112cd561e71f32a154728085`  
		Last Modified: Tue, 29 Mar 2022 15:57:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.6.1-2` - linux; arm variant v6

```console
$ docker pull notary@sha256:2aa8b9fcaf349469fc416895ecce25fd4239d240ea66a166fe8e15471eff3dee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a2039268f84d65dfdb2f37aa09a497b5d0bb91de57645a22fcf31dd984ac640`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:33:10 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 08:33:11 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 08:33:11 GMT
ENV INSTALLDIR=/notary/server
# Tue, 29 Mar 2022 08:33:12 GMT
EXPOSE 4443
# Tue, 29 Mar 2022 08:33:13 GMT
WORKDIR /notary/server
# Tue, 29 Mar 2022 08:33:41 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 29 Mar 2022 08:33:42 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 29 Mar 2022 08:33:42 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 29 Mar 2022 08:33:44 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 08:33:44 GMT
USER notary
# Tue, 29 Mar 2022 08:33:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 29 Mar 2022 08:33:45 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 08:33:46 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c1da5275a09ba650590ef2b53111ab5ed521700810f59e40650426112d540`  
		Last Modified: Tue, 29 Mar 2022 08:35:01 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a64a81b635f1085665b19b2228967bdaed77540c85328dd1b9cdcf1498a7406`  
		Last Modified: Tue, 29 Mar 2022 08:35:04 GMT  
		Size: 5.0 MB (5039548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e509047f943b526532a1ae08f949aba3c0d64e0c8906ebb788f0b25194d542`  
		Last Modified: Tue, 29 Mar 2022 08:35:01 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810fb26bbfd4082144aa83c79f575966b6d678e9a5ff9ab400274de091c6f957`  
		Last Modified: Tue, 29 Mar 2022 08:35:01 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbad6c882a79235140b1f2bc5497a678c5bab34851f67ee6415b4c8c76eab73`  
		Last Modified: Tue, 29 Mar 2022 08:35:01 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.6.1-2` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:f4e6b3233b17be8e85ecfbaf7f4e86ea0821319e697e8df86de86e6aa37e268a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7655419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44e1aaae065874c08d561a4980fd6301750b8fc8ccf034b5fe33ade656f4259`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:06:40 GMT
ENV TAG=v0.6.1
# Sat, 19 Mar 2022 01:06:41 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 19 Mar 2022 01:06:42 GMT
ENV INSTALLDIR=/notary/server
# Sat, 19 Mar 2022 01:06:43 GMT
EXPOSE 4443
# Sat, 19 Mar 2022 01:06:44 GMT
WORKDIR /notary/server
# Sat, 19 Mar 2022 01:06:55 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Sat, 19 Mar 2022 01:06:57 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Sat, 19 Mar 2022 01:06:58 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Sat, 19 Mar 2022 01:06:58 GMT
RUN adduser -D -H -g "" notary
# Sat, 19 Mar 2022 01:06:59 GMT
USER notary
# Sat, 19 Mar 2022 01:07:00 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 19 Mar 2022 01:07:01 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 19 Mar 2022 01:07:02 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df91ebdfbf2846f24d225ac5f917d63636854531e74cc368ec8d1940336b667`  
		Last Modified: Sat, 19 Mar 2022 01:07:46 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbf367055328bdabe93926865382994cc3fb719652bde98f7b19645cfa354e4`  
		Last Modified: Sat, 19 Mar 2022 01:07:47 GMT  
		Size: 4.9 MB (4934196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dfdeacdcaad458ed06182ff25b012ca9fc48c09fac4b5211fc0b8fb5abdf84`  
		Last Modified: Sat, 19 Mar 2022 01:07:46 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f99184962bfb866cd1451e9acb6d5ea4f70d9e6cbc5371f37b48de8d70e7610`  
		Last Modified: Sat, 19 Mar 2022 01:07:46 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f40e5af6cabb51ed6e2a29807efb5d5811b8145a4577753fcf15e0aef54d11`  
		Last Modified: Sat, 19 Mar 2022 01:07:46 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.6.1-2` - linux; 386

```console
$ docker pull notary@sha256:0abb8c58f4c8d91e5f4fac97ec822facb7476f92fa45898eb2eb88d4eaac3dae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7921725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf0b959bd6504d6036ef134cf9f0622589175fc630d6f6dd57719689094315b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:45 GMT
ADD file:f1abe5c2930209c2d735059c8e767e630c0818cc18a4fd10b0b90e6efbc675e2 in / 
# Tue, 29 Mar 2022 00:38:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 06:00:06 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 06:00:07 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 06:00:08 GMT
ENV INSTALLDIR=/notary/server
# Tue, 29 Mar 2022 06:00:09 GMT
EXPOSE 4443
# Tue, 29 Mar 2022 06:00:10 GMT
WORKDIR /notary/server
# Tue, 29 Mar 2022 06:00:22 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 29 Mar 2022 06:00:24 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 29 Mar 2022 06:00:25 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 29 Mar 2022 06:00:25 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 06:00:26 GMT
USER notary
# Tue, 29 Mar 2022 06:00:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 29 Mar 2022 06:00:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 06:00:29 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:dadad3128a09e6d507e89afe042cb1d48da14a72b28ca79dec7c6acf971bd9e6`  
		Last Modified: Tue, 29 Mar 2022 00:40:03 GMT  
		Size: 2.8 MB (2820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68fedfba76031367be31f30120970091b48e7dd8605927651a47208b250578f`  
		Last Modified: Tue, 29 Mar 2022 06:01:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e716e1ae372eec12a2303f6765c238dea810dbd3da66cfe1517d25c7f80696`  
		Last Modified: Tue, 29 Mar 2022 06:01:16 GMT  
		Size: 5.1 MB (5099251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7117d326b3b4b50aef490a0d073aedcc6e122163fb049cd54854e8b7e76cdbca`  
		Last Modified: Tue, 29 Mar 2022 06:01:16 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa7ef362ebc2237578f3eb9a91cb42adef5ec7410678439264fb0b685864afd`  
		Last Modified: Tue, 29 Mar 2022 06:01:15 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead48a446c7e7f6403bb6c577709582312af70aea4a4ca15024897ec79b50479`  
		Last Modified: Tue, 29 Mar 2022 06:01:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.6.1-2` - linux; ppc64le

```console
$ docker pull notary@sha256:985e6f478cb8ee7add51d3e9f8724aa2016c7a7236d579dde3392d7e9b4fded7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7618850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9e09095c5f1886a6deccbc8a54d4f2620bdd705f959addf4e611cafe02d082`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:40:53 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 12:40:54 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 12:40:57 GMT
ENV INSTALLDIR=/notary/server
# Tue, 29 Mar 2022 12:40:59 GMT
EXPOSE 4443
# Tue, 29 Mar 2022 12:41:00 GMT
WORKDIR /notary/server
# Tue, 29 Mar 2022 12:41:25 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 29 Mar 2022 12:41:26 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 29 Mar 2022 12:41:28 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 29 Mar 2022 12:41:39 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 12:41:42 GMT
USER notary
# Tue, 29 Mar 2022 12:41:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 29 Mar 2022 12:41:52 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 12:41:55 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c76495978927a7fe7c2be1d530d9bf734f689e3f34f34219015a15406969ba`  
		Last Modified: Tue, 29 Mar 2022 12:43:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd791a58b44dad9885c1e342e2ee6a6df8a2f56f61511ff5cb0ec82268a0297`  
		Last Modified: Tue, 29 Mar 2022 12:43:41 GMT  
		Size: 4.8 MB (4801885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd7d3843d345b5d6b230182ccf53b7a04638ccf43d3d01555fdc93c6c62a2ab`  
		Last Modified: Tue, 29 Mar 2022 12:43:40 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f6805b22c2a7210c35f9ad1684b9f8bbd7433d568d567fe9e08c504786531e`  
		Last Modified: Tue, 29 Mar 2022 12:43:40 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e1c442fd5e9a9521573101395114edb812d91cd7bcc3ee4cdef7eff1bcdb22`  
		Last Modified: Tue, 29 Mar 2022 12:43:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.6.1-2` - linux; s390x

```console
$ docker pull notary@sha256:9962ef3e77071068235a78fb84412920c4bb8f7eefe93481fa242f1a67400e92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7813164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a37d6d230d60291c2878a060f8a803c876b44fcbd81c1b06d96c1073342fd6b7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:45 GMT
ADD file:08b65c73088f2cc387829e0ce9aa160db404a3e5fa0e4fda048cdbc02d8f64c2 in / 
# Tue, 29 Mar 2022 00:41:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:18:16 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 11:18:16 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 11:18:17 GMT
ENV INSTALLDIR=/notary/server
# Tue, 29 Mar 2022 11:18:17 GMT
EXPOSE 4443
# Tue, 29 Mar 2022 11:18:17 GMT
WORKDIR /notary/server
# Tue, 29 Mar 2022 11:18:28 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 29 Mar 2022 11:18:29 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 29 Mar 2022 11:18:29 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 29 Mar 2022 11:18:29 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 11:18:30 GMT
USER notary
# Tue, 29 Mar 2022 11:18:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 29 Mar 2022 11:18:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 11:18:30 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:89a2ea5c1a3e1d541ae66fbd95d215b39b560c537460c3fc76ad6826582893fe`  
		Last Modified: Tue, 29 Mar 2022 00:47:35 GMT  
		Size: 2.6 MB (2605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2707cf8f836e5cb91bc63dd213fd715cf106987622ffdda1ec2f7dd2879a45b1`  
		Last Modified: Tue, 29 Mar 2022 11:19:41 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3427ae077b2708bf05570a9bc732a0fd2a681fc6bf87ce96addbdb0dd63fde45`  
		Last Modified: Tue, 29 Mar 2022 11:19:41 GMT  
		Size: 5.2 MB (5205968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17d90724c4d5f98449765b472873badaaa8fe6203568f82383fc34a44862a28`  
		Last Modified: Tue, 29 Mar 2022 11:19:37 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b799c4414787f245fccfb8f8794433549e206f3c0909b86460cc071fee9023aa`  
		Last Modified: Tue, 29 Mar 2022 11:19:41 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0319918d9e2797c7be605be95a34bef44f3ddf9c2a38ba99e4c207af10f64`  
		Last Modified: Tue, 29 Mar 2022 11:19:37 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer`

```console
$ docker pull notary@sha256:59a13eb12fdbb10830b7058fcb3e83e668ec9cf26c2404f974d3cc30faff9b82
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
$ docker pull notary@sha256:5a597b68b254bf6117fbb7b0985cb52a0c0e86d17f91a3e2f68b82a5e60ed6c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7690874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a1b0c0a51a29722cfcf864a2d028631e0853919ca0fc059237081377ad639a0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:56:36 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 15:56:36 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 15:56:55 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 15:56:56 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 15:56:56 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 15:56:56 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 15:57:10 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 15:57:10 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 15:57:10 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 15:57:11 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 15:57:11 GMT
USER notary
# Tue, 29 Mar 2022 15:57:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 15:57:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 15:57:11 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb1082d1643807ceaeb8e590f3432e78d20f6f87149b4b38ea6990bce6a906f`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b54f98c8f2aaa0488352c699dc96fbe5687447f43efe4f1e38e3bbc65fd3f4b`  
		Last Modified: Tue, 29 Mar 2022 15:57:34 GMT  
		Size: 4.9 MB (4869596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc364a837c60fc420eaa9f49d15469346627cbed5c2a05c01288d87976ee4233`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a7dffcbe64d230591ae8b8763c1ab40e881c5a3d02554bcd52c3e8a6fedf63`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7005a3d5fd6b1e09b7b2ef641c2e305005d980afab194064bf4f42963325eb04`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:e43398af5a51dc91344e33abe8cc1b68c5877cd257a122abb30dc1385d78bd82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7182318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b32666262b52eb80dee7cf63f70dc6ad985b2ca0504e03407b78717525355f4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:33:10 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 08:33:11 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 08:34:00 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 08:34:01 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 08:34:01 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 08:34:01 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 08:34:25 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 08:34:26 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 08:34:26 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 08:34:28 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 08:34:28 GMT
USER notary
# Tue, 29 Mar 2022 08:34:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 08:34:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 08:34:30 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b26d26abde63c15b13e6af115c7c6fb9fc2d22d642357f055785de91cb6483`  
		Last Modified: Tue, 29 Mar 2022 08:35:16 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c91bc37bc68a86160c7f6ab4b50a14877de14d73ea8610a6f44e63e7abb6669`  
		Last Modified: Tue, 29 Mar 2022 08:35:19 GMT  
		Size: 4.6 MB (4555116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4902016b7476344058a8d7a4bba669b89b6270d157c495fbe967027f2de91d9c`  
		Last Modified: Tue, 29 Mar 2022 08:35:15 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650c019ee1d8315a41d3aa9680e78efd657ec14b10b7de7ad84d2140ab8c539a`  
		Last Modified: Tue, 29 Mar 2022 08:35:16 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607eba904a7eb637730de293342b19501b3bb9a8af2563aa3cc3e7fb089ac7c`  
		Last Modified: Tue, 29 Mar 2022 08:35:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:7a186215872f1c3801ca640e32df5bef70f3d4dda626b07f8d1c4578ec127daa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7176931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d3cefe647af844bbe0906f558647bb943d54c43ffa98ab5367b4bfb557d8c69`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:06:40 GMT
ENV TAG=v0.6.1
# Sat, 19 Mar 2022 01:06:41 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 19 Mar 2022 01:07:07 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 19 Mar 2022 01:07:08 GMT
EXPOSE 4444
# Sat, 19 Mar 2022 01:07:09 GMT
EXPOSE 7899
# Sat, 19 Mar 2022 01:07:10 GMT
WORKDIR /notary/signer
# Sat, 19 Mar 2022 01:07:20 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 19 Mar 2022 01:07:22 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 19 Mar 2022 01:07:23 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 19 Mar 2022 01:07:23 GMT
RUN adduser -D -H -g "" notary
# Sat, 19 Mar 2022 01:07:24 GMT
USER notary
# Sat, 19 Mar 2022 01:07:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 19 Mar 2022 01:07:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 19 Mar 2022 01:07:27 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31637a795a9f059af1f95be8849f6be791dde68237d7c86c01454dd572b52a`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6255a8d20621a4455617d12053f107406d4975d78567f8c39b3da448abfb2bb8`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 4.5 MB (4455766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0160fc393462056b86027a87648ed7fea282ec77af91cef287afb242f901e311`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279ee1fa1db3cede4134d5e6f895becf8d3a8fc735510014fc1a38333270ac29`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030e2bf09c2d22c09c9c233270e2b5ddd5c4ef8df32d41a0c7ec854801f21ec1`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:d1e41ca16127354a473ab50ecfe3dbb2218900e7bba3d58ad7848907e8b04b44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7435786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b279ce042847ab5e2613ba443ddfadec0be78dc452c1685075cbb0f95c94cf5e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:45 GMT
ADD file:f1abe5c2930209c2d735059c8e767e630c0818cc18a4fd10b0b90e6efbc675e2 in / 
# Tue, 29 Mar 2022 00:38:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 06:00:06 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 06:00:07 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 06:00:37 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 06:00:38 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 06:00:39 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 06:00:40 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 06:00:51 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 06:00:53 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 06:00:54 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 06:00:54 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 06:00:55 GMT
USER notary
# Tue, 29 Mar 2022 06:00:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 06:00:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 06:00:58 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:dadad3128a09e6d507e89afe042cb1d48da14a72b28ca79dec7c6acf971bd9e6`  
		Last Modified: Tue, 29 Mar 2022 00:40:03 GMT  
		Size: 2.8 MB (2820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007901d388885795e87bab30fa93738b38540997491c7aa9d5394e7dff978b44`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4523fcd851d986eca1f25991fe3c80057aed1c4903505b2483a87641d32d7343`  
		Last Modified: Tue, 29 Mar 2022 06:01:34 GMT  
		Size: 4.6 MB (4613377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6d2f8bbfc6dcd19caf60def2df525745794e7a9333ca5d643ad3d725dd7a0b`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36549517e1365949e5f08a32766861b7173556953c36fe39bf205238d2222057`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0245f15cec6fc67c4540204f8a118c234d2dd595864055da21543eb145d79d7e`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:28d32bbc4575f6f5b205f3c8d731c9c7fe4f5d18539add28757e9da27d57e65c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7154680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1b5007de5cc8d26eacefb2bbd7fc47b0d52ad52826d8183409a33bc26f9aec`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:40:53 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 12:40:54 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 12:42:06 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 12:42:09 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 12:42:12 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 12:42:15 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 12:42:39 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 12:42:40 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 12:42:42 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 12:42:50 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 12:42:59 GMT
USER notary
# Tue, 29 Mar 2022 12:43:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 12:43:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 12:43:13 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacff4a4ed250261b3768bbfc9708d3da1b5331717d25f86c4c0928e2609079`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222b02a3c69a5071e2847e33f670374acb913d4475da9ba50a6783ba1d451b25`  
		Last Modified: Tue, 29 Mar 2022 12:43:54 GMT  
		Size: 4.3 MB (4337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295ab1754665b939a567857c6fbcf38d773ba83562ac53546e1e3246c54cd41a`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542bb77cdd69cc247f93a9cdef415bbd42df299d501c84c773cb89c00c8d133c`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7634254911f718d0571952c1c88cdbcf08b66ce4a7266e150a10dda53d468bed`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:4297e4e5302259953bbfd0747d42575db953ab665fcaf1a6b76c6a0fc9f9ffe3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7313790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17bf63d014899545474153c839259f8d7003c462d6119e39f30bcf88bc7105b9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:45 GMT
ADD file:08b65c73088f2cc387829e0ce9aa160db404a3e5fa0e4fda048cdbc02d8f64c2 in / 
# Tue, 29 Mar 2022 00:41:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:18:16 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 11:18:16 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 11:18:38 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 11:18:38 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 11:18:38 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 11:18:38 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 11:18:53 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 11:18:54 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 11:18:54 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 11:18:54 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 11:18:54 GMT
USER notary
# Tue, 29 Mar 2022 11:18:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 11:18:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 11:18:55 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:89a2ea5c1a3e1d541ae66fbd95d215b39b560c537460c3fc76ad6826582893fe`  
		Last Modified: Tue, 29 Mar 2022 00:47:35 GMT  
		Size: 2.6 MB (2605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ac5d8b5943f179b16c64910bc48fd499aa21c41988b7624c0dc68d00722ae6`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdafac6ccb7a2b11c2a1af545276b22159c24598c08634bc09222e69d5c613`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 4.7 MB (4706660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3a581a27946ea536cc943d404787a0689ce4cf258d70b8b332f6395775953b`  
		Last Modified: Tue, 29 Mar 2022 11:21:15 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318594e20762541b71ff092618a6ee9c9ff373980c82bc3b65e5adaff577df54`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b195fb8bc296e2295a27228fe70d834c0317902f1d723e80b5fe606ad4d950b`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer-0.6.1-2`

```console
$ docker pull notary@sha256:59a13eb12fdbb10830b7058fcb3e83e668ec9cf26c2404f974d3cc30faff9b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer-0.6.1-2` - linux; amd64

```console
$ docker pull notary@sha256:5a597b68b254bf6117fbb7b0985cb52a0c0e86d17f91a3e2f68b82a5e60ed6c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7690874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a1b0c0a51a29722cfcf864a2d028631e0853919ca0fc059237081377ad639a0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:56:36 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 15:56:36 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 15:56:55 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 15:56:56 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 15:56:56 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 15:56:56 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 15:57:10 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 15:57:10 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 15:57:10 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 15:57:11 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 15:57:11 GMT
USER notary
# Tue, 29 Mar 2022 15:57:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 15:57:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 15:57:11 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb1082d1643807ceaeb8e590f3432e78d20f6f87149b4b38ea6990bce6a906f`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b54f98c8f2aaa0488352c699dc96fbe5687447f43efe4f1e38e3bbc65fd3f4b`  
		Last Modified: Tue, 29 Mar 2022 15:57:34 GMT  
		Size: 4.9 MB (4869596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc364a837c60fc420eaa9f49d15469346627cbed5c2a05c01288d87976ee4233`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a7dffcbe64d230591ae8b8763c1ab40e881c5a3d02554bcd52c3e8a6fedf63`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7005a3d5fd6b1e09b7b2ef641c2e305005d980afab194064bf4f42963325eb04`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; arm variant v6

```console
$ docker pull notary@sha256:e43398af5a51dc91344e33abe8cc1b68c5877cd257a122abb30dc1385d78bd82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7182318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b32666262b52eb80dee7cf63f70dc6ad985b2ca0504e03407b78717525355f4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:33:10 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 08:33:11 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 08:34:00 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 08:34:01 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 08:34:01 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 08:34:01 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 08:34:25 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 08:34:26 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 08:34:26 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 08:34:28 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 08:34:28 GMT
USER notary
# Tue, 29 Mar 2022 08:34:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 08:34:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 08:34:30 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b26d26abde63c15b13e6af115c7c6fb9fc2d22d642357f055785de91cb6483`  
		Last Modified: Tue, 29 Mar 2022 08:35:16 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c91bc37bc68a86160c7f6ab4b50a14877de14d73ea8610a6f44e63e7abb6669`  
		Last Modified: Tue, 29 Mar 2022 08:35:19 GMT  
		Size: 4.6 MB (4555116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4902016b7476344058a8d7a4bba669b89b6270d157c495fbe967027f2de91d9c`  
		Last Modified: Tue, 29 Mar 2022 08:35:15 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650c019ee1d8315a41d3aa9680e78efd657ec14b10b7de7ad84d2140ab8c539a`  
		Last Modified: Tue, 29 Mar 2022 08:35:16 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607eba904a7eb637730de293342b19501b3bb9a8af2563aa3cc3e7fb089ac7c`  
		Last Modified: Tue, 29 Mar 2022 08:35:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:7a186215872f1c3801ca640e32df5bef70f3d4dda626b07f8d1c4578ec127daa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7176931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d3cefe647af844bbe0906f558647bb943d54c43ffa98ab5367b4bfb557d8c69`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:06:40 GMT
ENV TAG=v0.6.1
# Sat, 19 Mar 2022 01:06:41 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 19 Mar 2022 01:07:07 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 19 Mar 2022 01:07:08 GMT
EXPOSE 4444
# Sat, 19 Mar 2022 01:07:09 GMT
EXPOSE 7899
# Sat, 19 Mar 2022 01:07:10 GMT
WORKDIR /notary/signer
# Sat, 19 Mar 2022 01:07:20 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 19 Mar 2022 01:07:22 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 19 Mar 2022 01:07:23 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 19 Mar 2022 01:07:23 GMT
RUN adduser -D -H -g "" notary
# Sat, 19 Mar 2022 01:07:24 GMT
USER notary
# Sat, 19 Mar 2022 01:07:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 19 Mar 2022 01:07:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 19 Mar 2022 01:07:27 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31637a795a9f059af1f95be8849f6be791dde68237d7c86c01454dd572b52a`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6255a8d20621a4455617d12053f107406d4975d78567f8c39b3da448abfb2bb8`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 4.5 MB (4455766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0160fc393462056b86027a87648ed7fea282ec77af91cef287afb242f901e311`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279ee1fa1db3cede4134d5e6f895becf8d3a8fc735510014fc1a38333270ac29`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030e2bf09c2d22c09c9c233270e2b5ddd5c4ef8df32d41a0c7ec854801f21ec1`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; 386

```console
$ docker pull notary@sha256:d1e41ca16127354a473ab50ecfe3dbb2218900e7bba3d58ad7848907e8b04b44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7435786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b279ce042847ab5e2613ba443ddfadec0be78dc452c1685075cbb0f95c94cf5e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:45 GMT
ADD file:f1abe5c2930209c2d735059c8e767e630c0818cc18a4fd10b0b90e6efbc675e2 in / 
# Tue, 29 Mar 2022 00:38:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 06:00:06 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 06:00:07 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 06:00:37 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 06:00:38 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 06:00:39 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 06:00:40 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 06:00:51 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 06:00:53 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 06:00:54 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 06:00:54 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 06:00:55 GMT
USER notary
# Tue, 29 Mar 2022 06:00:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 06:00:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 06:00:58 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:dadad3128a09e6d507e89afe042cb1d48da14a72b28ca79dec7c6acf971bd9e6`  
		Last Modified: Tue, 29 Mar 2022 00:40:03 GMT  
		Size: 2.8 MB (2820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007901d388885795e87bab30fa93738b38540997491c7aa9d5394e7dff978b44`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4523fcd851d986eca1f25991fe3c80057aed1c4903505b2483a87641d32d7343`  
		Last Modified: Tue, 29 Mar 2022 06:01:34 GMT  
		Size: 4.6 MB (4613377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6d2f8bbfc6dcd19caf60def2df525745794e7a9333ca5d643ad3d725dd7a0b`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36549517e1365949e5f08a32766861b7173556953c36fe39bf205238d2222057`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0245f15cec6fc67c4540204f8a118c234d2dd595864055da21543eb145d79d7e`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; ppc64le

```console
$ docker pull notary@sha256:28d32bbc4575f6f5b205f3c8d731c9c7fe4f5d18539add28757e9da27d57e65c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7154680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1b5007de5cc8d26eacefb2bbd7fc47b0d52ad52826d8183409a33bc26f9aec`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:40:53 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 12:40:54 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 12:42:06 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 12:42:09 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 12:42:12 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 12:42:15 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 12:42:39 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 12:42:40 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 12:42:42 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 12:42:50 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 12:42:59 GMT
USER notary
# Tue, 29 Mar 2022 12:43:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 12:43:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 12:43:13 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacff4a4ed250261b3768bbfc9708d3da1b5331717d25f86c4c0928e2609079`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222b02a3c69a5071e2847e33f670374acb913d4475da9ba50a6783ba1d451b25`  
		Last Modified: Tue, 29 Mar 2022 12:43:54 GMT  
		Size: 4.3 MB (4337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295ab1754665b939a567857c6fbcf38d773ba83562ac53546e1e3246c54cd41a`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542bb77cdd69cc247f93a9cdef415bbd42df299d501c84c773cb89c00c8d133c`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7634254911f718d0571952c1c88cdbcf08b66ce4a7266e150a10dda53d468bed`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; s390x

```console
$ docker pull notary@sha256:4297e4e5302259953bbfd0747d42575db953ab665fcaf1a6b76c6a0fc9f9ffe3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7313790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17bf63d014899545474153c839259f8d7003c462d6119e39f30bcf88bc7105b9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:45 GMT
ADD file:08b65c73088f2cc387829e0ce9aa160db404a3e5fa0e4fda048cdbc02d8f64c2 in / 
# Tue, 29 Mar 2022 00:41:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:18:16 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 11:18:16 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 11:18:38 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 11:18:38 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 11:18:38 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 11:18:38 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 11:18:53 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 11:18:54 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 11:18:54 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 11:18:54 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 11:18:54 GMT
USER notary
# Tue, 29 Mar 2022 11:18:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 11:18:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 11:18:55 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:89a2ea5c1a3e1d541ae66fbd95d215b39b560c537460c3fc76ad6826582893fe`  
		Last Modified: Tue, 29 Mar 2022 00:47:35 GMT  
		Size: 2.6 MB (2605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ac5d8b5943f179b16c64910bc48fd499aa21c41988b7624c0dc68d00722ae6`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdafac6ccb7a2b11c2a1af545276b22159c24598c08634bc09222e69d5c613`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 4.7 MB (4706660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3a581a27946ea536cc943d404787a0689ce4cf258d70b8b332f6395775953b`  
		Last Modified: Tue, 29 Mar 2022 11:21:15 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318594e20762541b71ff092618a6ee9c9ff373980c82bc3b65e5adaff577df54`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b195fb8bc296e2295a27228fe70d834c0317902f1d723e80b5fe606ad4d950b`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
