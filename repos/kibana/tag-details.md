<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.23`](#kibana6823)
-	[`kibana:7.17.1`](#kibana7171)
-	[`kibana:8.1.0`](#kibana810)

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

## `kibana:8.1.0`

```console
$ docker pull kibana@sha256:003735391b570d705e3cb5b492c0677808787fbec0eb1dbca4b120834be12677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.1.0` - linux; amd64

```console
$ docker pull kibana@sha256:792a533420c35b99fb7879335b0bf9e4c3f62a3f5bb068903f06393441fc7e8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339722472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f13dbb88b03e520263e2b946250a440d7479dcc29d6c44ef0a3bfddcf2dce6`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 18:11:17 GMT
EXPOSE 5601
# Thu, 03 Mar 2022 18:11:43 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Thu, 03 Mar 2022 18:11:45 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Thu, 03 Mar 2022 18:11:45 GMT
RUN mkdir /usr/share/fonts/local
# Thu, 03 Mar 2022 18:11:47 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Thu, 03 Mar 2022 18:11:47 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Thu, 03 Mar 2022 18:11:48 GMT
RUN fc-cache -v
# Thu, 03 Mar 2022 18:12:22 GMT
COPY --chown=1000:0dir:eda4d8b61b932bdb964513de45167d72253f7ed4c08a6674e34427358966ed96 in /usr/share/kibana 
# Thu, 03 Mar 2022 18:12:27 GMT
WORKDIR /usr/share/kibana
# Thu, 03 Mar 2022 18:12:28 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 03 Mar 2022 18:12:28 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 03 Mar 2022 18:12:28 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 18:12:28 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Thu, 03 Mar 2022 18:12:28 GMT
COPY file:6c22337e28a5238c4691066da3ed9b35361d98a3f6f1ed3aef3b92ac54e5fa2b in /usr/local/bin/ 
# Thu, 03 Mar 2022 18:12:30 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 03 Mar 2022 18:12:31 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Thu, 03 Mar 2022 18:12:32 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Thu, 03 Mar 2022 18:12:32 GMT
LABEL org.label-schema.build-date=2022-03-03T18:00:43.075Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=4aaeda23aea9c3bf29698878c70a0107ea3c1659 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.1.0 org.opencontainers.image.created=2022-03-03T18:00:43.075Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=4aaeda23aea9c3bf29698878c70a0107ea3c1659 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.1.0
# Thu, 03 Mar 2022 18:12:32 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 03 Mar 2022 18:12:32 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 03 Mar 2022 18:12:32 GMT
USER kibana
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e718cec2b0e862dde93aa030e776eea4f07d31cfe9e7e3b56bde86fc4267e5`  
		Last Modified: Wed, 09 Mar 2022 08:52:37 GMT  
		Size: 19.7 MB (19676393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84faaf974d0b2f0a7b8cfd078d6cd07f2da8cf0083778e2ddd57abb3a2c636bd`  
		Last Modified: Wed, 09 Mar 2022 08:52:34 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73acb5a127b3b8bb5bab6b73d7c362ad6795e9f677d9b6cc9b5bd89a4e4f9606`  
		Last Modified: Wed, 09 Mar 2022 08:52:33 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f1f6b9f8a9e5dc4f7ba5f6c05648cab9bfa4c046e38ae79d0d86c4fe89a36e`  
		Last Modified: Wed, 09 Mar 2022 08:52:33 GMT  
		Size: 16.5 MB (16460488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01667ff426500e158d0e8d40e0e49cf5cc65fe8f7de96ab6a00882fa3ac9296`  
		Last Modified: Wed, 09 Mar 2022 08:52:31 GMT  
		Size: 5.3 KB (5280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98b82a9a0682420e30c5e1104cddb10ef4acfb05434d3efb5d3e88c5cd5d611`  
		Last Modified: Wed, 09 Mar 2022 08:52:56 GMT  
		Size: 274.8 MB (274810133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b405faf931d2b477a936a14f5feaefdc2a032cb5f92b137aa28860d3866407`  
		Last Modified: Wed, 09 Mar 2022 08:52:31 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf18d3cd4cb7af6204b7bbfbf4f36bc8042ec605f018483b544dde10a5a63fe`  
		Last Modified: Wed, 09 Mar 2022 08:52:28 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3be697f6b7dfb7bac08c47294d4c0abcff36872b22920ec187cdfcdad6672`  
		Last Modified: Wed, 09 Mar 2022 08:52:28 GMT  
		Size: 4.2 KB (4222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666c2b7f70ac15a87902681a5ae98d63764ed2ec2f5720faaa42f375d290fe44`  
		Last Modified: Wed, 09 Mar 2022 08:52:28 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361c85070bd3a5eab4dbeacfb97894eaf84687aaf6451bea92ef22f47093c39a`  
		Last Modified: Wed, 09 Mar 2022 08:52:29 GMT  
		Size: 189.4 KB (189383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc68aaf7c079a428e9752cef42a5f8098a4abc77697d0ea5a298ebc1f954a286`  
		Last Modified: Wed, 09 Mar 2022 08:52:28 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.1.0` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:0e217fee78825de6ef6b2bb06526909e74a60718fcc3d4a5f1e36b6c427c006d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.7 MB (351707191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e791db908920da3644b8deabe0c1659598c2432461e6f1c81bf588adc4861f8e`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 18:07:24 GMT
EXPOSE 5601
# Thu, 03 Mar 2022 18:07:47 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Thu, 03 Mar 2022 18:07:48 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Thu, 03 Mar 2022 18:07:49 GMT
RUN mkdir /usr/share/fonts/local
# Thu, 03 Mar 2022 18:07:51 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Thu, 03 Mar 2022 18:07:51 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Thu, 03 Mar 2022 18:07:52 GMT
RUN fc-cache -v
# Thu, 03 Mar 2022 18:08:26 GMT
COPY --chown=1000:0dir:d770c9250aac5a4363660e967c293f072507d12865e920e739b2e814ed32857b in /usr/share/kibana 
# Thu, 03 Mar 2022 18:08:30 GMT
WORKDIR /usr/share/kibana
# Thu, 03 Mar 2022 18:08:31 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 03 Mar 2022 18:08:31 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 03 Mar 2022 18:08:31 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 18:08:31 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Thu, 03 Mar 2022 18:08:31 GMT
COPY file:6c22337e28a5238c4691066da3ed9b35361d98a3f6f1ed3aef3b92ac54e5fa2b in /usr/local/bin/ 
# Thu, 03 Mar 2022 18:08:32 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 03 Mar 2022 18:08:34 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Thu, 03 Mar 2022 18:08:35 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Thu, 03 Mar 2022 18:08:35 GMT
LABEL org.label-schema.build-date=2022-03-03T18:03:03.013Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=4aaeda23aea9c3bf29698878c70a0107ea3c1659 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.1.0 org.opencontainers.image.created=2022-03-03T18:03:03.013Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=4aaeda23aea9c3bf29698878c70a0107ea3c1659 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.1.0
# Thu, 03 Mar 2022 18:08:35 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 03 Mar 2022 18:08:35 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 03 Mar 2022 18:08:35 GMT
USER kibana
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1556a4295c5a9506ebfd2a7c333ecf19f3d91a738bed4f2413dccc944ca6348`  
		Last Modified: Wed, 09 Mar 2022 21:41:41 GMT  
		Size: 18.4 MB (18422647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1e61d27c40f7ad0dbca5f178ac7659a80acbce498e80f0dd25ee66c49130b3`  
		Last Modified: Wed, 09 Mar 2022 21:41:39 GMT  
		Size: 9.1 KB (9097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858a19c5041a23894c31ba43d5de6e305c1e7e248e95ad26dbcfcd9950d8fa6a`  
		Last Modified: Wed, 09 Mar 2022 21:41:36 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb828bbedd0c1b8695b73ed54987144e9ef769837f507950488823567643e73`  
		Last Modified: Wed, 09 Mar 2022 21:41:38 GMT  
		Size: 16.5 MB (16460481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795687a45b7359764b2d35b8238a49f69eb0c2b1d55836500931bfb2bc08730e`  
		Last Modified: Wed, 09 Mar 2022 21:41:36 GMT  
		Size: 5.3 KB (5289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1e4ea52e03f118dd82a875ab74fa16aca5ef3f96031a361cdb7a43fa2d4672`  
		Last Modified: Wed, 09 Mar 2022 21:42:15 GMT  
		Size: 289.4 MB (289449472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b58f86ebb59acc5e74571b5b8cade21e37b56ab77e9142fe594d23a54e7b709`  
		Last Modified: Wed, 09 Mar 2022 21:41:36 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf84f7c72c93de3dfdad81e2c5afdbc54a0ad26f94c8677afad49b1d20bc021`  
		Last Modified: Wed, 09 Mar 2022 21:41:33 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f101511dcf65a5557771e73ced422c88315916e470d8d85fb38fc8dce1588be`  
		Last Modified: Wed, 09 Mar 2022 21:41:33 GMT  
		Size: 4.2 KB (4223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0598e3df5eed13405cb3613dac5950f4880d0ad048fddee81d812b9a0c5ef1`  
		Last Modified: Wed, 09 Mar 2022 21:41:33 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24432c918f740af4689e0caa82f4bf1a7798c1df7739aae4f21a092c4820ef34`  
		Last Modified: Wed, 09 Mar 2022 21:41:33 GMT  
		Size: 183.4 KB (183389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01a76ba92ca66d6c6b249b9bc15639bbc87b3663fd6f6e8a9750d6320cd7ca1`  
		Last Modified: Wed, 09 Mar 2022 21:41:33 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
