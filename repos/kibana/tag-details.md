<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.9`](#kibana7179)
-	[`kibana:8.7.0`](#kibana870)

## `kibana:7.17.9`

```console
$ docker pull kibana@sha256:69f04843b05fb3cf26ec8c06cd36d560e0bca9ce41e6886c807d865b7ea618e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.17.9` - linux; amd64

```console
$ docker pull kibana@sha256:aefb8ca90b82030e22037a957dee4bff9236eea235324375f19e8922eaa20502
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.2 MB (329196799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0059eed7da920704796ce2bb872e83155821f9a64fc634274d1e9f8cc23e22`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Mon, 30 Jan 2023 12:43:38 GMT
EXPOSE map[5601/tcp:{}]
# Mon, 30 Jan 2023 12:43:38 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Mon, 30 Jan 2023 12:43:39 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Mon, 30 Jan 2023 12:43:40 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Mon, 30 Jan 2023 12:43:40 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Mon, 30 Jan 2023 12:43:41 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Mon, 30 Jan 2023 12:43:41 GMT
RUN fc-cache -v # buildkit
# Mon, 30 Jan 2023 12:44:32 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Mon, 30 Jan 2023 12:44:32 GMT
WORKDIR /usr/share/kibana
# Mon, 30 Jan 2023 12:44:33 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Mon, 30 Jan 2023 12:44:33 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 30 Jan 2023 12:44:33 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Jan 2023 12:44:33 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Mon, 30 Jan 2023 12:44:33 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Mon, 30 Jan 2023 12:44:33 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Mon, 30 Jan 2023 12:44:34 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Mon, 30 Jan 2023 12:44:34 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Mon, 30 Jan 2023 12:44:34 GMT
LABEL org.label-schema.build-date=2023-01-30T12:17:55.756Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=00b0b0440dbf6f8c542448473e020c99d352a0f5 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.9 org.opencontainers.image.created=2023-01-30T12:17:55.756Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=00b0b0440dbf6f8c542448473e020c99d352a0f5 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.9
# Mon, 30 Jan 2023 12:44:34 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 30 Jan 2023 12:44:34 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Mon, 30 Jan 2023 12:44:34 GMT
USER kibana
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144df3972ed5731ddb73eedaa8175c38669f8733ffb422a4323513f0d44f71ba`  
		Last Modified: Tue, 07 Feb 2023 20:44:30 GMT  
		Size: 10.9 MB (10906819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee71c9917ce20f4dbee2249dea74ade95868679cfd52b5f03fa2840d5e30db3`  
		Last Modified: Tue, 07 Feb 2023 20:44:27 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb0c544b6b907f0514d9c683562908bca16da597f718e00213f669011b2cb2b`  
		Last Modified: Tue, 07 Feb 2023 20:44:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fdf76384b609c053725de172048895872be3940fb183653f5a828b8c165dcc`  
		Last Modified: Tue, 07 Feb 2023 20:44:27 GMT  
		Size: 16.5 MB (16460475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed11a68cbb9ec5d6759be8fb4fc4c3c1cba9a5ae575222c87c8b16e7c706f61`  
		Last Modified: Tue, 07 Feb 2023 20:44:23 GMT  
		Size: 5.3 KB (5296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90cf8802e3328f4006c3893cd1fe84ab5de0628bcc226d8aa8550f809903def`  
		Last Modified: Tue, 07 Feb 2023 20:45:14 GMT  
		Size: 273.0 MB (273040936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742662fee0f03cf5f5d8033ddea5645d2edf53a1e5bb4435c58d646a192af976`  
		Last Modified: Tue, 07 Feb 2023 20:44:23 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf74473cf818dbb8962a37a1dcb95e9c8a3f8fad10ae4b3b7b5fa5ebfa5cbb4`  
		Last Modified: Tue, 07 Feb 2023 20:44:23 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae97ce5d6732c6a7bdc0163a67625da75a8aaf77ebf32edaf598f9e8a1494e3`  
		Last Modified: Tue, 07 Feb 2023 20:44:23 GMT  
		Size: 4.5 KB (4505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abdf7b4ef80863e971dc65d278754db5234e6a094aa9b0e3dcf5b336a9b07a4`  
		Last Modified: Tue, 07 Feb 2023 20:44:21 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d01537b7d629fdbc3b6dc57a054b9aa96ee80ae82f5e033d8430266764403b`  
		Last Modified: Tue, 07 Feb 2023 20:44:21 GMT  
		Size: 189.4 KB (189391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f8c3eee3b1d20a9d5984f01a5f49bc0ddf13326997445a905fa0857f548a46`  
		Last Modified: Tue, 07 Feb 2023 20:44:21 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.17.9` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:33a858d7b002ca0dc15e0f26ce18567c3ffbfe2c5829dd94b7bb42536df89ce5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.1 MB (344107968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d71855e558ed8d7ca1dfc89490143dcadd482df2ee70398863b18ef11fd85cf`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Mon, 30 Jan 2023 12:46:34 GMT
EXPOSE map[5601/tcp:{}]
# Mon, 30 Jan 2023 12:46:34 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Mon, 30 Jan 2023 12:46:36 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Mon, 30 Jan 2023 12:46:36 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Mon, 30 Jan 2023 12:46:39 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Mon, 30 Jan 2023 12:46:39 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Mon, 30 Jan 2023 12:46:40 GMT
RUN fc-cache -v # buildkit
# Mon, 30 Jan 2023 12:47:30 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Mon, 30 Jan 2023 12:47:30 GMT
WORKDIR /usr/share/kibana
# Mon, 30 Jan 2023 12:47:30 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Mon, 30 Jan 2023 12:47:30 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 30 Jan 2023 12:47:30 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Jan 2023 12:47:31 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Mon, 30 Jan 2023 12:47:31 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Mon, 30 Jan 2023 12:47:31 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Mon, 30 Jan 2023 12:47:32 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Mon, 30 Jan 2023 12:47:33 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Mon, 30 Jan 2023 12:47:33 GMT
LABEL org.label-schema.build-date=2023-01-30T12:17:55.756Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=00b0b0440dbf6f8c542448473e020c99d352a0f5 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.9 org.opencontainers.image.created=2023-01-30T12:17:55.756Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=00b0b0440dbf6f8c542448473e020c99d352a0f5 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.9
# Mon, 30 Jan 2023 12:47:33 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 30 Jan 2023 12:47:33 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Mon, 30 Jan 2023 12:47:33 GMT
USER kibana
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacab5eee6d97ad288bcac89d5d41ce8543a839d2adec5064b5b9067644aef29`  
		Last Modified: Tue, 07 Feb 2023 22:57:17 GMT  
		Size: 10.8 MB (10768381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebdd3887fd1a28b41bbe597dbe690527176cb44a98c34976352a82c164536bd`  
		Last Modified: Tue, 07 Feb 2023 22:57:15 GMT  
		Size: 9.1 KB (9099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64a8b693a1a9f7e25477637e4a119cc9a75168f326e60c228b4da27e0f17332`  
		Last Modified: Tue, 07 Feb 2023 22:57:14 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d17e555a88d6e5d0b72515ee9c0b3bc44c4787e9d64a0307d457e7bab620e20`  
		Last Modified: Tue, 07 Feb 2023 22:57:15 GMT  
		Size: 16.5 MB (16460476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e70368d00a87c7cd3a307fedd180221ac5425754e1b33290ad59dcc1c62c118`  
		Last Modified: Tue, 07 Feb 2023 22:57:14 GMT  
		Size: 5.3 KB (5290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027bfdb93caa1ced65cc512ae065a682b899bf3a9072c327d63a2d18955bef2e`  
		Last Modified: Tue, 07 Feb 2023 22:57:41 GMT  
		Size: 289.5 MB (289480686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb89142f2d0761e51559b02dc38afb0ba5a8873b3f8b163f4930555a05ed6545`  
		Last Modified: Tue, 07 Feb 2023 22:57:13 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f002453150a97e2204515ee75923ab0cecdff8cb3205978a163ae0c86ac2ff6`  
		Last Modified: Tue, 07 Feb 2023 22:57:11 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2528ab2b7d241945a7a83f39ec84b06482e381b3a71d6302c9100be299ae700`  
		Last Modified: Tue, 07 Feb 2023 22:57:12 GMT  
		Size: 4.5 KB (4506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130895ed20fd9b4d2818be86b11b882d8efd0a721625edc022ad38cb5087dd2`  
		Last Modified: Tue, 07 Feb 2023 22:57:11 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fa2f4692370f3a8864a28f8476e0da22cd21b15b61ff73541cc8b5f09de4c7`  
		Last Modified: Tue, 07 Feb 2023 22:57:12 GMT  
		Size: 183.4 KB (183393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f22b75c18e5f9b7e0edb152d3537697fa37f4d35e069b4b4e87844bbfd8c527`  
		Last Modified: Tue, 07 Feb 2023 22:57:11 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.7.0`

```console
$ docker pull kibana@sha256:d5deba6a2303797077d1290b4c23cd34290bf29f5982baf557e946b921b90c31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.7.0` - linux; amd64

```console
$ docker pull kibana@sha256:35b26586f1b1180822047d9ee769e983c177f83a0235992d2495c09f9e6ad236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296222370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96c64a53cfef6942fa8c154d082b360d8e054d13c44df622d9197df63efea8e`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Mon, 27 Mar 2023 11:36:22 GMT
EXPOSE map[5601/tcp:{}]
# Mon, 27 Mar 2023 11:36:22 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Mon, 27 Mar 2023 11:36:23 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Mon, 27 Mar 2023 11:36:23 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Mon, 27 Mar 2023 11:36:24 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Mon, 27 Mar 2023 11:36:24 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Mon, 27 Mar 2023 11:36:25 GMT
RUN fc-cache -v # buildkit
# Mon, 27 Mar 2023 11:37:22 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Mon, 27 Mar 2023 11:37:22 GMT
WORKDIR /usr/share/kibana
# Mon, 27 Mar 2023 11:37:22 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Mon, 27 Mar 2023 11:37:22 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 27 Mar 2023 11:37:22 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 11:37:22 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Mon, 27 Mar 2023 11:37:22 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Mon, 27 Mar 2023 11:37:23 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Mon, 27 Mar 2023 11:37:23 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Mon, 27 Mar 2023 11:37:24 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Mon, 27 Mar 2023 11:37:24 GMT
LABEL org.label-schema.build-date=2023-03-27T11:09:20.771Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=05f12599523732051b84dde0b8d5610e0db2b06d org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.7.0 org.opencontainers.image.created=2023-03-27T11:09:20.771Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=05f12599523732051b84dde0b8d5610e0db2b06d org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.7.0
# Mon, 27 Mar 2023 11:37:24 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 27 Mar 2023 11:37:24 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Mon, 27 Mar 2023 11:37:24 GMT
USER kibana
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98647d2c3fafce2f36e423a6dd2bb4ffd864b34160a99f1d64d247e0474e42`  
		Last Modified: Wed, 05 Apr 2023 12:50:02 GMT  
		Size: 10.6 MB (10572323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726b0ba76f2f0a8ddbb8cf388f5d23bc3c883f17fe7cc046b2797e0fd5e7ba37`  
		Last Modified: Wed, 05 Apr 2023 12:49:52 GMT  
		Size: 9.5 KB (9526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aa88dac65bce64755ec84c90221fa7db754fa2f475b3dd02631e1728dc4f66`  
		Last Modified: Wed, 05 Apr 2023 12:49:50 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f3a0a33bc0851af4b502b5744d6493de4d831a73fd34f368b2b6b7857f11ad`  
		Last Modified: Wed, 05 Apr 2023 12:49:55 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c11ac6e8c00d1de56c8d3b4c98858403fe849c51e18cbe150b68c14dc935e`  
		Last Modified: Wed, 05 Apr 2023 12:49:48 GMT  
		Size: 5.3 KB (5299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbab1bb7e6a27bf8e047f9b9e8270816835e81e43b2611089e0a545b6128a5c`  
		Last Modified: Wed, 05 Apr 2023 12:50:33 GMT  
		Size: 240.4 MB (240399820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c215d8a6d0bac7626869f9dd072f87298491eba6dc1e617a0a26ae1fde9cdd`  
		Last Modified: Wed, 05 Apr 2023 12:49:48 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9ad2e0a02b7ac014cbdb78d04dccb19ba992ab0f78a2329c22c013036bec11`  
		Last Modified: Wed, 05 Apr 2023 12:49:44 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69c8f46e00caf21f5e919579d157b52da2485af6934bebb43727cf02e11dbf2`  
		Last Modified: Wed, 05 Apr 2023 12:49:44 GMT  
		Size: 4.5 KB (4481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d23bf98f9b948edfd5a70386d63f38c60c97f6b927c5183e59841b65bf1287`  
		Last Modified: Wed, 05 Apr 2023 12:49:44 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8902bdf4f1848448ebd83c56038e61e40b80c2364474fe15cf3c1760f6dda155`  
		Last Modified: Wed, 05 Apr 2023 12:49:45 GMT  
		Size: 189.4 KB (189394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fdd1b4302ceb39429466c38afea3612934e09287fa6d9ce9251968dc65ffc2`  
		Last Modified: Wed, 05 Apr 2023 12:49:44 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.7.0` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:26f656a347954677b77ddbce0c1769906e40f238577cc805cd32a75bd42b6c33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.1 MB (311120966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f43efc22fab06a1fec23aa425779674b2dad28bfe518da822613b35281f5a3b0`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Mon, 27 Mar 2023 11:39:23 GMT
EXPOSE map[5601/tcp:{}]
# Mon, 27 Mar 2023 11:39:23 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Mon, 27 Mar 2023 11:39:25 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Mon, 27 Mar 2023 11:39:25 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Mon, 27 Mar 2023 11:39:28 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Mon, 27 Mar 2023 11:39:28 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Mon, 27 Mar 2023 11:39:29 GMT
RUN fc-cache -v # buildkit
# Mon, 27 Mar 2023 11:40:26 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Mon, 27 Mar 2023 11:40:26 GMT
WORKDIR /usr/share/kibana
# Mon, 27 Mar 2023 11:40:26 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Mon, 27 Mar 2023 11:40:26 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 27 Mar 2023 11:40:26 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 11:40:26 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Mon, 27 Mar 2023 11:40:26 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Mon, 27 Mar 2023 11:40:27 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Mon, 27 Mar 2023 11:40:28 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Mon, 27 Mar 2023 11:40:28 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Mon, 27 Mar 2023 11:40:28 GMT
LABEL org.label-schema.build-date=2023-03-27T11:09:20.771Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=05f12599523732051b84dde0b8d5610e0db2b06d org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.7.0 org.opencontainers.image.created=2023-03-27T11:09:20.771Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=05f12599523732051b84dde0b8d5610e0db2b06d org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.7.0
# Mon, 27 Mar 2023 11:40:28 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 27 Mar 2023 11:40:28 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Mon, 27 Mar 2023 11:40:28 GMT
USER kibana
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fd75b9634426477ebcb42e3c9153f2833b67e04c727a5c7560ae8f413beb18`  
		Last Modified: Thu, 06 Apr 2023 01:31:41 GMT  
		Size: 10.4 MB (10440350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8a80ebe3f9ea27447cc35481fe40fcfb979aa594456e3f558fde319ef3cd40`  
		Last Modified: Thu, 06 Apr 2023 01:31:38 GMT  
		Size: 9.1 KB (9100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e240d41e7bbb1744c96bcb82a1dd13b43bf6e28ebc671df63b78e0226a72b09`  
		Last Modified: Thu, 06 Apr 2023 01:31:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e94d4121e2935a0b7255a780837c90441e449292d54b30e5ddce2180172163c`  
		Last Modified: Thu, 06 Apr 2023 01:31:37 GMT  
		Size: 16.5 MB (16460488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e9005ed3ab007710b272d97a5b8d0f64ea34261e73ceb01c6234ca4249f8d5`  
		Last Modified: Thu, 06 Apr 2023 01:31:36 GMT  
		Size: 5.3 KB (5297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f21dfbb604ecceab05b4f5b60d3111b619163ad73db02464994a570f7e35406`  
		Last Modified: Thu, 06 Apr 2023 01:32:00 GMT  
		Size: 256.8 MB (256818715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10762d5df24418231779a8668c7e4b4360d0864798715188aafd300e48dbbec2`  
		Last Modified: Thu, 06 Apr 2023 01:31:35 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c90fe6c4ab141def24a3c6ead328ce367acf78da59b7fe83a19b6ca7289c00`  
		Last Modified: Thu, 06 Apr 2023 01:31:33 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e025f8b86425a85de3fb4bc2ac6d4a529958f834d48b3941220b3525b8cc972`  
		Last Modified: Thu, 06 Apr 2023 01:31:33 GMT  
		Size: 4.5 KB (4486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb23b87d75e27faa0cf544d9e7471fb957c9ca1c01c85753e6cbf4d571ff72f`  
		Last Modified: Thu, 06 Apr 2023 01:31:33 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a644abc268aab8f5260fee79742afc1c75f557d48f1c2d0d5fb8a1799c22dc4`  
		Last Modified: Thu, 06 Apr 2023 01:31:34 GMT  
		Size: 183.4 KB (183398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75156bd242b110fb7c787d73865fa5092c46064ebe9cd6005798f6ff0b4c4bc`  
		Last Modified: Thu, 06 Apr 2023 01:31:38 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
