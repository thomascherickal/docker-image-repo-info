<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.14`](#kibana71714)
-	[`kibana:8.11.0`](#kibana8110)

## `kibana:7.17.14`

```console
$ docker pull kibana@sha256:7519d4bb02c8697d14f249f6ce1ad66345184734fd6b0aa7b0c362f8bfa6f374
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `kibana:7.17.14` - linux; amd64

```console
$ docker pull kibana@sha256:512f7c688770f4d08fd8f25ef74fda60c3c1493a874265a095645c79c6adfeeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.8 MB (404814683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d732a75b15df3dc4337fb2394faba3e86c140e264f48a3326f82767f6bd92148`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 05 Oct 2023 11:44:21 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 05 Oct 2023 11:44:21 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 05 Oct 2023 11:44:21 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 05 Oct 2023 11:44:22 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 05 Oct 2023 11:44:22 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 05 Oct 2023 11:44:23 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 05 Oct 2023 11:44:23 GMT
RUN fc-cache -v # buildkit
# Thu, 05 Oct 2023 11:45:26 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 05 Oct 2023 11:45:26 GMT
WORKDIR /usr/share/kibana
# Thu, 05 Oct 2023 11:45:26 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 05 Oct 2023 11:45:26 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 05 Oct 2023 11:45:26 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 11:45:26 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 05 Oct 2023 11:45:26 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 05 Oct 2023 11:45:26 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 05 Oct 2023 11:45:27 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 05 Oct 2023 11:45:27 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 05 Oct 2023 11:45:27 GMT
LABEL org.label-schema.build-date=2023-10-05T11:15:51.563Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=511a5a1f6ec639035d64f57cabf10b392dc3b9fb org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.14 org.opencontainers.image.created=2023-10-05T11:15:51.563Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=511a5a1f6ec639035d64f57cabf10b392dc3b9fb org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.14
# Thu, 05 Oct 2023 11:45:27 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 05 Oct 2023 11:45:27 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 05 Oct 2023 11:45:27 GMT
USER kibana
```

-	Layers:
	-	`sha256:f9175e7b73a4b948b4c5db289cbeeb1d8511aee675255978036e76ffeda560be`  
		Last Modified: Mon, 07 Aug 2023 21:55:17 GMT  
		Size: 31.8 MB (31795971 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e8042d285a55aaff169f086be7088e4d9d99462c97737572fbea995e1100f8c`  
		Last Modified: Tue, 10 Oct 2023 09:01:43 GMT  
		Size: 19.1 MB (19091297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:242e95a8f0ccd001a49448e7fdb80591062fbb281b2233f803f46a74a61e6b0e`  
		Last Modified: Tue, 10 Oct 2023 09:01:41 GMT  
		Size: 10.2 KB (10157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca4fbe6b208ce8dd8e5b8609c7a6c5904f9ac86277dc06c9d61c28325759f216`  
		Last Modified: Tue, 10 Oct 2023 09:01:41 GMT  
		Size: 164.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ddaf6cc97cc060a94e7b1d66db965f44036c7b1482e94ec7baac5161980e1af6`  
		Last Modified: Tue, 10 Oct 2023 09:01:43 GMT  
		Size: 17.8 MB (17831460 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8dca212837a8738c753011d502d6e69967ed64b7bbbb7d52bed661c51228114a`  
		Last Modified: Tue, 10 Oct 2023 09:01:43 GMT  
		Size: 5.9 KB (5941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16a350e49d9505999c9e0d4776e17600671b38e4fc48d68282aaa279b14836f4`  
		Last Modified: Tue, 10 Oct 2023 09:02:04 GMT  
		Size: 335.9 MB (335863349 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4956618e774df7295d2c696e1786cbc904efc11b097b521035912da6dba1e918`  
		Last Modified: Tue, 10 Oct 2023 09:01:44 GMT  
		Size: 140.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81fec2d0ccd6b3f014676b65b6a1528424263754ed74f7492c7bed59f68f8469`  
		Last Modified: Tue, 10 Oct 2023 09:01:45 GMT  
		Size: 416.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d66c814bb28aa4da48780b06630d2aaab49a4ea40781c18dc6414da83bde590b`  
		Last Modified: Tue, 10 Oct 2023 09:01:45 GMT  
		Size: 5.0 KB (5012 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e6a23431e0cb96dbabca902b754393c7b70d25e03aa08a8aeca0dd8ead6fad3`  
		Last Modified: Tue, 10 Oct 2023 09:01:46 GMT  
		Size: 417.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a21a8364606b80e26211968af37001d903213d2b1a8dd4ef7c1943c4e65acdfc`  
		Last Modified: Tue, 10 Oct 2023 09:01:46 GMT  
		Size: 208.2 KB (208249 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0792afd956ee0cae7bfcc1ad4d7e9a8e12a437e568fb09f844c815bd6b7ae747`  
		Last Modified: Tue, 10 Oct 2023 09:01:46 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `kibana:7.17.14` - unknown; unknown

```console
$ docker pull kibana@sha256:cbd2b1d3bc6bf6fa8dfb947791aeb51762ce950ebf7d96fa7a75804b8228d989
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e97566710efe95b7a8fa5fcf47d1774b8e9d5a8cf034cef24017daf81a22d4`

```dockerfile
```

-	Layers:
	-	`sha256:ce162abef48d1140be20080a4f4c36197cd57b2776c8e0b1f4d2b43aa6e373d4`  
		Last Modified: Thu, 09 Nov 2023 22:20:05 GMT  
		Size: 3.0 MB (3037137 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:58fb3ebe435e5f03d91db513d624dea4d44320696d6e8198bb17e7bf708b9c05`  
		Last Modified: Thu, 09 Nov 2023 22:20:04 GMT  
		Size: 8.6 KB (8566 bytes)  
		MIME: application/vnd.in-toto+json

### `kibana:7.17.14` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:acdd1447521bdd8b952549af75c0f3211d3c6d8e82f88920af530dd1d6a87e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.6 MB (414646021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbd2ec9e047157bfb43720d6501c8fe47c1cbbd5b88ecaf2bda5091b0513cfed`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 05 Oct 2023 11:47:41 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 05 Oct 2023 11:47:41 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 05 Oct 2023 11:47:42 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 05 Oct 2023 11:47:43 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 05 Oct 2023 11:47:45 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 05 Oct 2023 11:47:46 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 05 Oct 2023 11:47:46 GMT
RUN fc-cache -v # buildkit
# Thu, 05 Oct 2023 11:48:49 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 05 Oct 2023 11:48:49 GMT
WORKDIR /usr/share/kibana
# Thu, 05 Oct 2023 11:48:49 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 05 Oct 2023 11:48:49 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 05 Oct 2023 11:48:49 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 11:48:49 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 05 Oct 2023 11:48:49 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 05 Oct 2023 11:48:50 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 05 Oct 2023 11:48:51 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 05 Oct 2023 11:48:52 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 05 Oct 2023 11:48:52 GMT
LABEL org.label-schema.build-date=2023-10-05T11:15:51.563Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=511a5a1f6ec639035d64f57cabf10b392dc3b9fb org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.14 org.opencontainers.image.created=2023-10-05T11:15:51.563Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=511a5a1f6ec639035d64f57cabf10b392dc3b9fb org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.14
# Thu, 05 Oct 2023 11:48:52 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 05 Oct 2023 11:48:52 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 05 Oct 2023 11:48:52 GMT
USER kibana
```

-	Layers:
	-	`sha256:e61e4aa6ecf06d84f177710ed7a16ba36429af08286de7aa5a485fdcedaac1f7`  
		Last Modified: Thu, 17 Aug 2023 10:22:08 GMT  
		Size: 29.9 MB (29915840 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65edd6608a730132f7b9534b4eca0c6e9d9035d0e74fa0323b614b14a776d018`  
		Last Modified: Tue, 10 Oct 2023 09:01:46 GMT  
		Size: 17.5 MB (17530098 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17b5714ab4797d455636148a09e9269815aeb17ee15e95103ac9aa79e31e0e5a`  
		Last Modified: Tue, 10 Oct 2023 09:01:45 GMT  
		Size: 9.8 KB (9758 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a70746584bded2bfa74019bada0d9224f551de5844bf1560e55801382c7b81dd`  
		Last Modified: Tue, 10 Oct 2023 09:01:45 GMT  
		Size: 164.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8657444217bd9dd23288cd785830a621076ddc836c4c9e052f27f3d7ea37000d`  
		Last Modified: Tue, 10 Oct 2023 09:01:47 GMT  
		Size: 17.8 MB (17831464 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b326a03cdae764180f92f57e79e5283114aedd3eea85a6134f5efe4ec53b7c0`  
		Last Modified: Tue, 10 Oct 2023 09:01:46 GMT  
		Size: 6.0 KB (5959 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8150789ac11dadd264e5b6940342218eb269ae5fe18746871e37658dfcbe6687`  
		Last Modified: Tue, 10 Oct 2023 09:02:13 GMT  
		Size: 349.1 MB (349144330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d560d8882ccd05c4818b7bc2e583df65e4907e35b0f03f92f73c8e76d38abb02`  
		Last Modified: Tue, 10 Oct 2023 09:01:48 GMT  
		Size: 140.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f907e12d180fc28bf4948c797e1e18f7fb9d80a7691c3abd3e066428a7441c26`  
		Last Modified: Tue, 10 Oct 2023 09:01:48 GMT  
		Size: 417.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2841b517f7b330762e6dd0cf3b6a5bebb40b1092aa26ea259fa1ee5eb9d99319`  
		Last Modified: Tue, 10 Oct 2023 09:01:49 GMT  
		Size: 5.0 KB (5010 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0288286364badffcc98209d02658d778d1f713db91a942de6b3923c9eec0f48c`  
		Last Modified: Tue, 10 Oct 2023 09:01:49 GMT  
		Size: 419.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4895402879963935f7f4e29781de1359507a0bf625d901a7ab5ba43ab4fb0253`  
		Last Modified: Tue, 10 Oct 2023 09:01:50 GMT  
		Size: 200.3 KB (200304 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb1294d67390b22f3e4c4d0e042f2036f058ac066a46407f018594d148a4b7bd`  
		Last Modified: Tue, 10 Oct 2023 09:01:51 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `kibana:7.17.14` - unknown; unknown

```console
$ docker pull kibana@sha256:4aa8558b2b95698198cdbf43cb800d18f91dedd0993a7c1a92f64825b25475d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3046046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86e3523a5c8b69cf048c8cc41cf80a75ad08cfe09cc0bdab7f63d3f1097fe3ae`

```dockerfile
```

-	Layers:
	-	`sha256:404c2d5fe31bc1fe289085b3f2563de5c9a8dbce8e6cd388311e428ffa28f289`  
		Last Modified: Thu, 09 Nov 2023 22:32:39 GMT  
		Size: 3.0 MB (3037478 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:21d8a7c2e113b4e26246adfe7d2aaeaeaa4f9fb8bf8a14894c8ad84869fac967`  
		Last Modified: Thu, 09 Nov 2023 22:32:40 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.in-toto+json

## `kibana:8.11.0`

```console
$ docker pull kibana@sha256:18088be31fc33f8abcbee8b379299710d3e6d06df8a81368c5c35e906b6791a7
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 3
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8

### `kibana:8.11.0` - linux; amd64

```console
$ docker pull kibana@sha256:8d3b75d6b6477bf29fa65de1ba137e766b5f4b3396156544518783ead8af808e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.2 MB (419245553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14de45f6130869a4ad2ae0004544c83750db66b4a0867614eb12cf22f06db216`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 11:43:06 GMT
EXPOSE map[5601/tcp:{}]
# Sat, 04 Nov 2023 11:43:06 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Sat, 04 Nov 2023 11:43:07 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Sat, 04 Nov 2023 11:43:08 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Sat, 04 Nov 2023 11:43:09 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Sat, 04 Nov 2023 11:43:09 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Sat, 04 Nov 2023 11:43:10 GMT
RUN fc-cache -v # buildkit
# Sat, 04 Nov 2023 11:44:56 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Sat, 04 Nov 2023 11:44:56 GMT
WORKDIR /usr/share/kibana
# Sat, 04 Nov 2023 11:44:56 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Sat, 04 Nov 2023 11:44:56 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 04 Nov 2023 11:44:56 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 11:44:56 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Sat, 04 Nov 2023 11:44:56 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 11:44:57 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Sat, 04 Nov 2023 11:44:58 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Sat, 04 Nov 2023 11:44:58 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Sat, 04 Nov 2023 11:44:58 GMT
LABEL org.label-schema.build-date=2023-11-04T11:05:43.123Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=f2ea0c43ec0d854259d63d926b97e5c556b5f6b2 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.11.0 org.opencontainers.image.created=2023-11-04T11:05:43.123Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=f2ea0c43ec0d854259d63d926b97e5c556b5f6b2 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.0
# Sat, 04 Nov 2023 11:44:58 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Sat, 04 Nov 2023 11:44:58 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Sat, 04 Nov 2023 11:44:58 GMT
USER kibana
```

-	Layers:
	-	`sha256:70db4e7a2af7f73b7cef95301fc20fbedcfe68e5fb874e2cfba0b5ae41a066ca`  
		Last Modified: Wed, 25 Oct 2023 11:40:40 GMT  
		Size: 31.8 MB (31790746 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7413290cc362e8d5cc6e90941d5264840d5c8e2ea1cd2b0388991fb39431e62c`  
		Last Modified: Tue, 07 Nov 2023 14:30:13 GMT  
		Size: 11.7 MB (11718207 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72616e7296fbc3ee86976cfebab512228085ec508d79d968adbf0c73dfd1bdd0`  
		Last Modified: Tue, 07 Nov 2023 14:30:11 GMT  
		Size: 10.2 KB (10157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f541970e6b68391f6c45413790b3b9837bbbfa11160f981165de3d73fe9b1665`  
		Last Modified: Tue, 07 Nov 2023 14:30:57 GMT  
		Size: 164.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ecb94b53d7d640b9f7225b23f39287dc751b40625efeebf106d332e0639fd482`  
		Last Modified: Tue, 07 Nov 2023 14:30:53 GMT  
		Size: 17.8 MB (17831463 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d95812e4d485b6c423f058226d7a33dca2eb134a917a91c6c52b7ce7b2820b05`  
		Last Modified: Tue, 07 Nov 2023 14:30:27 GMT  
		Size: 5.9 KB (5946 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d3b4c94950836ee9ec591dc7932972a3d0771420bfb3efd9c99ac12142b138b`  
		Last Modified: Tue, 07 Nov 2023 14:30:06 GMT  
		Size: 357.7 MB (357672406 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98e8f048e90fdec4f53747b1d3c99343067772be0a79c1cfbe5a3eee56f1b911`  
		Last Modified: Tue, 07 Nov 2023 14:30:18 GMT  
		Size: 140.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:847df9b49e1196ada8f35abf5f1ec419f48fc687e53a54d9b84da66a081d1869`  
		Last Modified: Tue, 07 Nov 2023 14:30:17 GMT  
		Size: 416.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58c21d0fd8db6ff7a012818bfe0773fbbbc0fd5500ab033fc0a5f6788e2eaae3`  
		Last Modified: Tue, 07 Nov 2023 14:29:48 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:443d4789d61d2949396acaac9e7b16536d8beeb02e363318be389758b071461b`  
		Last Modified: Tue, 07 Nov 2023 14:29:45 GMT  
		Size: 416.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55133e78e7c1f4d5ab4a3da8fbf80dc2d21eeae376205d0cd75a113bd1df68e6`  
		Last Modified: Tue, 07 Nov 2023 14:29:47 GMT  
		Size: 208.2 KB (208247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:daa86f9287ca9044d5d519e179dfe6db345acad3a5a7b96ae13f305e7396832f`  
		Last Modified: Tue, 07 Nov 2023 14:30:28 GMT  
		Size: 2.0 KB (2036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `kibana:8.11.0` - unknown; unknown

```console
$ docker pull kibana@sha256:ca8ae3e1a1fac2b6d449f02807efc830f75f36b34668165955edd6a9c97cb802
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3466018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861f314bad384ae4b9da69e5e3c2cbf42b9edce88b71dc358aea1c90a679d1dc`

```dockerfile
```

-	Layers:
	-	`sha256:78d2302dd1906ab054ebd678bcbedadbb9f93a1fed496b115ae9539a378ba87f`  
		Last Modified: Thu, 09 Nov 2023 22:20:26 GMT  
		Size: 3.5 MB (3457458 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:58e8e857baceef971b5142ca76ed44aead36b00ae849754753c40767bc5b5dd6`  
		Last Modified: Thu, 09 Nov 2023 22:20:25 GMT  
		Size: 8.6 KB (8560 bytes)  
		MIME: application/vnd.in-toto+json

### `kibana:8.11.0` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:c4ae2cc41dedc3afd7f23bfa6b43593e2e662e6dd06ea12310b7e9f3285717d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.0 MB (379989035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a20524a06f125560ea4e7cd8e134d21cc266cd44c54f32d312eeb931c52769ca`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 11:47:16 GMT
EXPOSE map[5601/tcp:{}]
# Sat, 04 Nov 2023 11:47:16 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Sat, 04 Nov 2023 11:47:20 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Sat, 04 Nov 2023 11:47:20 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Sat, 04 Nov 2023 11:47:24 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Sat, 04 Nov 2023 11:47:25 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Sat, 04 Nov 2023 11:47:25 GMT
RUN fc-cache -v # buildkit
# Sat, 04 Nov 2023 11:49:23 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Sat, 04 Nov 2023 11:49:23 GMT
WORKDIR /usr/share/kibana
# Sat, 04 Nov 2023 11:49:23 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Sat, 04 Nov 2023 11:49:23 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 04 Nov 2023 11:49:23 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 11:49:23 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Sat, 04 Nov 2023 11:49:23 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 11:49:25 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Sat, 04 Nov 2023 11:49:26 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Sat, 04 Nov 2023 11:49:27 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Sat, 04 Nov 2023 11:49:27 GMT
LABEL org.label-schema.build-date=2023-11-04T11:05:43.123Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=f2ea0c43ec0d854259d63d926b97e5c556b5f6b2 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.11.0 org.opencontainers.image.created=2023-11-04T11:05:43.123Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=f2ea0c43ec0d854259d63d926b97e5c556b5f6b2 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.0
# Sat, 04 Nov 2023 11:49:27 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Sat, 04 Nov 2023 11:49:27 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Sat, 04 Nov 2023 11:49:27 GMT
USER kibana
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaf1e0369170a4483e3643464bdd14b0fb628892c55474811bbf12e012b08e7`  
		Last Modified: Tue, 07 Nov 2023 23:47:44 GMT  
		Size: 10.4 MB (10399319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a552314993012ff06066bdc9d303c193019bc8cadfbed6477c266543129859`  
		Last Modified: Tue, 07 Nov 2023 23:47:42 GMT  
		Size: 9.1 KB (9098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ad294bbd34c694dc27f8d10f407f9887cc0479feea845a1c7400d053f922f0`  
		Last Modified: Tue, 07 Nov 2023 23:47:42 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129de6f7096bba867e34a11284d7ec26fab05955e050eaf5f4301fa42a0a7d0c`  
		Last Modified: Tue, 07 Nov 2023 23:47:42 GMT  
		Size: 16.5 MB (16460486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07308b2afe0377d18c4fbea8477de9d86d9d898b9d52eaf29b44cfc06f9dff77`  
		Last Modified: Tue, 07 Nov 2023 23:47:40 GMT  
		Size: 5.3 KB (5288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808c00c917f4cb1ebd710daf7fc5d89826641350f2e81fed251ac34fd9647b39`  
		Last Modified: Tue, 07 Nov 2023 23:48:15 GMT  
		Size: 325.7 MB (325724397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db2cc52d6076c59bb0f3c919862daa2ade01cb3760f38657710bb916fbbfb47`  
		Last Modified: Tue, 07 Nov 2023 23:47:40 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11248d8c8f2b36d337022eeeffb1ebf2501bb23228f340411fbc8dc77a785434`  
		Last Modified: Tue, 07 Nov 2023 23:47:38 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e909dd48b67a6d90c2f4cdfdd733c5deb57ba214250a39ba721f6231047b89c`  
		Last Modified: Tue, 07 Nov 2023 23:47:37 GMT  
		Size: 4.6 KB (4555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806914c45a72cf2bb8905cd0cca34a8e4c5872077b3c62316d21fd679928df8e`  
		Last Modified: Tue, 07 Nov 2023 23:47:37 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50789af08027f336da9fc6c47d3e6e0d6de50da55dab05c277aa77901c0ba982`  
		Last Modified: Tue, 07 Nov 2023 23:47:38 GMT  
		Size: 183.4 KB (183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7420e62c9a6195d16bc3b56def214e9442617c7046dd2f4856ae5de04f54f4`  
		Last Modified: Tue, 07 Nov 2023 23:47:41 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
