<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.23`](#kibana6823)
-	[`kibana:7.17.1`](#kibana7171)
-	[`kibana:8.1.1`](#kibana811)

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

## `kibana:8.1.1`

```console
$ docker pull kibana@sha256:6cb616bc5a432c554c7c034ac0cd7e6abba2cbe741e04d0527f2d3bdca301ae2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.1.1` - linux; amd64

```console
$ docker pull kibana@sha256:622f7c3a8234306e8da1b61ee941e5b482e9ce823b36f91e10279543018b98db
```

-	Docker Version: 20.10.13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.9 MB (330860355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d567696c16b31d90b6818a94aeb3facb2aa92b7933c94e392ffaed6ebd96cd8d`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:46:31 GMT
EXPOSE 5601
# Fri, 18 Mar 2022 01:46:52 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Fri, 18 Mar 2022 01:46:53 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Fri, 18 Mar 2022 01:46:54 GMT
RUN mkdir /usr/share/fonts/local
# Fri, 18 Mar 2022 01:46:56 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Fri, 18 Mar 2022 01:46:56 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Fri, 18 Mar 2022 01:46:57 GMT
RUN fc-cache -v
# Fri, 18 Mar 2022 01:47:33 GMT
COPY --chown=1000:0dir:57c1f98518da04d1a8be6b6dc127ee387ce746f092b9da5da9d47b31ccf9790f in /usr/share/kibana 
# Fri, 18 Mar 2022 01:47:37 GMT
WORKDIR /usr/share/kibana
# Fri, 18 Mar 2022 01:47:37 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Fri, 18 Mar 2022 01:47:38 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 18 Mar 2022 01:47:38 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 01:47:38 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Fri, 18 Mar 2022 01:47:38 GMT
COPY file:6c22337e28a5238c4691066da3ed9b35361d98a3f6f1ed3aef3b92ac54e5fa2b in /usr/local/bin/ 
# Fri, 18 Mar 2022 01:47:40 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Fri, 18 Mar 2022 01:47:41 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Fri, 18 Mar 2022 01:47:42 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Fri, 18 Mar 2022 01:47:42 GMT
LABEL org.label-schema.build-date=2022-03-18T01:37:25.152Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=0a94c82a3656a1600666ba9beb0f0b18ceb7464f org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.1.1 org.opencontainers.image.created=2022-03-18T01:37:25.152Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=0a94c82a3656a1600666ba9beb0f0b18ceb7464f org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.1.1
# Fri, 18 Mar 2022 01:47:42 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Fri, 18 Mar 2022 01:47:42 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Fri, 18 Mar 2022 01:47:43 GMT
USER kibana
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f2abe1b0ba05dc499de0fb39f5125e4cb72e75c0e3007015c2fe0aa8a02f8e`  
		Last Modified: Tue, 22 Mar 2022 20:43:21 GMT  
		Size: 10.8 MB (10765461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7603cc4bb6b761de8113b83daa8071138cc04b918b9c152e849a0bc27d24edaf`  
		Last Modified: Tue, 22 Mar 2022 20:43:15 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd5b340d32bf5d42791817ea9dd9b91a591bb8f0e21c77ded777bc256aa9009`  
		Last Modified: Tue, 22 Mar 2022 20:43:14 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c010e66f99432e7481608047b3f054d489d3bd6c413c91d4d157963fdf8f29`  
		Last Modified: Tue, 22 Mar 2022 20:43:32 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b5a2068f0d5860ca27729b49dbe7411c83ae4ee0f14a99919733c156a48da2`  
		Last Modified: Tue, 22 Mar 2022 20:43:09 GMT  
		Size: 5.3 KB (5287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc78166c84f684a305da58dbbecc4a43bf9ceb061998e35ab4977074d244f92`  
		Last Modified: Tue, 22 Mar 2022 20:45:28 GMT  
		Size: 274.9 MB (274857301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071216e6ad73cc0f2e440bf928716d435959f9ee75d068110375c98ed6107137`  
		Last Modified: Tue, 22 Mar 2022 20:43:09 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693f81de926fabf50169bc421f936a9574921a51a670acb157eb8f32aa8a70cf`  
		Last Modified: Tue, 22 Mar 2022 20:43:08 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792a46d541c358f63928c9653be01cd47d3e1e920092c40db2b1f7e93757548c`  
		Last Modified: Tue, 22 Mar 2022 20:43:03 GMT  
		Size: 4.2 KB (4221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fa5ab5c419786536709b27d4757960349f6519aa87221394d73526fb290739`  
		Last Modified: Tue, 22 Mar 2022 20:43:03 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2b954737d20c80b013db0c73e5abf4c496e2d0ca156ebee13a6a05d50e1549`  
		Last Modified: Tue, 22 Mar 2022 20:43:04 GMT  
		Size: 189.4 KB (189377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf377427786f73ea5bf4c47917dc7ee86594f951aee2c4c72b1a88b50f728ab`  
		Last Modified: Tue, 22 Mar 2022 20:43:03 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.1.1` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:bcf29b9dfb673d45a91320c38aed0d35addd8789a6868dae275a99662b0b8f51
```

-	Docker Version: 20.10.13
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.7 MB (343701337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6042a0a744655aa5ae7f98ee25c098646a5f5fb74fac7c1819bf54c3e68b116d`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:42:17 GMT
EXPOSE 5601
# Fri, 18 Mar 2022 01:42:34 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Fri, 18 Mar 2022 01:42:35 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Fri, 18 Mar 2022 01:42:36 GMT
RUN mkdir /usr/share/fonts/local
# Fri, 18 Mar 2022 01:42:38 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Fri, 18 Mar 2022 01:42:38 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Fri, 18 Mar 2022 01:42:39 GMT
RUN fc-cache -v
# Fri, 18 Mar 2022 01:43:39 GMT
COPY --chown=1000:0dir:2fbe21421462fa2d0cd0df4d2bfca5d98db7329e8f357d5a75cd728bedf541ee in /usr/share/kibana 
# Fri, 18 Mar 2022 01:43:42 GMT
WORKDIR /usr/share/kibana
# Fri, 18 Mar 2022 01:43:43 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Fri, 18 Mar 2022 01:43:43 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 18 Mar 2022 01:43:43 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 01:43:43 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Fri, 18 Mar 2022 01:43:43 GMT
COPY file:6c22337e28a5238c4691066da3ed9b35361d98a3f6f1ed3aef3b92ac54e5fa2b in /usr/local/bin/ 
# Fri, 18 Mar 2022 01:43:44 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Fri, 18 Mar 2022 01:43:46 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Fri, 18 Mar 2022 01:43:47 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Fri, 18 Mar 2022 01:43:47 GMT
LABEL org.label-schema.build-date=2022-03-18T01:38:30.094Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=0a94c82a3656a1600666ba9beb0f0b18ceb7464f org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.1.1 org.opencontainers.image.created=2022-03-18T01:38:30.094Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=0a94c82a3656a1600666ba9beb0f0b18ceb7464f org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.1.1
# Fri, 18 Mar 2022 01:43:47 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Fri, 18 Mar 2022 01:43:47 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Fri, 18 Mar 2022 01:43:47 GMT
USER kibana
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c6b5885c18057d11de374ab888d02701251b69f5574cb9b567769c4ba7b1d7`  
		Last Modified: Thu, 24 Mar 2022 02:07:25 GMT  
		Size: 10.4 MB (10384627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9b79d32060bd9b3d43cdf2969743d13018a78e17f718c5159d35263134c491`  
		Last Modified: Thu, 24 Mar 2022 02:07:23 GMT  
		Size: 9.1 KB (9092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db5c87897f3a70bbce469ad953f028a1b6e4a891fb66716ca6ba98f748a62b9`  
		Last Modified: Thu, 24 Mar 2022 02:07:21 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443f1fae9e6e3c29e27d135a4ad77d4f439141fb38ac1e4f4d841041d68f7e25`  
		Last Modified: Thu, 24 Mar 2022 02:07:22 GMT  
		Size: 16.5 MB (16460475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe9142fc44759a42ce78f8fbef080dbea0bcd6197e3619d830b31d8f8a57286`  
		Last Modified: Thu, 24 Mar 2022 02:07:21 GMT  
		Size: 5.3 KB (5283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d707b606f8c9ab8ba06c07068151f40203895a2e2fd84e5e6daad0ba07ad23b8`  
		Last Modified: Thu, 24 Mar 2022 02:07:59 GMT  
		Size: 289.5 MB (289481708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6726a77ae119576b7766b683d0da7392a66d5cf0be45d72ac6ca52c35767cfc8`  
		Last Modified: Thu, 24 Mar 2022 02:07:20 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6549d875614775b6a567d9e985ca7a8a74f2d1cc313ccf3835e9ac8c7801a259`  
		Last Modified: Thu, 24 Mar 2022 02:07:18 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530edb184ce409886b09be0b3b14ac4f95b6532b2dfc719b95e82fc7d3c9d470`  
		Last Modified: Thu, 24 Mar 2022 02:07:18 GMT  
		Size: 4.2 KB (4218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f9e364beda04f22f2001b21b3d716149a33833209853d1b12f32bd1e1cf160`  
		Last Modified: Thu, 24 Mar 2022 02:07:18 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba8e4f092c7be071b229f43d2237fa83e11fde29624216b4efc8304d9de0f94`  
		Last Modified: Thu, 24 Mar 2022 02:07:18 GMT  
		Size: 183.4 KB (183384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cebc0be666756d186dd511b75741d6f662ee208653cd22cecde5b3e34a74530`  
		Last Modified: Thu, 24 Mar 2022 02:07:18 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
