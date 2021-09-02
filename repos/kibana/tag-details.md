<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.18`](#kibana6818)
-	[`kibana:7.14.1`](#kibana7141)

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

## `kibana:7.14.1`

```console
$ docker pull kibana@sha256:e58baa69fc22e0069f2ecbbe79c91039718f08e16cb8bdf4d80a3a7ec5c709d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `kibana:7.14.1` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:48e9b552f02ac25bfab0d24ac8b4ffa5431b7abf55b072dd086e3d3be1d7fd4e
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **494.5 MB (494512919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89493da5b88901edd3fe157f01af7380566d19fa40f468b29fbaaebfc7f3c2f1`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Mon, 07 Dec 2020 23:42:06 GMT
ADD file:edd6e1253ec7bbb67b5a28d40c7d28b34a443c2cfa327bebf55c8b0b19484bf9 in / 
# Mon, 07 Dec 2020 23:42:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Mon, 07 Dec 2020 23:42:10 GMT
CMD ["/bin/bash"]
# Thu, 26 Aug 2021 10:16:31 GMT
EXPOSE 5601
# Thu, 26 Aug 2021 10:17:28 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y         fontconfig freetype shadow-utils nss  &&       yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Thu, 26 Aug 2021 10:17:31 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Thu, 26 Aug 2021 10:17:31 GMT
RUN mkdir /usr/share/fonts/local
# Thu, 26 Aug 2021 10:17:34 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Thu, 26 Aug 2021 10:17:34 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Thu, 26 Aug 2021 10:17:35 GMT
RUN fc-cache -v
# Thu, 26 Aug 2021 10:18:40 GMT
COPY --chown=1000:0dir:16a5f413c2201f355bdbf1ed3341072cadf3b4bb7985c4eeae9efe36f8c1d012 in /usr/share/kibana 
# Thu, 26 Aug 2021 10:18:42 GMT
WORKDIR /usr/share/kibana
# Thu, 26 Aug 2021 10:18:43 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 26 Aug 2021 10:18:43 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 26 Aug 2021 10:18:44 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Aug 2021 10:18:44 GMT
COPY --chown=1000:0file:ab38106de0b2164e20c73bb3449b4682fb9c654eac5b38ed7f560f16ed9c9105 in /usr/share/kibana/config/kibana.yml 
# Thu, 26 Aug 2021 10:18:44 GMT
COPY --chown=1000:0file:a971e8b1ef047eb3eecd6a3776ff0fa8a4e252d1c434e2fe5e7b840af024d381 in /usr/local/bin/ 
# Thu, 26 Aug 2021 10:18:45 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 26 Aug 2021 10:18:48 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Thu, 26 Aug 2021 10:18:48 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Thu, 26 Aug 2021 10:18:49 GMT
LABEL org.label-schema.build-date=2021-08-26T10:12:57.285Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=196ec3974d4c725a3d937725419e5ed7d8fdb104 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.14.1 org.opencontainers.image.created=2021-08-26T10:12:57.285Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=196ec3974d4c725a3d937725419e5ed7d8fdb104 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.14.1
# Thu, 26 Aug 2021 10:18:49 GMT
USER kibana
# Thu, 26 Aug 2021 10:18:49 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 26 Aug 2021 10:18:49 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:333cbcae3fb80b9a46084ae4caea81a84aafda9700fb646ab89206d0cfe213fd`  
		Last Modified: Mon, 07 Dec 2020 23:42:49 GMT  
		Size: 75.6 MB (75613064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e6a3bf60d13ed27f1dc7af1d0af39f1928a2ae3af7221fb4501bac830ffbbb`  
		Last Modified: Wed, 01 Sep 2021 23:43:46 GMT  
		Size: 97.1 MB (97093120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5720b29735ed4cda9ae7b4505608030fdf0288457d737dac5e8fb879b165a56c`  
		Last Modified: Wed, 01 Sep 2021 23:43:29 GMT  
		Size: 9.1 KB (9107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850ca43af4cfde657ecc458c0eb876bf7ff87b247a020ce6496f904e703833ff`  
		Last Modified: Wed, 01 Sep 2021 23:43:29 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5023744085ed1ccfd05904d433d0ce0704a39a1625bf137c0c44063edaf533d2`  
		Last Modified: Wed, 01 Sep 2021 23:43:29 GMT  
		Size: 16.5 MB (16460476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a05a2f3b87d481e058a47b6ee82939b8046e24c3e906f0aa4f5b2423f40f2`  
		Last Modified: Wed, 01 Sep 2021 23:43:27 GMT  
		Size: 8.3 KB (8313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab1bae4b46913f5e89ad4c7ffb92cdd4f0588ff7e79e8c5e32b49e62409f7c4`  
		Last Modified: Wed, 01 Sep 2021 23:44:10 GMT  
		Size: 305.1 MB (305123990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63939f8febcdf6fdb2d254ea564b919073557fb29c35eb438220b18ee9dc91`  
		Last Modified: Wed, 01 Sep 2021 23:43:27 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a60698c1e884841d0143e393852374c2bf606764644db0ca0fa94d2c5fbad6`  
		Last Modified: Wed, 01 Sep 2021 23:43:24 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d0aeb553b508a26c2077d274da76f3c8bcd143f7ac0e6847b0ddea2082b72`  
		Last Modified: Wed, 01 Sep 2021 23:43:24 GMT  
		Size: 4.4 KB (4442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c433e1455228027530dc6cce667b66f1c7b6d4616ebb0296aae66c5a944903c`  
		Last Modified: Wed, 01 Sep 2021 23:43:24 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8cd0ac0b69e93b20ebc3e44e853ca74cbfa3df10232bc2b7e75df4c5b1056be`  
		Last Modified: Wed, 01 Sep 2021 23:43:25 GMT  
		Size: 197.4 KB (197408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76a0ad84a2d801cf9904405402f6744425a90ec813acfae85a3e296e9a0a9cd`  
		Last Modified: Wed, 01 Sep 2021 23:43:24 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
