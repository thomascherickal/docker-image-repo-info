<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.23`](#kibana6823)
-	[`kibana:7.17.2`](#kibana7172)
-	[`kibana:8.1.2`](#kibana812)

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

## `kibana:7.17.2`

```console
$ docker pull kibana@sha256:214302162d75a7c8ade156b3298f3e12ba275bc537503109f13a8caac33fbef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.17.2` - linux; amd64

```console
$ docker pull kibana@sha256:0b3778350b5cb12f33f4c520939c1eba9d8997a70b827a9786abf4011dd82012
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343040762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19591c8c1eb3bf5b464ac5741c9828faac07812ba8486cc3a6bb2555722e8a4c`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Mon, 28 Mar 2022 09:35:07 GMT
EXPOSE 5601
# Mon, 28 Mar 2022 09:35:25 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Mon, 28 Mar 2022 09:35:26 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Mon, 28 Mar 2022 09:35:27 GMT
RUN mkdir /usr/share/fonts/local
# Mon, 28 Mar 2022 09:35:28 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Mon, 28 Mar 2022 09:35:29 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Mon, 28 Mar 2022 09:35:30 GMT
RUN fc-cache -v
# Mon, 28 Mar 2022 09:36:03 GMT
COPY --chown=1000:0dir:80b1751364f9b0590783599a5cd396d79f4f23da8572b38a0e784af55a3f96db in /usr/share/kibana 
# Mon, 28 Mar 2022 09:36:09 GMT
WORKDIR /usr/share/kibana
# Mon, 28 Mar 2022 09:36:10 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Mon, 28 Mar 2022 09:36:10 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 28 Mar 2022 09:36:10 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 28 Mar 2022 09:36:10 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Mon, 28 Mar 2022 09:36:10 GMT
COPY file:64ce3ba9275bed6c9214b200cd3b7913d52068df7094bee2baccc5b713d391f7 in /usr/local/bin/ 
# Mon, 28 Mar 2022 09:36:12 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Mon, 28 Mar 2022 09:36:13 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Mon, 28 Mar 2022 09:36:14 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Mon, 28 Mar 2022 09:36:14 GMT
LABEL org.label-schema.build-date=2022-03-28T08:38:19.218Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=07cff2b713ccaea7caa78c054848de6cc2ba0331 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.2 org.opencontainers.image.created=2022-03-28T08:38:19.218Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=07cff2b713ccaea7caa78c054848de6cc2ba0331 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.2
# Mon, 28 Mar 2022 09:36:14 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 28 Mar 2022 09:36:15 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Mon, 28 Mar 2022 09:36:15 GMT
USER kibana
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfa92e782fa0e7f9f6146d6168427935a07677fc00a9e7a42bc685414e54276`  
		Last Modified: Fri, 01 Apr 2022 21:01:55 GMT  
		Size: 10.5 MB (10514814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e475533f4b392d3273e2d6788763a231ee47e3240f77dc343b8c0758ad084b`  
		Last Modified: Fri, 01 Apr 2022 21:01:53 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce5af872cfd6944e1d8a2534e320251c11724697afe456906c8d167dac7cbe`  
		Last Modified: Fri, 01 Apr 2022 21:01:50 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436799be3926a4bbd4b90ad9d53b9866f68d6d31141e9615e3ae35ca0bf0babb`  
		Last Modified: Fri, 01 Apr 2022 21:01:52 GMT  
		Size: 16.5 MB (16460481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770503d8e3ad98ab910ffd5676cfa85beca172b2bf2ddea86ccb5220432fe6d7`  
		Last Modified: Fri, 01 Apr 2022 21:01:50 GMT  
		Size: 5.3 KB (5276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b1639d81b78e4925c921e1ad65ce1f4ffc5c47dd4b847e84198de863fd2c1`  
		Last Modified: Fri, 01 Apr 2022 21:02:25 GMT  
		Size: 287.3 MB (287287933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda94123f6411d80f3b04b948e6ae5a8f4549fa1774a23daf39f377edfb7b74d`  
		Last Modified: Fri, 01 Apr 2022 21:01:50 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b44c0933f43b8c031b46b179151220ba4f994a2e19cf18a8949eb5bea89c7b7`  
		Last Modified: Fri, 01 Apr 2022 21:01:48 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f984d55c676b2eb9f76846a6a200e6a618bbaac061a41bf4bc56c54a83dea17`  
		Last Modified: Fri, 01 Apr 2022 21:01:48 GMT  
		Size: 4.5 KB (4498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9192321c02111dd630d006f765190ab128d0a71e2d26dbf6fcb9fcec30fbf177`  
		Last Modified: Fri, 01 Apr 2022 21:01:48 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8dc20e0401cb70367456d7818f645d9677da65b99b2f71cf5dd48a682112cb`  
		Last Modified: Fri, 01 Apr 2022 21:01:48 GMT  
		Size: 189.4 KB (189381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de49a43c45f58a711c36a6a544b6ff5444458e90616e550c4bd8249a879ad41`  
		Last Modified: Fri, 01 Apr 2022 21:01:48 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.17.2` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:76e943a46226882917fa294d9384c97a50ed88d9100f128a9af2726525b4c093
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.1 MB (356116796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e33ba540bb55fe5ba63ec8f41bf6324cc777d8c0ddbac4662327caecfde1ec`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Mon, 28 Mar 2022 16:12:44 GMT
EXPOSE 5601
# Mon, 28 Mar 2022 16:13:00 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Mon, 28 Mar 2022 16:13:01 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Mon, 28 Mar 2022 16:13:02 GMT
RUN mkdir /usr/share/fonts/local
# Mon, 28 Mar 2022 16:13:03 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Mon, 28 Mar 2022 16:13:04 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Mon, 28 Mar 2022 16:13:04 GMT
RUN fc-cache -v
# Mon, 28 Mar 2022 16:13:31 GMT
COPY --chown=1000:0dir:f00fd4140e9fffc4c90b7268eb30ca830834c0bb88ba8c86d8057ace28326dcc in /usr/share/kibana 
# Mon, 28 Mar 2022 16:13:35 GMT
WORKDIR /usr/share/kibana
# Mon, 28 Mar 2022 16:13:35 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Mon, 28 Mar 2022 16:13:35 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 28 Mar 2022 16:13:36 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 28 Mar 2022 16:13:36 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Mon, 28 Mar 2022 16:13:36 GMT
COPY file:64ce3ba9275bed6c9214b200cd3b7913d52068df7094bee2baccc5b713d391f7 in /usr/local/bin/ 
# Mon, 28 Mar 2022 16:13:37 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Mon, 28 Mar 2022 16:13:38 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Mon, 28 Mar 2022 16:13:39 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Mon, 28 Mar 2022 16:13:39 GMT
LABEL org.label-schema.build-date=2022-03-28T16:09:26.081Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=07cff2b713ccaea7caa78c054848de6cc2ba0331 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.2 org.opencontainers.image.created=2022-03-28T16:09:26.081Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=07cff2b713ccaea7caa78c054848de6cc2ba0331 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.2
# Mon, 28 Mar 2022 16:13:39 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 28 Mar 2022 16:13:39 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Mon, 28 Mar 2022 16:13:39 GMT
USER kibana
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90420d71e5a9b13638ff7abfd1fe8f62361a43393e5403acb50a50c843d2b828`  
		Last Modified: Fri, 01 Apr 2022 19:19:23 GMT  
		Size: 10.4 MB (10384773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b86450a38b4bd353d12a34a97d3b55cf1404a02f58e98303a3abcf67d5000c2`  
		Last Modified: Fri, 01 Apr 2022 19:19:22 GMT  
		Size: 9.1 KB (9097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b010dc16a1e0965694c114cf158be6968000b04d0609cc347c18ed7b62c19ea8`  
		Last Modified: Fri, 01 Apr 2022 19:19:19 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2d7e4aae9e5db9a24858500fe0f3fb841664b208134112a4defb7812161fc`  
		Last Modified: Fri, 01 Apr 2022 19:19:21 GMT  
		Size: 16.5 MB (16460483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8032c6eaf309729ad33e12b72042a6940d5d5e1591b8c5c84270be544958e86a`  
		Last Modified: Fri, 01 Apr 2022 19:19:19 GMT  
		Size: 5.3 KB (5285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041bb3b625a5d4d0607e8ca861c266d82172598e3e4d0c4dec0c4afe51d276ef`  
		Last Modified: Fri, 01 Apr 2022 19:20:00 GMT  
		Size: 301.9 MB (301896712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebc23d87e1bb2b3e4dc906728013fe7793bd52cad85321564ab6ccb21e18a18`  
		Last Modified: Fri, 01 Apr 2022 19:19:19 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26de705d4d501e2a8645c9bb109d3f74acaee4f3498da8e2ad5543d9d262a24e`  
		Last Modified: Fri, 01 Apr 2022 19:19:17 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87385cda2e87fda72518493df2b0c5cb995c0705fbbe2e4b85aa1ee0c380399`  
		Last Modified: Fri, 01 Apr 2022 19:19:17 GMT  
		Size: 4.5 KB (4494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f2bdb13aba4b2c1241d541ea55120da27bcad90acabe5eb559665e47f40500`  
		Last Modified: Fri, 01 Apr 2022 19:19:17 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5579e6fc4803b34e14fa14e61222338c5f7b04a0459044867ef8be078e9b6d`  
		Last Modified: Fri, 01 Apr 2022 19:19:17 GMT  
		Size: 183.4 KB (183389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4547ad518c5f1283cc4eb5d356471012644868140bc2af5cc1fedcf4f329cc1`  
		Last Modified: Fri, 01 Apr 2022 19:19:17 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.1.2`

```console
$ docker pull kibana@sha256:16522ca04a01c252ff4785f0c8102178995d3bc31bb4302abc49903623fad3b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.1.2` - linux; amd64

```console
$ docker pull kibana@sha256:910877448e030abf0ab87600739c064d189f57a3528d6d1ad789a6060cd2c28d
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.1 MB (331070408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6d3a3c39d21f2ef0aaba278e54a7f3a057f8939fe95d95c53fbe613d89cc946`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:01:53 GMT
EXPOSE 5601
# Wed, 30 Mar 2022 01:02:11 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Wed, 30 Mar 2022 01:02:12 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Wed, 30 Mar 2022 01:02:12 GMT
RUN mkdir /usr/share/fonts/local
# Wed, 30 Mar 2022 01:02:14 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Wed, 30 Mar 2022 01:02:15 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Wed, 30 Mar 2022 01:02:15 GMT
RUN fc-cache -v
# Wed, 30 Mar 2022 01:02:51 GMT
COPY --chown=1000:0dir:84cb0d87e91d8a1848132996023e50982d7b1d5c6c29b05de61647730db3d2f5 in /usr/share/kibana 
# Wed, 30 Mar 2022 01:02:57 GMT
WORKDIR /usr/share/kibana
# Wed, 30 Mar 2022 01:02:57 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Wed, 30 Mar 2022 01:02:57 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 30 Mar 2022 01:02:58 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 01:02:58 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Wed, 30 Mar 2022 01:02:58 GMT
COPY file:7c7c9d2b7fd3a7bac99ec2cc74e9f55d2255b807334a4eb61596a05358fbcde2 in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:02:59 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Wed, 30 Mar 2022 01:03:01 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Wed, 30 Mar 2022 01:03:02 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Wed, 30 Mar 2022 01:03:02 GMT
LABEL org.label-schema.build-date=2022-03-30T00:51:54.148Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=0f6d770b4febdce2134bcadc34959b96cbac8ecc org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.1.2 org.opencontainers.image.created=2022-03-30T00:51:54.148Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=0f6d770b4febdce2134bcadc34959b96cbac8ecc org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.1.2
# Wed, 30 Mar 2022 01:03:02 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 30 Mar 2022 01:03:02 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Wed, 30 Mar 2022 01:03:02 GMT
USER kibana
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291e5777a2bd607062d09034e9a91e60c2b42a8d863f118180bcf130f0ffea02`  
		Last Modified: Thu, 31 Mar 2022 18:38:17 GMT  
		Size: 10.5 MB (10514819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c22eae527e2c2f472dbb9b987985c1c407890f10c72232ea10e9b9f5623c97`  
		Last Modified: Thu, 31 Mar 2022 18:38:14 GMT  
		Size: 9.5 KB (9530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6196de944c08da7944945d562c8bb4e880b72a8c59d58e1c433dce5a8e5029b`  
		Last Modified: Thu, 31 Mar 2022 18:38:12 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda09de2e6d9f57134ccd9b7a47fbb47d49c5789aadcf1ddc49e125834b0d152`  
		Last Modified: Thu, 31 Mar 2022 18:38:14 GMT  
		Size: 16.5 MB (16460488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3280e2473d8a7d5f998b4b4e59fc21ae3b606216e3316133eeebf05482ba5cad`  
		Last Modified: Thu, 31 Mar 2022 18:38:11 GMT  
		Size: 5.3 KB (5275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9158bc45d8e5ad3838528895cd68511ed3d44ff38069a31b1091d6861c59daef`  
		Last Modified: Thu, 31 Mar 2022 18:39:09 GMT  
		Size: 275.3 MB (275317835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5df2a7a04bee78808533b6baf466998e63f05b77c7ec70826b601ecc7d5567`  
		Last Modified: Thu, 31 Mar 2022 18:38:10 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9e857b1bc0dea85d964fe22d46f1b8245b40153c39c78d4c7d89708b855afc`  
		Last Modified: Thu, 31 Mar 2022 18:38:07 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532decaedde01bef28734cbebcfc92167d280713524ddbb0df836c0deb959be1`  
		Last Modified: Thu, 31 Mar 2022 18:38:08 GMT  
		Size: 4.2 KB (4235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a333b837eda5249e43d7ca60a54aa5c7785bb5b552ea7097720f9be5a29ec1`  
		Last Modified: Thu, 31 Mar 2022 18:38:07 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e079c6ae4739c71b477cc73b36362246bae32b0cc770a4bb9069e031b641802d`  
		Last Modified: Thu, 31 Mar 2022 18:38:07 GMT  
		Size: 189.4 KB (189381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b546d180979b60760cdab9f9c42c7af8985ef0a116da1b26a0abe77f688bad`  
		Last Modified: Thu, 31 Mar 2022 18:38:06 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.1.2` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:fa97a5ab79e6cbc8032aea3d795ba795afcd963fa99af73b939fd64c678cc5de
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.2 MB (344169650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca3b6b0e710589d1cc665502379f7ac42edeb871d7f0b353399f17d4925225be`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 00:57:20 GMT
EXPOSE 5601
# Wed, 30 Mar 2022 00:57:37 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Wed, 30 Mar 2022 00:57:38 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Wed, 30 Mar 2022 00:57:38 GMT
RUN mkdir /usr/share/fonts/local
# Wed, 30 Mar 2022 00:57:41 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Wed, 30 Mar 2022 00:57:41 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Wed, 30 Mar 2022 00:57:42 GMT
RUN fc-cache -v
# Wed, 30 Mar 2022 00:58:12 GMT
COPY --chown=1000:0dir:d0da4fd329a6480a81a15946172333fd610883402a4f9d3dd40a9a67ab250010 in /usr/share/kibana 
# Wed, 30 Mar 2022 00:58:14 GMT
WORKDIR /usr/share/kibana
# Wed, 30 Mar 2022 00:58:15 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Wed, 30 Mar 2022 00:58:15 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 30 Mar 2022 00:58:15 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 00:58:15 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Wed, 30 Mar 2022 00:58:15 GMT
COPY file:7c7c9d2b7fd3a7bac99ec2cc74e9f55d2255b807334a4eb61596a05358fbcde2 in /usr/local/bin/ 
# Wed, 30 Mar 2022 00:58:16 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Wed, 30 Mar 2022 00:58:18 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Wed, 30 Mar 2022 00:58:18 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Wed, 30 Mar 2022 00:58:18 GMT
LABEL org.label-schema.build-date=2022-03-30T00:53:34.746Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=0f6d770b4febdce2134bcadc34959b96cbac8ecc org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.1.2 org.opencontainers.image.created=2022-03-30T00:53:34.746Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=0f6d770b4febdce2134bcadc34959b96cbac8ecc org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.1.2
# Wed, 30 Mar 2022 00:58:18 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 30 Mar 2022 00:58:19 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Wed, 30 Mar 2022 00:58:19 GMT
USER kibana
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e26dd8c6299fbde3d9e7bd33ccd11cf0dfe241ccfa4917a4d7fa43498c52719`  
		Last Modified: Fri, 01 Apr 2022 19:18:27 GMT  
		Size: 10.4 MB (10384670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172751e6b118fac21d8a166423050ab8202144d1fc1f4e6beb84bcac92a56d0c`  
		Last Modified: Fri, 01 Apr 2022 19:18:26 GMT  
		Size: 9.1 KB (9101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292f42cbd5cd000ee9f6992fc99a1c47006417be1b0f96a0fbae6b6a48fe179e`  
		Last Modified: Fri, 01 Apr 2022 19:18:24 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cc295a8a0266b906b446ce019c6ececa98d352d4f08861eaeb2ce7539945d`  
		Last Modified: Fri, 01 Apr 2022 19:18:25 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0f1fe1546d504b8652669b19b138c5ce02ca2718e3f147bd8cb2dcf699e735`  
		Last Modified: Fri, 01 Apr 2022 19:18:23 GMT  
		Size: 5.3 KB (5275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46c456f0d8c6a98b5e2dcf9498f0b9d5a0047bbb576c4ddcfb9b2c390884094`  
		Last Modified: Fri, 01 Apr 2022 19:19:02 GMT  
		Size: 289.9 MB (289949935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0517227f65216b18af40e432c15e2aec6e79362ed5b7a7b0cf357d2858f29d`  
		Last Modified: Fri, 01 Apr 2022 19:18:23 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ab5efc71052ddb8f020278b8ad16dfbb492084c43d62c25a48d6fd3840b367`  
		Last Modified: Fri, 01 Apr 2022 19:18:21 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f76a657458fa94bcd8094f723e0f70e8d0c32ec582e6250adf9233f630257`  
		Last Modified: Fri, 01 Apr 2022 19:18:21 GMT  
		Size: 4.2 KB (4234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c99ac9eb28b5e21032faff2847e26b855e1404cd4f00ec4e760bcc511628b37`  
		Last Modified: Fri, 01 Apr 2022 19:18:21 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acc6d4b5f77d7f752cd5799db69aed80a08785bdc3b6545466eaef9986bea12`  
		Last Modified: Fri, 01 Apr 2022 19:18:21 GMT  
		Size: 183.4 KB (183386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0705a4d225f0d4572755c5e0b8e0b6910d544b4c4868fa50ead51dc308dae8`  
		Last Modified: Fri, 01 Apr 2022 19:18:21 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
