<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.18`](#kibana6818)
-	[`kibana:7.14.0`](#kibana7140)

## `kibana:6.8.18`

```console
$ docker pull kibana@sha256:3ff64280e63934cc206a2de232104ed629ddb719f2540e3a451d76e3dd4a8a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kibana:6.8.18` - linux; amd64

```console
$ docker pull kibana@sha256:70bd0fd66592567793d9a25776b881a009d071036d0e88a161ba0fd33f493058
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.4 MB (314378155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2728cb7ee745241970ac8d99d09c8df96468eb75b0378e99ddb94dcaff80298d`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Wed, 28 Jul 2021 16:54:15 GMT
EXPOSE 5601
# Wed, 28 Jul 2021 16:54:55 GMT
RUN yum update -y && yum install -y fontconfig freetype && yum clean all
# Wed, 28 Jul 2021 16:55:16 GMT
COPY --chown=1000:0dir:ef39be03f4f1585353627cfac56e45cbbb94ee2836384f5689d1b93b32744d97 in /usr/share/kibana 
# Wed, 28 Jul 2021 16:55:18 GMT
WORKDIR /usr/share/kibana
# Wed, 28 Jul 2021 16:55:19 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Wed, 28 Jul 2021 16:55:19 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 28 Jul 2021 16:55:19 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Jul 2021 16:55:20 GMT
COPY --chown=1000:0file:60b6181f28c99b362092ea6139b6d4112ddd0bef32d52563c33b26bdc2b51318 in /usr/share/kibana/config/kibana.yml 
# Wed, 28 Jul 2021 16:55:20 GMT
COPY --chown=1000:0file:7d472d1939e23e2f10e7c5fd1e9166eefd646214aa0d8a1c09d92af71c9cbd87 in /usr/local/bin/ 
# Wed, 28 Jul 2021 16:55:21 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Wed, 28 Jul 2021 16:55:22 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Wed, 28 Jul 2021 16:55:23 GMT
USER kibana
# Wed, 28 Jul 2021 16:55:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=6.8.18 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License license=Elastic License
# Wed, 28 Jul 2021 16:55:23 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd00bb9b2623a286789eea25eb4c5f4b35ece70dfa534db3b97bdaf7a5b538e`  
		Last Modified: Tue, 03 Aug 2021 13:37:28 GMT  
		Size: 51.1 MB (51079252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90d8ff1432a6e38dc7e67371e45e251c88186f2aa052b89a1724ecb744ebe5e`  
		Last Modified: Tue, 03 Aug 2021 13:37:45 GMT  
		Size: 187.2 MB (187196991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4b33bf7081374a75998bde48b53b070a2ec593f528555f46967157baf30f43`  
		Last Modified: Tue, 03 Aug 2021 13:37:19 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a96f8e923c2fcec0dd06f9b2ace15c8a7b98fe62efe93a0a68b82e54bb598c7`  
		Last Modified: Tue, 03 Aug 2021 13:37:16 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36d235a608239b33e1e0a8f2020fe2eb4ec91b91c66498f3f5644733907f1fc`  
		Last Modified: Tue, 03 Aug 2021 13:37:16 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd5c1bbb9986018d0928e09d110c23f4f823ca96d427a78e8658e9c7729ab07`  
		Last Modified: Tue, 03 Aug 2021 13:37:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd64dedd5083b44389ce0521ec9459e1aa560bc91c9701cbcf2a9dc834968ff6`  
		Last Modified: Tue, 03 Aug 2021 13:37:13 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:7.14.0`

```console
$ docker pull kibana@sha256:7188839aee88057c1f92aaff12d6ca4f54f5f89c1a07caedbc0247c4ec041392
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.14.0` - linux; amd64

```console
$ docker pull kibana@sha256:a1c80a2b22f6c9a93a089c8b983078d482e6dad5e693c64e84b491afd0e90f53
```

-	Docker Version: 20.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515774654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58dffcbc8caa43c7bb0084fb51b29706bc0dca39405b39b67f4923988b11c527`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Thu, 29 Jul 2021 20:35:56 GMT
EXPOSE 5601
# Thu, 29 Jul 2021 20:36:42 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y         fontconfig freetype shadow-utils nss  &&       yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Thu, 29 Jul 2021 20:36:44 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Thu, 29 Jul 2021 20:36:45 GMT
RUN mkdir /usr/share/fonts/local
# Thu, 29 Jul 2021 20:36:47 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Thu, 29 Jul 2021 20:36:48 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Thu, 29 Jul 2021 20:36:48 GMT
RUN fc-cache -v
# Thu, 29 Jul 2021 20:37:18 GMT
COPY --chown=1000:0dir:197f570bc0584eb7ce56539827b52fc3d20f49ced3c8807f4c24a63ee3d51d42 in /usr/share/kibana 
# Thu, 29 Jul 2021 20:37:26 GMT
WORKDIR /usr/share/kibana
# Thu, 29 Jul 2021 20:37:26 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 29 Jul 2021 20:37:26 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 29 Jul 2021 20:37:26 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Jul 2021 20:37:27 GMT
COPY --chown=1000:0file:ab38106de0b2164e20c73bb3449b4682fb9c654eac5b38ed7f560f16ed9c9105 in /usr/share/kibana/config/kibana.yml 
# Thu, 29 Jul 2021 20:37:27 GMT
COPY --chown=1000:0file:a971e8b1ef047eb3eecd6a3776ff0fa8a4e252d1c434e2fe5e7b840af024d381 in /usr/local/bin/ 
# Thu, 29 Jul 2021 20:37:28 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 29 Jul 2021 20:37:30 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Thu, 29 Jul 2021 20:37:31 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Thu, 29 Jul 2021 20:37:31 GMT
LABEL org.label-schema.build-date=2021-07-29T19:46:48.986Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=f032cf9bdbf6f74b70db5e43b7b1d30f5de22d3e org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.14.0 org.opencontainers.image.created=2021-07-29T19:46:48.986Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=f032cf9bdbf6f74b70db5e43b7b1d30f5de22d3e org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.14.0
# Thu, 29 Jul 2021 20:37:31 GMT
USER kibana
# Thu, 29 Jul 2021 20:37:31 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 29 Jul 2021 20:37:31 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92a27ccb611c62150826ba4f0c573264565ed97db3e3758a01a0f8743a011ef`  
		Last Modified: Tue, 03 Aug 2021 13:53:30 GMT  
		Size: 97.1 MB (97122433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7ecfbf36a1490e8040c49c94f79c0cf20ec9b820f5d360a1f4bfa770dfa24b`  
		Last Modified: Tue, 03 Aug 2021 13:53:00 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9081d817c445d8e1c334967101a6fe414db34302f98dffb0e7867485bef87c`  
		Last Modified: Tue, 03 Aug 2021 13:53:00 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530cdbe89f1c3b0741642707c222d7934aad819023b426b753421f699b072f5`  
		Last Modified: Tue, 03 Aug 2021 13:53:02 GMT  
		Size: 16.5 MB (16460486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccffe653ddc0bf9fdfa2778abfbc112e0b085cfa8c86ba58ccb7a28c1eda336b`  
		Last Modified: Tue, 03 Aug 2021 13:52:59 GMT  
		Size: 8.3 KB (8263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af29ddcbaa8e9b14e0daa998b930c9c63a8a07464b1742ff38db2b6c4bd95c7f`  
		Last Modified: Tue, 03 Aug 2021 13:54:06 GMT  
		Size: 326.8 MB (326787785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4704d6a2703eb552bb9a26b2cac66e3a54dab672d1539e469fbfde3d66e3f2`  
		Last Modified: Tue, 03 Aug 2021 13:52:57 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458a467a065159283f41f8f255ba968306a661223804bbbd4cbc9a448b721969`  
		Last Modified: Tue, 03 Aug 2021 13:52:57 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcc78271e5af8beb5ed488c4990b0d7009bd61cfbb0bf28fba0a036916f80a7`  
		Last Modified: Tue, 03 Aug 2021 13:52:57 GMT  
		Size: 4.4 KB (4438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86420aa7083abf67a9ae366bbb11e82727059b36908f95d71a6d1ac6c05878b`  
		Last Modified: Tue, 03 Aug 2021 13:52:57 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e6996042202b336b84d10cd6a52c856433904f49013518a8283471d5a47bb1`  
		Last Modified: Tue, 03 Aug 2021 13:52:55 GMT  
		Size: 196.7 KB (196722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c69cf1db76f9373a0ba5c3b35bafaa264ae7194a12f835afcfc8d9a0a4f02`  
		Last Modified: Tue, 03 Aug 2021 13:52:55 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.14.0` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:4826c5665c879272cb0fedb4e654d45dc16666b4f8df9c0850c511166acfb342
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.6 MB (530577104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c52b5264c4b55c1f459f3ffb224ffaa63f700b052bcd8cef0edb9a2677621c4`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Mon, 07 Dec 2020 23:42:06 GMT
ADD file:edd6e1253ec7bbb67b5a28d40c7d28b34a443c2cfa327bebf55c8b0b19484bf9 in / 
# Mon, 07 Dec 2020 23:42:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Mon, 07 Dec 2020 23:42:10 GMT
CMD ["/bin/bash"]
# Thu, 29 Jul 2021 22:01:40 GMT
EXPOSE 5601
# Thu, 29 Jul 2021 22:02:36 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y         fontconfig freetype shadow-utils nss  &&       yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Thu, 29 Jul 2021 22:02:39 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Thu, 29 Jul 2021 22:02:39 GMT
RUN mkdir /usr/share/fonts/local
# Thu, 29 Jul 2021 22:02:41 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Thu, 29 Jul 2021 22:02:42 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Thu, 29 Jul 2021 22:02:42 GMT
RUN fc-cache -v
# Thu, 29 Jul 2021 22:03:52 GMT
COPY --chown=1000:0dir:2c25d540577fdeca03468b54deec298740a3c4e5c7f02e9faac5853c5f6b77de in /usr/share/kibana 
# Thu, 29 Jul 2021 22:03:54 GMT
WORKDIR /usr/share/kibana
# Thu, 29 Jul 2021 22:03:55 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 29 Jul 2021 22:03:55 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 29 Jul 2021 22:03:55 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Jul 2021 22:03:55 GMT
COPY --chown=1000:0file:ab38106de0b2164e20c73bb3449b4682fb9c654eac5b38ed7f560f16ed9c9105 in /usr/share/kibana/config/kibana.yml 
# Thu, 29 Jul 2021 22:03:55 GMT
COPY --chown=1000:0file:a971e8b1ef047eb3eecd6a3776ff0fa8a4e252d1c434e2fe5e7b840af024d381 in /usr/local/bin/ 
# Thu, 29 Jul 2021 22:03:57 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 29 Jul 2021 22:03:59 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Thu, 29 Jul 2021 22:04:00 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Thu, 29 Jul 2021 22:04:00 GMT
LABEL org.label-schema.build-date=2021-07-29T21:58:22.398Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=f032cf9bdbf6f74b70db5e43b7b1d30f5de22d3e org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.14.0 org.opencontainers.image.created=2021-07-29T21:58:22.398Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=f032cf9bdbf6f74b70db5e43b7b1d30f5de22d3e org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.14.0
# Thu, 29 Jul 2021 22:04:00 GMT
USER kibana
# Thu, 29 Jul 2021 22:04:00 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 29 Jul 2021 22:04:00 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:333cbcae3fb80b9a46084ae4caea81a84aafda9700fb646ab89206d0cfe213fd`  
		Last Modified: Mon, 07 Dec 2020 23:42:49 GMT  
		Size: 75.6 MB (75613064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a66da3dc0ecd01b49f35fa9b382d907be4ee8b1c3165c61c640f39a6947fefb`  
		Last Modified: Wed, 04 Aug 2021 00:00:57 GMT  
		Size: 97.1 MB (97109651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d20fc6d9baa1b62724e76ade735eeb6794d4f65a1962fdf1b7350896a383a27`  
		Last Modified: Wed, 04 Aug 2021 00:00:41 GMT  
		Size: 9.1 KB (9102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb0aea6f151a68b267530d40a2dba462a3b18561c99216cb745eaee7f04cef`  
		Last Modified: Wed, 04 Aug 2021 00:00:39 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfcc3233374b38443ef951639099ded2c3a85dc539e061b70a73e9e8f0b359f`  
		Last Modified: Wed, 04 Aug 2021 00:00:40 GMT  
		Size: 16.5 MB (16460495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8264e0762143ad37b6af21fc820c5a96913f972c281df3c0d886fb9bbfde5edc`  
		Last Modified: Wed, 04 Aug 2021 00:00:38 GMT  
		Size: 8.3 KB (8313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54879e69654e0920c587227d7831214a1621a183ba0ca2c26af9ebd9aa9e53f7`  
		Last Modified: Wed, 04 Aug 2021 00:01:23 GMT  
		Size: 341.2 MB (341171634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048858ab67fac2961bce569a2c8e893cc114cb75cfb7c3061a5a6864124309df`  
		Last Modified: Wed, 04 Aug 2021 00:00:38 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c899a84be8c512cacea253652261dc6ae6aef05b0ef1e5c983540862913ec3`  
		Last Modified: Wed, 04 Aug 2021 00:00:35 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a2f15de0f20a3f361d59b94e1523d2c406f6b86ceb949dcd5420c6e409c408`  
		Last Modified: Wed, 04 Aug 2021 00:00:35 GMT  
		Size: 4.4 KB (4441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949c578e744811f0d999138b9702af6fc26a3457358043467ae72a5f040e63d2`  
		Last Modified: Wed, 04 Aug 2021 00:00:35 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35f406ea13c8a63255288a170576bbafb813a1b9b4a3abc4dafe4a787683a96`  
		Last Modified: Wed, 04 Aug 2021 00:00:35 GMT  
		Size: 197.4 KB (197404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e29e73ca5f49ff0ee5d4ace086b3e15d3d504b7592c1e947e16de06e885df0`  
		Last Modified: Wed, 04 Aug 2021 00:00:36 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
