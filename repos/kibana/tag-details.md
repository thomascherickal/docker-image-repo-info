<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.14`](#kibana6814)
-	[`kibana:7.11.1`](#kibana7111)

## `kibana:6.8.14`

```console
$ docker pull kibana@sha256:e983bb7be0f854f28f1772baa779e89adf9151e96c84bd74b258f218ebc6680d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kibana:6.8.14` - linux; amd64

```console
$ docker pull kibana@sha256:a3805636548a099bacf8fad2da72bb45f459da3d51d1901ba2eeccd2c141da5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.8 MB (301765463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fea356f9e252a3f4d968fa0c58ee7ba015d5a25d623797f9e97fb2df4a7a8977`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Tue, 02 Feb 2021 20:46:47 GMT
EXPOSE 5601
# Tue, 02 Feb 2021 20:47:24 GMT
RUN yum update -y && yum install -y fontconfig freetype && yum clean all
# Tue, 02 Feb 2021 20:48:09 GMT
COPY --chown=1000:0dir:5e9b6a376d2e38bdc096184fcbafab033d15dfd967dc2398dc7d76018aca6087 in /usr/share/kibana 
# Tue, 02 Feb 2021 20:48:11 GMT
WORKDIR /usr/share/kibana
# Tue, 02 Feb 2021 20:48:13 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Tue, 02 Feb 2021 20:48:13 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 02 Feb 2021 20:48:13 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Feb 2021 20:48:14 GMT
COPY --chown=1000:0file:60b6181f28c99b362092ea6139b6d4112ddd0bef32d52563c33b26bdc2b51318 in /usr/share/kibana/config/kibana.yml 
# Tue, 02 Feb 2021 20:48:15 GMT
COPY --chown=1000:0file:7d472d1939e23e2f10e7c5fd1e9166eefd646214aa0d8a1c09d92af71c9cbd87 in /usr/local/bin/ 
# Tue, 02 Feb 2021 20:48:20 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Tue, 02 Feb 2021 20:48:21 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Tue, 02 Feb 2021 20:48:21 GMT
USER kibana
# Tue, 02 Feb 2021 20:48:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=6.8.14 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License license=Elastic License
# Tue, 02 Feb 2021 20:48:21 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78434e1118c09074188e6df5d4b8f3ef66ece0c65e5b8410ab7968854c75929`  
		Last Modified: Wed, 10 Feb 2021 15:38:53 GMT  
		Size: 35.9 MB (35893220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4cc6184057ac1eb5fc58dd9e768ab4b268428194738557abd0a5c449847f4e`  
		Last Modified: Wed, 10 Feb 2021 15:39:28 GMT  
		Size: 189.8 MB (189770332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a2b410b46764bea500003e94a005ad6a5aad15043182656b5533da26869063`  
		Last Modified: Wed, 10 Feb 2021 15:38:45 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1508d157d85bd45809b2786913e9b2f8ad82c3e522fb20a301475274a141cdf`  
		Last Modified: Wed, 10 Feb 2021 15:38:43 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f7f7376c9934eb35c936761ed9d9d648852005adba1e5b2c9f999738dc1f5`  
		Last Modified: Wed, 10 Feb 2021 15:38:42 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae96c5b515917ac1435353e8a83b3d0fa2b0612fd72efc7015c0a1532f862b`  
		Last Modified: Wed, 10 Feb 2021 15:38:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cea76b607b5dcc335d4b2b388d285c00744262df87bd554f5795c5422d89f1`  
		Last Modified: Wed, 10 Feb 2021 15:38:42 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:7.11.1`

```console
$ docker pull kibana@sha256:ea7f70a31733dbae5536281612fccbfa823e89015a8a4fd6f9544a596e2edfb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kibana:7.11.1` - linux; amd64

```console
$ docker pull kibana@sha256:0570b27bb7c2947a50eeb1dd7cc09fa4bc51f1f234b1f113e01ac8e7443999a4
```

-	Docker Version: 20.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **389.5 MB (389485412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecf6e21a953f5148bee563966654193ca80c9bbd3d16553086cebb1e06c4a561`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Mon, 15 Feb 2021 13:35:37 GMT
EXPOSE 5601
# Mon, 15 Feb 2021 13:36:00 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y         fontconfig freetype shadow-utils libnss3.so  &&       yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Mon, 15 Feb 2021 13:36:02 GMT
RUN set -e ;   TINI_VERSION='v0.19.0' ;   TINI_BIN='tini-amd64' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Mon, 15 Feb 2021 13:36:02 GMT
RUN mkdir /usr/share/fonts/local
# Mon, 15 Feb 2021 13:36:04 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Mon, 15 Feb 2021 13:36:05 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Mon, 15 Feb 2021 13:36:05 GMT
RUN fc-cache -v
# Mon, 15 Feb 2021 13:36:32 GMT
COPY --chown=1000:0dir:42e16f38024e16af387b21fd506527840e6bb41e0a507387d8673b2992cfc716 in /usr/share/kibana 
# Mon, 15 Feb 2021 13:36:37 GMT
WORKDIR /usr/share/kibana
# Mon, 15 Feb 2021 13:36:38 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Mon, 15 Feb 2021 13:36:38 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 15 Feb 2021 13:36:38 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 Feb 2021 13:36:38 GMT
COPY --chown=1000:0file:6327494502800698df48e00f1f91972c882c036b3fda354262515e3410c28d4a in /usr/share/kibana/config/kibana.yml 
# Mon, 15 Feb 2021 13:36:38 GMT
COPY --chown=1000:0file:07f27eccee0d6cb9319627d224edc391ba0d2a271f5be067999987d49c4f63ea in /usr/local/bin/ 
# Mon, 15 Feb 2021 13:36:39 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Mon, 15 Feb 2021 13:36:41 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Mon, 15 Feb 2021 13:36:42 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Mon, 15 Feb 2021 13:36:42 GMT
LABEL org.label-schema.build-date=2021-02-15T13:32:51.720Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=348233f89825946d65101f6d9082567353459b8e org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.11.1 org.opencontainers.image.created=2021-02-15T13:32:51.720Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=348233f89825946d65101f6d9082567353459b8e org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.11.1
# Mon, 15 Feb 2021 13:36:42 GMT
USER kibana
# Mon, 15 Feb 2021 13:36:42 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 15 Feb 2021 13:36:42 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ebb37b70cb173fcf8d55fbec162912f00ba62ab51e00f8f481a5e90ff1b98c`  
		Last Modified: Wed, 17 Feb 2021 14:58:16 GMT  
		Size: 42.1 MB (42065458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3aad23fb3ebf23b5d17011d8b5d862866dea0171bfac96a36624d18455be0d`  
		Last Modified: Wed, 17 Feb 2021 14:57:31 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b0bd20a4ba9033d274a7877c7f8a6640304966e656cea8584fc4c8c9650038`  
		Last Modified: Wed, 17 Feb 2021 14:57:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d86c3c79c8f7796a59ffd28ddb671c72a5fe5df1cef691e3150d2383380d97`  
		Last Modified: Wed, 17 Feb 2021 14:57:27 GMT  
		Size: 16.5 MB (16460490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47820b9e28241cf80f544da2fc4a166839f61906f7e581cb7180ad30885aac40`  
		Last Modified: Wed, 17 Feb 2021 14:57:24 GMT  
		Size: 8.3 KB (8320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1739bfba4ea3b27d8f6fc810c5307d72ec17115d62a43e4f11f176ed97fb6a`  
		Last Modified: Wed, 17 Feb 2021 15:01:11 GMT  
		Size: 255.6 MB (255557115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918430b891458dad02cb7ba6fb6b3a10fa654ef5150ee50d9ca40f430e64976`  
		Last Modified: Wed, 17 Feb 2021 14:57:22 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975c08b89803706db6f6bc9ae0d166ca07ad115c73aeca547b56feca6e6e6735`  
		Last Modified: Wed, 17 Feb 2021 14:57:20 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f164ff9f9d5dc50f699fcafdf941880213ad143b9e8d995fcd7a77d37e57e8`  
		Last Modified: Wed, 17 Feb 2021 14:57:19 GMT  
		Size: 3.2 KB (3168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13ca2675e46f10d5546af67800263cd3b827eb293ab1e78a46bd1a427e2c1e0`  
		Last Modified: Wed, 17 Feb 2021 14:57:19 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee13c96a4d383fabeb5e5c100a8b54a3024aabcc25201f45a2db37cae6d43c3`  
		Last Modified: Wed, 17 Feb 2021 14:57:17 GMT  
		Size: 196.4 KB (196383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdbc424c1d3087133d18c378e4199700edef5e22c163d3f370afefd3d5e52ed`  
		Last Modified: Wed, 17 Feb 2021 14:57:16 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
