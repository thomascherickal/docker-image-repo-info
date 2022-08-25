<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.23`](#kibana6823)
-	[`kibana:7.17.6`](#kibana7176)
-	[`kibana:8.4.0`](#kibana840)

## `kibana:6.8.23`

```console
$ docker pull kibana@sha256:dd123d133fa7e995f83eef23df6aad30c589711e6171fee8db63097a7706eae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kibana:6.8.23` - linux; amd64

```console
$ docker pull kibana@sha256:adb468810c34ccc141f01ea79135d5a2f48d09890ecd08ce59ec94444f0a09f1
```

-	Docker Version: 20.10.10
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.8 MB (325750637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e174261beaec7ef8b8fc7e3df6b62b87e442f3451d408e7fe4525b151a061ebd`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Thu, 06 Jan 2022 22:40:29 GMT
EXPOSE 5601
# Thu, 06 Jan 2022 22:41:30 GMT
RUN yum update -y && yum install -y fontconfig freetype && yum clean all
# Thu, 06 Jan 2022 22:42:25 GMT
COPY --chown=1000:0dir:91d1ac171c4ceb98ce1764191b4bde36072fa18167199a2214eb559670a34b06 in /usr/share/kibana 
# Thu, 06 Jan 2022 22:42:28 GMT
WORKDIR /usr/share/kibana
# Thu, 06 Jan 2022 22:42:29 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 06 Jan 2022 22:42:30 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 06 Jan 2022 22:42:30 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:42:31 GMT
COPY --chown=1000:0file:60b6181f28c99b362092ea6139b6d4112ddd0bef32d52563c33b26bdc2b51318 in /usr/share/kibana/config/kibana.yml 
# Thu, 06 Jan 2022 22:42:31 GMT
COPY --chown=1000:0file:7d472d1939e23e2f10e7c5fd1e9166eefd646214aa0d8a1c09d92af71c9cbd87 in /usr/local/bin/ 
# Thu, 06 Jan 2022 22:42:34 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 06 Jan 2022 22:42:39 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Thu, 06 Jan 2022 22:42:39 GMT
USER kibana
# Thu, 06 Jan 2022 22:42:40 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=6.8.23 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License license=Elastic License
# Thu, 06 Jan 2022 22:42:41 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842e4249e10492c4ab35d3e76f93cad922781f7d61752e1b4b3ca25636b5c56f`  
		Last Modified: Thu, 13 Jan 2022 16:11:43 GMT  
		Size: 61.0 MB (61010271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f4609300d658bf52b006741f5590abdf93d8d575e0ddf04ce5be28e82b50a4`  
		Last Modified: Thu, 13 Jan 2022 16:11:58 GMT  
		Size: 188.6 MB (188638449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784cf3007996898653e12b85f6cf71597349b95377a60e1c57d40aaf682ddc3e`  
		Last Modified: Thu, 13 Jan 2022 16:11:32 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e291dafdd6a7112a1b18f88f42cbef2225094f58f18d2f364d0d34006b69e1`  
		Last Modified: Thu, 13 Jan 2022 16:11:30 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c90f666fc9fbd62181b8b51f391386e0a1a137451605b6f0a105171abe51380`  
		Last Modified: Thu, 13 Jan 2022 16:11:29 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8abc3a9f73c2948571140a610a8c9f79b87c33bcbfdf320cd0f6e5d9fbe944`  
		Last Modified: Thu, 13 Jan 2022 16:11:29 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73634fb3f49af52529a1b025a3cebf50531fdbcbdb3876b7b00908dfe9dc0a85`  
		Last Modified: Thu, 13 Jan 2022 16:11:29 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:7.17.6`

```console
$ docker pull kibana@sha256:49ce9c48deea2a50da7f88fc7e3b6d819b15f4af905f6a227c13a3fe31364eda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kibana:7.17.6` - linux; amd64

```console
$ docker pull kibana@sha256:a031b02cd029ce22abed498362f4ebbcd63cc8fc7bc364e95de7ceeb5eb1dfb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325453183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4239c3f5bd3d17a8a64cde246ea36e3329effe834ac38e3151f9279ec4fff004`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Mon, 22 Aug 2022 11:31:20 GMT
RUN EXPOSE map[5601/tcp:{}]
# Mon, 22 Aug 2022 11:31:20 GMT
RUN RUN /bin/sh -c for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Mon, 22 Aug 2022 11:31:21 GMT
RUN RUN /bin/sh -c set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Mon, 22 Aug 2022 11:31:21 GMT
RUN RUN /bin/sh -c mkdir /usr/share/fonts/local # buildkit
# Mon, 22 Aug 2022 11:31:22 GMT
RUN RUN /bin/sh -c curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Mon, 22 Aug 2022 11:31:23 GMT
RUN RUN /bin/sh -c echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Mon, 22 Aug 2022 11:31:23 GMT
RUN RUN /bin/sh -c fc-cache -v # buildkit
# Mon, 22 Aug 2022 11:32:25 GMT
RUN COPY /usr/share/kibana /usr/share/kibana # buildkit
# Mon, 22 Aug 2022 11:32:25 GMT
RUN WORKDIR /usr/share/kibana
# Mon, 22 Aug 2022 11:32:25 GMT
RUN RUN /bin/sh -c ln -s /usr/share/kibana /opt/kibana # buildkit
# Mon, 22 Aug 2022 11:32:25 GMT
RUN ENV ELASTIC_CONTAINER=true
# Mon, 22 Aug 2022 11:32:25 GMT
RUN ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 Aug 2022 11:32:26 GMT
RUN COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Mon, 22 Aug 2022 11:32:26 GMT
RUN COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Mon, 22 Aug 2022 11:32:26 GMT
RUN RUN /bin/sh -c chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Mon, 22 Aug 2022 11:32:27 GMT
RUN RUN /bin/sh -c find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Mon, 22 Aug 2022 11:32:27 GMT
RUN RUN /bin/sh -c groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Mon, 22 Aug 2022 11:32:27 GMT
RUN LABEL org.label-schema.build-date=2022-08-22T11:05:33.075Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=d2647b053b769d4517fbb14ce37765808a1b6e0c org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.6 org.opencontainers.image.created=2022-08-22T11:05:33.075Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=d2647b053b769d4517fbb14ce37765808a1b6e0c org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.6
# Mon, 22 Aug 2022 11:32:27 GMT
RUN ENTRYPOINT ["/bin/tini" "--"]
# Mon, 22 Aug 2022 11:32:27 GMT
RUN CMD ["/usr/local/bin/kibana-docker"]
# Mon, 22 Aug 2022 11:32:27 GMT
RUN USER kibana
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4909e7eae242ddcd04ea4cac57905cde860307c129f881473a17640f26c77c22`  
		Last Modified: Wed, 24 Aug 2022 23:34:31 GMT  
		Size: 11.4 MB (11402602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe40d6fb24c0886259a755e922a95303529eb029e1832db71f8a14982cfba201`  
		Last Modified: Wed, 24 Aug 2022 23:34:29 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcaf4a9c0882e6eb369888122a32f1f3ff9c9c17fe4d43d5115afcd3be4d69b`  
		Last Modified: Wed, 24 Aug 2022 23:34:27 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338bcf0d330658b4a5060ae46689eb526ad90811fe9fe3a5dad5f423052b025c`  
		Last Modified: Wed, 24 Aug 2022 23:34:28 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af5505a20feb5f0627a99c2f926ba87c2c8de93c16ad5ce60b2fb05fde4e38e`  
		Last Modified: Wed, 24 Aug 2022 23:34:27 GMT  
		Size: 5.3 KB (5288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe77eb249d6ffdbb9ace2b8c472e6601e48fa6eae4b6c3e6ab4a52560ff4d4d0`  
		Last Modified: Wed, 24 Aug 2022 23:34:58 GMT  
		Size: 268.8 MB (268805804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25728b71e5a44fc7a4e2eded91557b5d50399f103c7d69bb69c4d711242bc7b`  
		Last Modified: Wed, 24 Aug 2022 23:34:26 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35830107ab914645b77f72703837b4845d46e2ea9e789ecd0e2a785aff4715f1`  
		Last Modified: Wed, 24 Aug 2022 23:34:24 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1209f693487452a4793e8fcab07dd4e8d085bd70ba07bc66e042cf4ad7be65`  
		Last Modified: Wed, 24 Aug 2022 23:34:24 GMT  
		Size: 4.5 KB (4509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb27ec66f047fd0c1c30851d2089ce1dedb11fc081f75efd80c5a1026a583a9`  
		Last Modified: Wed, 24 Aug 2022 23:34:24 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6216454c4b6e809c3de959f46e320085ee49f81831ffbf88f3dacd31f32d1da1`  
		Last Modified: Wed, 24 Aug 2022 23:34:24 GMT  
		Size: 189.4 KB (189390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baec0471caba7ed8badff4bb66852efdf363c69411b328a0e2cf26ea0b1971d`  
		Last Modified: Wed, 24 Aug 2022 23:34:24 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.4.0`

```console
$ docker pull kibana@sha256:6bc28151e59015b90c6432a5efa68c29e68e631ebb2aa28f4659d2f4d6741e1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kibana:8.4.0` - linux; amd64

```console
$ docker pull kibana@sha256:d4b350ff15fa3ac3a5e2910043b615ad7d61b684eef76a0f49a9eaf5441a68e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.4 MB (342410724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890eaa34d22dcf7acf1aeb6459e46f147ba4cd3f4d8ca60d6e66816283cd9485`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Fri, 19 Aug 2022 11:36:31 GMT
RUN EXPOSE map[5601/tcp:{}]
# Fri, 19 Aug 2022 11:36:31 GMT
RUN RUN /bin/sh -c for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Fri, 19 Aug 2022 11:36:32 GMT
RUN RUN /bin/sh -c set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Fri, 19 Aug 2022 11:36:33 GMT
RUN RUN /bin/sh -c mkdir /usr/share/fonts/local # buildkit
# Fri, 19 Aug 2022 11:36:33 GMT
RUN RUN /bin/sh -c curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Fri, 19 Aug 2022 11:36:34 GMT
RUN RUN /bin/sh -c echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Fri, 19 Aug 2022 11:36:34 GMT
RUN RUN /bin/sh -c fc-cache -v # buildkit
# Fri, 19 Aug 2022 11:37:40 GMT
RUN COPY /usr/share/kibana /usr/share/kibana # buildkit
# Fri, 19 Aug 2022 11:37:40 GMT
RUN WORKDIR /usr/share/kibana
# Fri, 19 Aug 2022 11:37:41 GMT
RUN RUN /bin/sh -c ln -s /usr/share/kibana /opt/kibana # buildkit
# Fri, 19 Aug 2022 11:37:41 GMT
RUN ENV ELASTIC_CONTAINER=true
# Fri, 19 Aug 2022 11:37:41 GMT
RUN ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Aug 2022 11:37:41 GMT
RUN COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Fri, 19 Aug 2022 11:37:41 GMT
RUN COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Fri, 19 Aug 2022 11:37:41 GMT
RUN RUN /bin/sh -c chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Fri, 19 Aug 2022 11:37:42 GMT
RUN RUN /bin/sh -c find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Fri, 19 Aug 2022 11:37:42 GMT
RUN RUN /bin/sh -c groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Fri, 19 Aug 2022 11:37:42 GMT
RUN LABEL org.label-schema.build-date=2022-08-19T11:09:25.439Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=1922ab0b6f8dc2906ef10f3fb65fc4d0e0076f90 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.4.0 org.opencontainers.image.created=2022-08-19T11:09:25.439Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=1922ab0b6f8dc2906ef10f3fb65fc4d0e0076f90 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.4.0
# Fri, 19 Aug 2022 11:37:42 GMT
RUN ENTRYPOINT ["/bin/tini" "--"]
# Fri, 19 Aug 2022 11:37:42 GMT
RUN CMD ["/usr/local/bin/kibana-docker"]
# Fri, 19 Aug 2022 11:37:42 GMT
RUN USER kibana
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8004f215385420feb4682858d910d9b1cd1df96d0dd17a54eb6e214f5279de3`  
		Last Modified: Wed, 24 Aug 2022 23:33:50 GMT  
		Size: 11.4 MB (11402477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7547b9592f5dc8e9bd3d01bd4ac4e563181125d661b365c68835464e13e5e903`  
		Last Modified: Wed, 24 Aug 2022 23:33:48 GMT  
		Size: 9.5 KB (9525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47342ef40781c2e0795526dca974b4ac6d08daca3a6c7473fe2e3bcc6363b5f`  
		Last Modified: Wed, 24 Aug 2022 23:33:47 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59563107ddc8540ecd3a2f8e39c423746ef9452df9a7a1b9e8383b44b88be180`  
		Last Modified: Wed, 24 Aug 2022 23:33:47 GMT  
		Size: 16.5 MB (16460478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1964775507f928f72c238c747d9696eb6e73f51c19eab2c5410967fde5fa21`  
		Last Modified: Wed, 24 Aug 2022 23:33:45 GMT  
		Size: 5.3 KB (5279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67064b347a2b42b4efd6257dcf3645b72696b54effbd392249eae2cdf0967b5`  
		Last Modified: Wed, 24 Aug 2022 23:34:17 GMT  
		Size: 285.8 MB (285763631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b929eac129ea4901bea485809622bcbeaccb172f551c4dbbac90d3469325d7`  
		Last Modified: Wed, 24 Aug 2022 23:33:45 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8af0fc81363de87fa11cc5b656892ae6513198f880c089ac42e28a43a00c5a`  
		Last Modified: Wed, 24 Aug 2022 23:33:42 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958fafb9f481c54bf180967b58902019c6c225c6aceb09f722f982dd4c650749`  
		Last Modified: Wed, 24 Aug 2022 23:33:43 GMT  
		Size: 4.4 KB (4380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be11f7d3bb417728dd5bc8dcad5c2a7a4c70fef8326e0694e8a0b1834af2e030`  
		Last Modified: Wed, 24 Aug 2022 23:33:43 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321d0a7c950c8d1a2fdd334e50370e8b3930b993fc0c9ab2fc6d1f831495860b`  
		Last Modified: Wed, 24 Aug 2022 23:33:43 GMT  
		Size: 189.4 KB (189388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a090a6415eec403665afb724be9a995c1c2cac51fd77ae5855f485e013daa7b4`  
		Last Modified: Wed, 24 Aug 2022 23:33:44 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
