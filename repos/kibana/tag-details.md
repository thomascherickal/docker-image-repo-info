<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.23`](#kibana6823)
-	[`kibana:7.17.1`](#kibana7171)
-	[`kibana:8.0.1`](#kibana801)

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

## `kibana:7.17.1`

```console
$ docker pull kibana@sha256:bd67c1b5e8fda76890a548f702010fdc952a47708a5fbf18eb62790c7fca669a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.17.1` - linux; amd64

```console
$ docker pull kibana@sha256:6fc9b88682bb1f7fa4c5d553e9950fd18fa1d21170a05cb752361f7028ef0bd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.2 MB (345181564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbc840d074ff322e16454ee3f28e3db9b2f5e5d4570ffc04173ad94834b0fca`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 23 Feb 2022 23:19:27 GMT
EXPOSE 5601
# Wed, 23 Feb 2022 23:19:47 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Wed, 23 Feb 2022 23:19:48 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Wed, 23 Feb 2022 23:19:49 GMT
RUN mkdir /usr/share/fonts/local
# Wed, 23 Feb 2022 23:19:50 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Wed, 23 Feb 2022 23:19:51 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Wed, 23 Feb 2022 23:19:51 GMT
RUN fc-cache -v
# Wed, 23 Feb 2022 23:20:19 GMT
COPY --chown=1000:0dir:66c9010dabdc0e2b163ad29c0bc754b5f7c65d80e580ef858ff7da5882cde522 in /usr/share/kibana 
# Wed, 23 Feb 2022 23:20:28 GMT
WORKDIR /usr/share/kibana
# Wed, 23 Feb 2022 23:20:29 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Wed, 23 Feb 2022 23:20:29 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 23 Feb 2022 23:20:29 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Feb 2022 23:20:29 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Wed, 23 Feb 2022 23:20:29 GMT
COPY file:4b05cc4ee8dc464b192dc25102b9385329fd96ca9e48428d3b36b7d2a9e4be58 in /usr/local/bin/ 
# Wed, 23 Feb 2022 23:20:31 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Wed, 23 Feb 2022 23:20:32 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Wed, 23 Feb 2022 23:20:33 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Wed, 23 Feb 2022 23:20:33 GMT
LABEL org.label-schema.build-date=2022-02-23T22:27:26.294Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=78e8422ed4e7d2054bd35b82a91299b3f7bd6231 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.1 org.opencontainers.image.created=2022-02-23T22:27:26.294Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=78e8422ed4e7d2054bd35b82a91299b3f7bd6231 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.1
# Wed, 23 Feb 2022 23:20:33 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 23 Feb 2022 23:20:33 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Wed, 23 Feb 2022 23:20:33 GMT
USER kibana
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a626211e3cfb6433bbb0cff2164cb229b75cbefa17cc074ec7b56aaaf3b2302`  
		Last Modified: Tue, 01 Mar 2022 10:18:40 GMT  
		Size: 13.1 MB (13098666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b68dfd213c09231653a94c830d954dd65a896f0b0afbfbbe8e9d9e9401891`  
		Last Modified: Tue, 01 Mar 2022 10:18:37 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2327f66fda0b3e6eb1daf65c0588de4758f002d59c2d277ba24184cff26a09f4`  
		Last Modified: Tue, 01 Mar 2022 10:18:34 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65c471c2d0c6c2119060b464910cd7710da922af843a06732b981e84f7940b1`  
		Last Modified: Tue, 01 Mar 2022 10:18:37 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bfe566b83ffbc1c4f354914220a75ac9e3fa2ea5f6ea91fdbbf700f8b1a6fb`  
		Last Modified: Tue, 01 Mar 2022 10:18:34 GMT  
		Size: 5.3 KB (5280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3548d824c5c4be6d525a6c3082191bb1e283652b2955ab29b1e9744c771cae0`  
		Last Modified: Tue, 01 Mar 2022 10:19:35 GMT  
		Size: 286.8 MB (286846693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ff5bce7e13de403400cd715b663ccd5dc872e4f4fe4a61318f331a32e9621c`  
		Last Modified: Tue, 01 Mar 2022 10:18:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9119495718111341888e67baf9d3db3b96b2b792fd07e571c7eee7f0e2a783ad`  
		Last Modified: Tue, 01 Mar 2022 10:18:30 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12919d251abfbb6cec5df59d39ce8be378a96464fbbdf80b6297af488e16ff`  
		Last Modified: Tue, 01 Mar 2022 10:18:30 GMT  
		Size: 4.5 KB (4483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d80876eb773dbe6466bf019e12dcb29579428d3cfc6f26a1427349c750ffd7`  
		Last Modified: Tue, 01 Mar 2022 10:18:30 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48854083c036baee1f764c4f15c6d843612ddf40911aa54b4eb8a7db2e29c64`  
		Last Modified: Tue, 01 Mar 2022 10:18:31 GMT  
		Size: 189.4 KB (189383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dd7b4ff9f008c7638541055bed4cb30703e154736791a0d923db10ebbd8dc0`  
		Last Modified: Tue, 01 Mar 2022 10:18:30 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.17.1` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:ef1bfddd24d04df0bc646ed3fd740ab63a2986a6f403ca109b1e98b9f8e9b3bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.2 MB (358232605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9caf9988206793eaee2b8fc855dbbadf98221a5fbc083c3fde55b7fca0f2cd`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Thu, 24 Feb 2022 00:41:15 GMT
EXPOSE 5601
# Thu, 24 Feb 2022 00:41:36 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Thu, 24 Feb 2022 00:41:37 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Thu, 24 Feb 2022 00:41:37 GMT
RUN mkdir /usr/share/fonts/local
# Thu, 24 Feb 2022 00:41:39 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Thu, 24 Feb 2022 00:41:40 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Thu, 24 Feb 2022 00:41:40 GMT
RUN fc-cache -v
# Thu, 24 Feb 2022 00:42:37 GMT
COPY --chown=1000:0dir:d46b5f9ec9018257184650761893e5e81904c22af616eda0092c33f2d430ed4f in /usr/share/kibana 
# Thu, 24 Feb 2022 00:42:39 GMT
WORKDIR /usr/share/kibana
# Thu, 24 Feb 2022 00:42:40 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 24 Feb 2022 00:42:40 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 24 Feb 2022 00:42:40 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Feb 2022 00:42:40 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Thu, 24 Feb 2022 00:42:40 GMT
COPY file:4b05cc4ee8dc464b192dc25102b9385329fd96ca9e48428d3b36b7d2a9e4be58 in /usr/local/bin/ 
# Thu, 24 Feb 2022 00:42:41 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 24 Feb 2022 00:42:43 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Thu, 24 Feb 2022 00:42:43 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Thu, 24 Feb 2022 00:42:43 GMT
LABEL org.label-schema.build-date=2022-02-24T00:37:48.474Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=78e8422ed4e7d2054bd35b82a91299b3f7bd6231 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.1 org.opencontainers.image.created=2022-02-24T00:37:48.474Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=78e8422ed4e7d2054bd35b82a91299b3f7bd6231 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.1
# Thu, 24 Feb 2022 00:42:44 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 24 Feb 2022 00:42:44 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 24 Feb 2022 00:42:44 GMT
USER kibana
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7983671e45452e58558399dbef289e2ece8fcf4617cb27b921eb41485f2da3`  
		Last Modified: Wed, 02 Mar 2022 16:08:22 GMT  
		Size: 12.9 MB (12920195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a6b9dee66c6e5921ca8322b867d6c21484893e37184050ce22b395727cc300`  
		Last Modified: Wed, 02 Mar 2022 16:08:20 GMT  
		Size: 9.1 KB (9102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd256ada5f848e2f7d147c3f21a9e842de239d7a4132e9139c819ad91886e0db`  
		Last Modified: Wed, 02 Mar 2022 16:08:18 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a680846641f3207b50dca54d2f203b4ccea3f0cf6892cbf93527d527ef07724`  
		Last Modified: Wed, 02 Mar 2022 16:08:20 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ba9c51b6a6007c42e5e1abc95a7c25e671d0f070dd4f91550d96d00b0ff265`  
		Last Modified: Wed, 02 Mar 2022 16:08:18 GMT  
		Size: 5.3 KB (5275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab791cc455d25d563176fb197588480171d73a2eb1ccd4dc99395b73bf199e9`  
		Last Modified: Wed, 02 Mar 2022 16:08:59 GMT  
		Size: 301.5 MB (301477085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10990a4f3b2f37da1f541f8c2115fa82bdf5f244fe670c45be2e3a59ea3b068a`  
		Last Modified: Wed, 02 Mar 2022 16:08:18 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02b9fb498614c296353cd4cce05ce2c5a499fa8fad302cfc464e288a9ffcc9f`  
		Last Modified: Wed, 02 Mar 2022 16:08:15 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fec27b4116cc1753a564752ab9d7b82359aeb05964d4282d4d5ca0ee88e84`  
		Last Modified: Wed, 02 Mar 2022 16:08:15 GMT  
		Size: 4.5 KB (4481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c774c08aa37efdb82834abf0aeccc2e4a7cda749b0a1eb675d9facd58e697b80`  
		Last Modified: Wed, 02 Mar 2022 16:08:15 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c819565bcb70943aa699cabaa1fbb9ed9a8daadedb756c2e6e59b8ca52de0218`  
		Last Modified: Wed, 02 Mar 2022 16:08:15 GMT  
		Size: 183.4 KB (183389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cb56c6e87a72db02f1d672b85ca43b1d4b2dbb2758a1fa85c3be83d83fb8d4`  
		Last Modified: Wed, 02 Mar 2022 16:08:16 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.0.1`

```console
$ docker pull kibana@sha256:1ec3a471e124c74a404c0d15820ff038d6e68241788bc6ff77b6462adedc654e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.0.1` - linux; amd64

```console
$ docker pull kibana@sha256:dce9cfbde0c096fe25ab526e57e61d4a03bd7853d8578aff81e1b2ac3834d4fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.7 MB (340665289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63dda2ae62aef9724f2e2f8f7ceafdfa08fa7556c72e7f7594e09addee8ce4da`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Thu, 24 Feb 2022 18:45:30 GMT
EXPOSE 5601
# Thu, 24 Feb 2022 18:45:52 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Thu, 24 Feb 2022 18:45:53 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Thu, 24 Feb 2022 18:45:54 GMT
RUN mkdir /usr/share/fonts/local
# Thu, 24 Feb 2022 18:45:55 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Thu, 24 Feb 2022 18:45:56 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Thu, 24 Feb 2022 18:45:56 GMT
RUN fc-cache -v
# Thu, 24 Feb 2022 18:46:29 GMT
COPY --chown=1000:0dir:cdabf8082fbccca261ecc4132a14188d9f29d73911872ddba84f4c68070c085d in /usr/share/kibana 
# Thu, 24 Feb 2022 18:46:34 GMT
WORKDIR /usr/share/kibana
# Thu, 24 Feb 2022 18:46:35 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 24 Feb 2022 18:46:35 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 24 Feb 2022 18:46:35 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Feb 2022 18:46:35 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Thu, 24 Feb 2022 18:46:35 GMT
COPY file:52e8ac9215e9f098c5481c490f121df8283bdefe968591a8fd8e938bb4b6e17c in /usr/local/bin/ 
# Thu, 24 Feb 2022 18:46:37 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 24 Feb 2022 18:46:38 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Thu, 24 Feb 2022 18:46:39 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Thu, 24 Feb 2022 18:46:39 GMT
LABEL org.label-schema.build-date=2022-02-24T18:37:08.177Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=9c546f1a2162580bb6968354371db8c2e080fe2b org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.0.1 org.opencontainers.image.created=2022-02-24T18:37:08.177Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=9c546f1a2162580bb6968354371db8c2e080fe2b org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.0.1
# Thu, 24 Feb 2022 18:46:39 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 24 Feb 2022 18:46:39 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 24 Feb 2022 18:46:39 GMT
USER kibana
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb752a2253c3e3d2e3c0cf8a7796fdbd7a7f26a41a868ec0bfbcdec6d2783813`  
		Last Modified: Tue, 01 Mar 2022 22:31:22 GMT  
		Size: 13.1 MB (13098789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f82bb684380e5468aa06b2ccba575102e0095e24448338693b327c802164a5`  
		Last Modified: Tue, 01 Mar 2022 22:31:13 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e870aac99eea4c035fe4d85671772f30a85ad7b3316ed23e0765b610f00bdc0`  
		Last Modified: Tue, 01 Mar 2022 22:31:12 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cff7f2b9dd8916da4546e0ff2e47ed52e57037704192845e046bca45139b819`  
		Last Modified: Tue, 01 Mar 2022 22:31:30 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5eef5fb352d7a45149c220a79993524d2116119570ecd948c34d9914aa520f`  
		Last Modified: Tue, 01 Mar 2022 22:31:07 GMT  
		Size: 5.3 KB (5287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecbe6d3db5e6065edff4043a156c0d3185bf91cd1c965997e244d3e7eeda03e`  
		Last Modified: Tue, 01 Mar 2022 22:33:27 GMT  
		Size: 282.3 MB (282330563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccac34d3b455e5040cb0665f1948062af4b558c664ab9a5a8a1a69410742998`  
		Last Modified: Tue, 01 Mar 2022 22:31:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17393a2809625d55af255ff850d12b22110d67e4333c5576985a5a52d1badf2e`  
		Last Modified: Tue, 01 Mar 2022 22:31:06 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4af56b41170d881e3e3982760bda4a474bcfd7bd73b1406c1e934e9f1522606`  
		Last Modified: Tue, 01 Mar 2022 22:31:01 GMT  
		Size: 4.2 KB (4210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c6a29c866cae5cdd0085cf9550a7eada64c5c4e61bc822182a2fa27f709cd5`  
		Last Modified: Tue, 01 Mar 2022 22:31:01 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b43cbfafc8e05b223880e69a5533b9203a0b21cabf296fc0816f8101ff13dd3`  
		Last Modified: Tue, 01 Mar 2022 22:31:01 GMT  
		Size: 189.4 KB (189382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610798a943d596a0e958e6f4bbaa5a20af3c9093d4f713eeed8d0edbb72e490b`  
		Last Modified: Tue, 01 Mar 2022 22:31:00 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.0.1` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:2d8e4af1ad8324d4bdb0728df19c725b8ac4291508423287f2704d725977b251
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.7 MB (353713773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fab8ca826139b744cfde77600c006b30c53070e5f10bb0b2b64031b730f98f9`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Thu, 24 Feb 2022 18:41:57 GMT
EXPOSE 5601
# Thu, 24 Feb 2022 18:42:18 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Thu, 24 Feb 2022 18:42:19 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Thu, 24 Feb 2022 18:42:20 GMT
RUN mkdir /usr/share/fonts/local
# Thu, 24 Feb 2022 18:42:22 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Thu, 24 Feb 2022 18:42:23 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Thu, 24 Feb 2022 18:42:23 GMT
RUN fc-cache -v
# Thu, 24 Feb 2022 18:42:51 GMT
COPY --chown=1000:0dir:75200434bbf093556cb5ed5872b29746fa00d4fe04b8fa56b6c5d674dbe9027e in /usr/share/kibana 
# Thu, 24 Feb 2022 18:42:54 GMT
WORKDIR /usr/share/kibana
# Thu, 24 Feb 2022 18:42:55 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 24 Feb 2022 18:42:55 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 24 Feb 2022 18:42:55 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Feb 2022 18:42:55 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Thu, 24 Feb 2022 18:42:55 GMT
COPY file:52e8ac9215e9f098c5481c490f121df8283bdefe968591a8fd8e938bb4b6e17c in /usr/local/bin/ 
# Thu, 24 Feb 2022 18:42:57 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 24 Feb 2022 18:42:58 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Thu, 24 Feb 2022 18:42:58 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Thu, 24 Feb 2022 18:42:59 GMT
LABEL org.label-schema.build-date=2022-02-24T18:38:22.239Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=9c546f1a2162580bb6968354371db8c2e080fe2b org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.0.1 org.opencontainers.image.created=2022-02-24T18:38:22.239Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=9c546f1a2162580bb6968354371db8c2e080fe2b org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.0.1
# Thu, 24 Feb 2022 18:42:59 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 24 Feb 2022 18:42:59 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 24 Feb 2022 18:42:59 GMT
USER kibana
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb113af31e363c31da88047f399d3b2868edf6a886661a91ff4fc853bb74d81`  
		Last Modified: Wed, 02 Mar 2022 16:07:29 GMT  
		Size: 12.9 MB (12920273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00416955fbbd83f42a0213329b03e249072d7d55a0ea34efa2c67e7b35d81a1`  
		Last Modified: Wed, 02 Mar 2022 16:07:27 GMT  
		Size: 9.1 KB (9102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9ea4c4cc1faf0ff332f9209090b7bb91c9a3ed2a44992574f77de827101a4d`  
		Last Modified: Wed, 02 Mar 2022 16:07:25 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af1e85b3b0443e2f57eef8034708814f99603b890f6cf18aba9deebb771b58d`  
		Last Modified: Wed, 02 Mar 2022 16:07:27 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9846a092b3b42c1209eaa333f3a4a70590d6c8f7c440090d2092b5095d44ba4b`  
		Last Modified: Wed, 02 Mar 2022 16:07:24 GMT  
		Size: 5.3 KB (5287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fab6637cd7e589ace33fb3a57a65dff7f40a5b7e0091906ffd51b470ed71a4`  
		Last Modified: Wed, 02 Mar 2022 16:08:06 GMT  
		Size: 297.0 MB (296958442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809c35475f172d6b187ec23a372e103448fd98a0f324e22544646497d42d8dcf`  
		Last Modified: Wed, 02 Mar 2022 16:07:24 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f4e35c6b0fdb421d29340d5a98d7aaaf990f9389f8a2c1fe44845178e6f648`  
		Last Modified: Wed, 02 Mar 2022 16:07:22 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d821ebf4e0e66b685abda718dc9c631d1cdca8bc8fa211ae63a45589b0e499`  
		Last Modified: Wed, 02 Mar 2022 16:07:22 GMT  
		Size: 4.2 KB (4210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8d30d58c35f7519adb5b0239c59721bb76a12604cc5b919927dce818a0d76d`  
		Last Modified: Wed, 02 Mar 2022 16:07:22 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb8177c6be3d67bd714c46aa90e90a1cdf734b36ee8786538b814f16fae7ecd`  
		Last Modified: Wed, 02 Mar 2022 16:07:22 GMT  
		Size: 183.4 KB (183388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f65365334939f3f18ed5c6588c38baf0c6657985c09e79cde927461b7924c1f`  
		Last Modified: Wed, 02 Mar 2022 16:07:22 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
