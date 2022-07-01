<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.23`](#kibana6823)
-	[`kibana:7.17.5`](#kibana7175)
-	[`kibana:8.3.1`](#kibana831)

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

## `kibana:7.17.5`

```console
$ docker pull kibana@sha256:fd5ab4aecc6b648c3c3ae8557b691fae54dd81e9c238522a6174cc52a3b6a0a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.17.5` - linux; amd64

```console
$ docker pull kibana@sha256:80d5bb4429cbba76a6f81f6087f3bd368709feb94de2b352fd9a5ee4ca12f854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.7 MB (326696767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5756b819359becc22c1bb41fd61e10ccf8bc21c6f5ba4331e03bc833bd989f35`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 11:36:02 GMT
RUN EXPOSE map[5601/tcp:{}]
# Thu, 23 Jun 2022 11:36:02 GMT
RUN RUN /bin/sh -c for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 23 Jun 2022 11:36:04 GMT
RUN RUN /bin/sh -c set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 23 Jun 2022 11:36:04 GMT
RUN RUN /bin/sh -c mkdir /usr/share/fonts/local # buildkit
# Thu, 23 Jun 2022 11:36:05 GMT
RUN RUN /bin/sh -c curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 23 Jun 2022 11:36:05 GMT
RUN RUN /bin/sh -c echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 23 Jun 2022 11:36:05 GMT
RUN RUN /bin/sh -c fc-cache -v # buildkit
# Thu, 23 Jun 2022 11:37:05 GMT
RUN COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 23 Jun 2022 11:37:05 GMT
RUN WORKDIR /usr/share/kibana
# Thu, 23 Jun 2022 11:37:05 GMT
RUN RUN /bin/sh -c ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 23 Jun 2022 11:37:05 GMT
RUN ENV ELASTIC_CONTAINER=true
# Thu, 23 Jun 2022 11:37:05 GMT
RUN ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 11:37:05 GMT
RUN COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 23 Jun 2022 11:37:05 GMT
RUN COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 23 Jun 2022 11:37:06 GMT
RUN RUN /bin/sh -c chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 23 Jun 2022 11:37:07 GMT
RUN RUN /bin/sh -c find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 23 Jun 2022 11:37:07 GMT
RUN RUN /bin/sh -c groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 23 Jun 2022 11:37:07 GMT
RUN LABEL org.label-schema.build-date=2022-06-23T11:10:20.179Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=cd49631953cd3a928d6dbaadc722fe1d51191fa4 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.5 org.opencontainers.image.created=2022-06-23T11:10:20.179Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=cd49631953cd3a928d6dbaadc722fe1d51191fa4 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.5
# Thu, 23 Jun 2022 11:37:07 GMT
RUN ENTRYPOINT ["/bin/tini" "--"]
# Thu, 23 Jun 2022 11:37:07 GMT
RUN CMD ["/usr/local/bin/kibana-docker"]
# Thu, 23 Jun 2022 11:37:07 GMT
RUN USER kibana
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382214fb9ec073ab20674e06d9610ec7eb5c24ca000ed72723bf02fbd4c82476`  
		Last Modified: Fri, 01 Jul 2022 01:24:46 GMT  
		Size: 12.8 MB (12779359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26094ac7658d71bf488651b887b072ff53b5691153124ae0b1b4543ff4b1ad32`  
		Last Modified: Fri, 01 Jul 2022 01:24:44 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55e1db6dca2b1e28cd1f18da67e23e10a410591fc4ff126d7514b8fbc5c808c`  
		Last Modified: Fri, 01 Jul 2022 01:24:41 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247156d3f804c14264fd81b2543ae7a6e5cf5d93371e604cd90553d2b6a67368`  
		Last Modified: Fri, 01 Jul 2022 01:24:43 GMT  
		Size: 16.5 MB (16460478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ca53a1282011aec357cc5707a1ff6a432ee33c1a3492480c76d073222d613d`  
		Last Modified: Fri, 01 Jul 2022 01:24:41 GMT  
		Size: 5.3 KB (5292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387da1d0a375c032c4f099d587215502f5eaddad7f4786bd8b026e79cc880b75`  
		Last Modified: Fri, 01 Jul 2022 01:25:12 GMT  
		Size: 268.7 MB (268672587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140d066295dd32b3ccc0bbf330e444e06d02e688d0453af2d15a7587345b3c1c`  
		Last Modified: Fri, 01 Jul 2022 01:24:41 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd852f849779d38acc06e7c158d164bf319c3c094281bf11223eb09d8979d4b5`  
		Last Modified: Fri, 01 Jul 2022 01:24:38 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf553866d833c5e12eac37dda61edf9c20e3861707e4b0ed36237094fc4295ba`  
		Last Modified: Fri, 01 Jul 2022 01:24:38 GMT  
		Size: 4.5 KB (4505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f7618cd501b7d79cdd8cee7e51f79e281ed01d84fb63003f6424fd3c987ec`  
		Last Modified: Fri, 01 Jul 2022 01:24:38 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a43030fb61cf300f26d38bd9f41840c9df5f79e44297d4e45cc582375f9f6f`  
		Last Modified: Fri, 01 Jul 2022 01:24:38 GMT  
		Size: 189.4 KB (189387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967d419c015388a96356a866746fc7f7b8cf87819fd5d3fcf448140ccc77a3df`  
		Last Modified: Fri, 01 Jul 2022 01:24:38 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.17.5` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:aff54cc9e8458f46c288cf8b6c6fe312bb92bb288c7c35f0dcdbfd08eaaeca17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339734068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54cdeed819c30fc7c7a4aadf2448e449d3a3c1989dfd1fd7440d3366ae4b8500`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 11:39:10 GMT
RUN EXPOSE map[5601/tcp:{}]
# Thu, 23 Jun 2022 11:39:10 GMT
RUN RUN /bin/sh -c for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 23 Jun 2022 11:39:11 GMT
RUN RUN /bin/sh -c set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 23 Jun 2022 11:39:12 GMT
RUN RUN /bin/sh -c mkdir /usr/share/fonts/local # buildkit
# Thu, 23 Jun 2022 11:39:15 GMT
RUN RUN /bin/sh -c curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 23 Jun 2022 11:39:16 GMT
RUN RUN /bin/sh -c echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 23 Jun 2022 11:39:16 GMT
RUN RUN /bin/sh -c fc-cache -v # buildkit
# Thu, 23 Jun 2022 11:40:11 GMT
RUN COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 23 Jun 2022 11:40:11 GMT
RUN WORKDIR /usr/share/kibana
# Thu, 23 Jun 2022 11:40:12 GMT
RUN RUN /bin/sh -c ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 23 Jun 2022 11:40:12 GMT
RUN ENV ELASTIC_CONTAINER=true
# Thu, 23 Jun 2022 11:40:12 GMT
RUN ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 11:40:12 GMT
RUN COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 23 Jun 2022 11:40:12 GMT
RUN COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 23 Jun 2022 11:40:13 GMT
RUN RUN /bin/sh -c chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 23 Jun 2022 11:40:14 GMT
RUN RUN /bin/sh -c find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 23 Jun 2022 11:40:14 GMT
RUN RUN /bin/sh -c groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 23 Jun 2022 11:40:14 GMT
RUN LABEL org.label-schema.build-date=2022-06-23T11:10:20.179Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=cd49631953cd3a928d6dbaadc722fe1d51191fa4 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.5 org.opencontainers.image.created=2022-06-23T11:10:20.179Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=cd49631953cd3a928d6dbaadc722fe1d51191fa4 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.5
# Thu, 23 Jun 2022 11:40:14 GMT
RUN ENTRYPOINT ["/bin/tini" "--"]
# Thu, 23 Jun 2022 11:40:14 GMT
RUN CMD ["/usr/local/bin/kibana-docker"]
# Thu, 23 Jun 2022 11:40:14 GMT
RUN USER kibana
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfd1ac1eb9ebb50eedf7ec1329c61b9902b6ebf016d9dbfbc3f8c038eeff1f`  
		Last Modified: Fri, 01 Jul 2022 00:46:04 GMT  
		Size: 12.6 MB (12573182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afc56e882a0b8cf0bc4a06603e8b0d895704326706e315e8c95a8a57fc52993`  
		Last Modified: Fri, 01 Jul 2022 00:46:02 GMT  
		Size: 9.1 KB (9101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a956f2b6d5b1d379f2e13ead9b13b7ef8d7f510099605538eaa9a50b36b17a7`  
		Last Modified: Fri, 01 Jul 2022 00:46:00 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342f4ef286581269b89f853a8f07b39baad9f63a1f4b3aa6d58f73e36584557`  
		Last Modified: Fri, 01 Jul 2022 00:46:02 GMT  
		Size: 16.5 MB (16460488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591f06e840233cef75b86cd9af61daa5471125711701670db05f3c0dc1202741`  
		Last Modified: Fri, 01 Jul 2022 00:46:00 GMT  
		Size: 5.3 KB (5299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d950d19e970c30a0fa62d361aca35cbe2c443086b42712dd46849fcb4afb13b`  
		Last Modified: Fri, 01 Jul 2022 00:46:35 GMT  
		Size: 283.3 MB (283303885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97d37c682f504ce8afe2ad1b97a5f2ca7a0664fd5b60143be433e7a52a0045f`  
		Last Modified: Fri, 01 Jul 2022 00:45:59 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd853c7622229bd45f3c1239dceaa1afaca2b44ad46612501948826e3ca979b0`  
		Last Modified: Fri, 01 Jul 2022 00:45:57 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88c74cc962c83e8665fb800119c721401fa0a3171222a063cbd6e195d4d116f`  
		Last Modified: Fri, 01 Jul 2022 00:45:57 GMT  
		Size: 4.5 KB (4505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dd7dc236f38a2d30a8099abf1a5eb9b0a26c82a8dc4fc85dc8e1a57b087c91`  
		Last Modified: Fri, 01 Jul 2022 00:45:57 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312475f70d9ef631aa6592827a35d5571a5941cecc8e993231d307b63199315`  
		Last Modified: Fri, 01 Jul 2022 00:45:57 GMT  
		Size: 183.4 KB (183393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b2cf6978dc3bcc1b8c4d26407569c9b0b89862a9ef2c2b4023ca5bfbe8a1f7`  
		Last Modified: Fri, 01 Jul 2022 00:45:57 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.3.1`

```console
$ docker pull kibana@sha256:f5f46e4444c1902be031ab28cdb066e2116c7c3eb461a7371dc8f9c6cdb1b328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.3.1` - linux; amd64

```console
$ docker pull kibana@sha256:01360a5d64c68c447b1df858118d065c3a3d78b51da83da8ec06f816aa66e36e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.5 MB (332506571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da965013399c575489c0996b8d397fab6c7fecbd28b5e044d4b7a8ff45e0dae`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Wed, 29 Jun 2022 12:47:03 GMT
RUN EXPOSE map[5601/tcp:{}]
# Wed, 29 Jun 2022 12:47:03 GMT
RUN RUN /bin/sh -c for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Wed, 29 Jun 2022 12:47:04 GMT
RUN RUN /bin/sh -c set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Wed, 29 Jun 2022 12:47:05 GMT
RUN RUN /bin/sh -c mkdir /usr/share/fonts/local # buildkit
# Wed, 29 Jun 2022 12:47:06 GMT
RUN RUN /bin/sh -c curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Wed, 29 Jun 2022 12:47:06 GMT
RUN RUN /bin/sh -c echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Wed, 29 Jun 2022 12:47:07 GMT
RUN RUN /bin/sh -c fc-cache -v # buildkit
# Wed, 29 Jun 2022 12:48:18 GMT
RUN COPY /usr/share/kibana /usr/share/kibana # buildkit
# Wed, 29 Jun 2022 12:48:18 GMT
RUN WORKDIR /usr/share/kibana
# Wed, 29 Jun 2022 12:48:18 GMT
RUN RUN /bin/sh -c ln -s /usr/share/kibana /opt/kibana # buildkit
# Wed, 29 Jun 2022 12:48:18 GMT
RUN ENV ELASTIC_CONTAINER=true
# Wed, 29 Jun 2022 12:48:18 GMT
RUN ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 12:48:18 GMT
RUN COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Wed, 29 Jun 2022 12:48:18 GMT
RUN COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Wed, 29 Jun 2022 12:48:19 GMT
RUN RUN /bin/sh -c chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Wed, 29 Jun 2022 12:48:20 GMT
RUN RUN /bin/sh -c find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Wed, 29 Jun 2022 12:48:20 GMT
RUN RUN /bin/sh -c groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Wed, 29 Jun 2022 12:48:20 GMT
RUN LABEL org.label-schema.build-date=2022-06-29T12:23:27.577Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=a4f8dc60edb19553f16c166ea79c83c16572897a org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.3.1 org.opencontainers.image.created=2022-06-29T12:23:27.577Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=a4f8dc60edb19553f16c166ea79c83c16572897a org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.3.1
# Wed, 29 Jun 2022 12:48:20 GMT
RUN ENTRYPOINT ["/bin/tini" "--"]
# Wed, 29 Jun 2022 12:48:20 GMT
RUN CMD ["/usr/local/bin/kibana-docker"]
# Wed, 29 Jun 2022 12:48:20 GMT
RUN USER kibana
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad8383db02eb114b932f4dfb3960d059152df7a323d6c72b4c99faafcecaa3d`  
		Last Modified: Fri, 01 Jul 2022 01:24:04 GMT  
		Size: 12.8 MB (12779407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbfe5e9142c8f5111d7e924b3bf7fd0a5f6ebe3328eb3d867d5920c67574c96`  
		Last Modified: Fri, 01 Jul 2022 01:24:02 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7fcf902e02788e8f243687cb4c6a616a0c74552ab90a373b599e847c0cd2bf`  
		Last Modified: Fri, 01 Jul 2022 01:24:02 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f22b40bfadbcf9950f02aaf17236ee449641befc3558b4cb7090ce397785ba8`  
		Last Modified: Fri, 01 Jul 2022 01:24:01 GMT  
		Size: 16.5 MB (16460481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded8839e3f891c55683eb5f33a3eb36aa9aadc9eee46cf4eea37438e88ecf8d8`  
		Last Modified: Fri, 01 Jul 2022 01:23:59 GMT  
		Size: 5.3 KB (5298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18bca62bb3d5d1ab80757a54bb9336841601617665e1a9625c03c30a75207fc8`  
		Last Modified: Fri, 01 Jul 2022 01:24:30 GMT  
		Size: 274.5 MB (274482433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672036976551c36a6b14e5bba918cb238240d67dfe77956dd24149d7cf762d6b`  
		Last Modified: Fri, 01 Jul 2022 01:23:59 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edd4ccd4cf38f0fda5690d12c2442c928df8f2029af1e85d91aef19e5917fc5`  
		Last Modified: Fri, 01 Jul 2022 01:23:56 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d304014ef23a471a4f3cb0d835662e95b19e96943e7d251a606e98c2536f173f`  
		Last Modified: Fri, 01 Jul 2022 01:23:56 GMT  
		Size: 4.4 KB (4394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ec41e86bfbe74058187d2c433543e126ea3e1d31a91c325d29611031227456`  
		Last Modified: Fri, 01 Jul 2022 01:23:56 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df984c9df0511293cef7d9267257741852ae56d790c832f4ec770198cd20e4cf`  
		Last Modified: Fri, 01 Jul 2022 01:23:56 GMT  
		Size: 189.4 KB (189389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0be37a9cdfbe7492a1c591b7edefc2d5becbc8699d6657dfe9cb584c0ea2f2`  
		Last Modified: Fri, 01 Jul 2022 01:23:59 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.3.1` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:d795c0a4876c9c8a9e46f2c7a5ee577599ea2d599b788327acd2d6fe91c2201e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.6 MB (345557088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f57e7cd70e2f837fef47ec3939265dc0a496a3b3b3d6b36a837ad48c5002a082`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Wed, 29 Jun 2022 12:50:24 GMT
RUN EXPOSE map[5601/tcp:{}]
# Wed, 29 Jun 2022 12:50:24 GMT
RUN RUN /bin/sh -c for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Wed, 29 Jun 2022 12:50:26 GMT
RUN RUN /bin/sh -c set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Wed, 29 Jun 2022 12:50:26 GMT
RUN RUN /bin/sh -c mkdir /usr/share/fonts/local # buildkit
# Wed, 29 Jun 2022 12:50:29 GMT
RUN RUN /bin/sh -c curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Wed, 29 Jun 2022 12:50:29 GMT
RUN RUN /bin/sh -c echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Wed, 29 Jun 2022 12:50:31 GMT
RUN RUN /bin/sh -c fc-cache -v # buildkit
# Wed, 29 Jun 2022 12:51:36 GMT
RUN COPY /usr/share/kibana /usr/share/kibana # buildkit
# Wed, 29 Jun 2022 12:51:36 GMT
RUN WORKDIR /usr/share/kibana
# Wed, 29 Jun 2022 12:51:36 GMT
RUN RUN /bin/sh -c ln -s /usr/share/kibana /opt/kibana # buildkit
# Wed, 29 Jun 2022 12:51:36 GMT
RUN ENV ELASTIC_CONTAINER=true
# Wed, 29 Jun 2022 12:51:36 GMT
RUN ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 12:51:36 GMT
RUN COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Wed, 29 Jun 2022 12:51:36 GMT
RUN COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Wed, 29 Jun 2022 12:51:37 GMT
RUN RUN /bin/sh -c chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Wed, 29 Jun 2022 12:51:38 GMT
RUN RUN /bin/sh -c find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Wed, 29 Jun 2022 12:51:38 GMT
RUN RUN /bin/sh -c groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Wed, 29 Jun 2022 12:51:38 GMT
RUN LABEL org.label-schema.build-date=2022-06-29T12:23:27.577Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=a4f8dc60edb19553f16c166ea79c83c16572897a org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.3.1 org.opencontainers.image.created=2022-06-29T12:23:27.577Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=a4f8dc60edb19553f16c166ea79c83c16572897a org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.3.1
# Wed, 29 Jun 2022 12:51:38 GMT
RUN ENTRYPOINT ["/bin/tini" "--"]
# Wed, 29 Jun 2022 12:51:38 GMT
RUN CMD ["/usr/local/bin/kibana-docker"]
# Wed, 29 Jun 2022 12:51:38 GMT
RUN USER kibana
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52323d621b316b37d5406e866498bfa22442cb4698073fd6353d80bd471a246`  
		Last Modified: Fri, 01 Jul 2022 00:45:15 GMT  
		Size: 12.6 MB (12573032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb4b08c93ac5ee043c6c9ff494c4eec40ec5cacdf59f0c529da49fc293ec59`  
		Last Modified: Fri, 01 Jul 2022 00:45:13 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5218b9f269cd8e0e5e843a4a5a36ce720a06bbfd74b5a8b2585df31a1e7219f0`  
		Last Modified: Fri, 01 Jul 2022 00:45:11 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d915355a14b07b53ee4a870ade3d484120748ed975dbc42fa8eac3c57353b75`  
		Last Modified: Fri, 01 Jul 2022 00:45:12 GMT  
		Size: 16.5 MB (16460488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffc83e3bcf021ef0c52740a54f6ede1557028bfb18f6f14038e39e27990185f`  
		Last Modified: Fri, 01 Jul 2022 00:45:11 GMT  
		Size: 5.3 KB (5301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0842d67ddecf0c6a060409ab3707ca0770ef8cf842972e1ac72d607b34a055`  
		Last Modified: Fri, 01 Jul 2022 00:45:47 GMT  
		Size: 289.1 MB (289127176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c1bd32025797fc38ededb2fd2fe8a2836d2df9e41c1d9639f5fbd22ff30527`  
		Last Modified: Fri, 01 Jul 2022 00:45:11 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28649d0085ff84e9ac35ccf2b6bd7e3ce5bd1fb66c7b500feeba6dff4c6e36`  
		Last Modified: Fri, 01 Jul 2022 00:45:08 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c46bb2607374b9f493a98513658edc55e2986174031e249bb0b907f866c252f`  
		Last Modified: Fri, 01 Jul 2022 00:45:08 GMT  
		Size: 4.4 KB (4391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34f95cabeffdabc099358df11fefeda61e4f50c5cb0e8807fd14cef1b9788ff`  
		Last Modified: Fri, 01 Jul 2022 00:45:08 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8011ac6447f4a5a7408ba97efa55595cccfb863ec6a8a76fbb98492f5f0d8d09`  
		Last Modified: Fri, 01 Jul 2022 00:45:08 GMT  
		Size: 183.4 KB (183393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2272462d144a10ede5fe016011e50037b3cf7c1e38dfbbf2045b3b844fd1e0`  
		Last Modified: Fri, 01 Jul 2022 00:45:08 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
