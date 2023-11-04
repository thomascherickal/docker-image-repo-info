<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.14`](#kibana71714)
-	[`kibana:8.10.3`](#kibana8103)
-	[`kibana:8.10.4`](#kibana8104)

## `kibana:7.17.14`

```console
$ docker pull kibana@sha256:a4036d6e1417388874d7496e9562eb900a2401b9750714f138db51093900802b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.17.14` - linux; amd64

```console
$ docker pull kibana@sha256:b1e30d8571b641bed67cf4de746d33b7b2943da429cbea043e1e2bc7d5d56898
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.9 MB (361934569 bytes)**  
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
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c20a59c466c3d2dbdce225e72179228de318b956dc3c89b36850546e544ca7`  
		Last Modified: Fri, 03 Nov 2023 00:24:38 GMT  
		Size: 17.1 MB (17122592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7246d90e7a3f7c73a1392d89051e28ff9e45e5729208340971e9beeb6b4225b`  
		Last Modified: Fri, 03 Nov 2023 00:24:36 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97247639b414b16b175d8b937f4ca08647384b5499e8538d651f3d9639b58fce`  
		Last Modified: Fri, 03 Nov 2023 00:24:34 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832778b738a8d352a6df08792883ebba8fd27dfbc7f9e5d26ef15e3f0f2aceac`  
		Last Modified: Fri, 03 Nov 2023 00:24:44 GMT  
		Size: 16.5 MB (16460483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5e62fee72ad07c59d65586a104e21b56e995c9f4a232866b4677b3c29e1465`  
		Last Modified: Fri, 03 Nov 2023 00:24:33 GMT  
		Size: 5.3 KB (5286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed93a8574c02043ada6d088c300cfc4f97b9ecb564af92870a2666de34274866`  
		Last Modified: Fri, 03 Nov 2023 00:27:05 GMT  
		Size: 299.6 MB (299559122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d1179197dde4a9c9c9585623f7e54461fceb6b16a95a2e2c4c81e00b8aec79`  
		Last Modified: Fri, 03 Nov 2023 00:24:33 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654a213b43f922c4b8571591c445c849bd172e17034704644b9409bf20bf9c2c`  
		Last Modified: Fri, 03 Nov 2023 00:24:31 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fb8099ab0a9ea8c0e1cec3afd9f6358c2ac732d2def773828c01f75500e60c`  
		Last Modified: Fri, 03 Nov 2023 00:24:31 GMT  
		Size: 4.5 KB (4509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecae3a4652605592d2eb98587b44e853f42b6cf20d33bcbd0928040dbfa52ba7`  
		Last Modified: Fri, 03 Nov 2023 00:24:31 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f141f7157f24f0a1cd3c857b82ca58d743e3f54b227c724ac6fdb76f784f36a`  
		Last Modified: Fri, 03 Nov 2023 00:24:32 GMT  
		Size: 189.4 KB (189407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466d5b98847fbd625bbd254358056b573224f3924d4b52e24ff394b06ac8587`  
		Last Modified: Fri, 03 Nov 2023 00:24:31 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.17.14` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:b79b1d2b3dc7766c8d62f1390e8c2438bd6d47cc5c82f7574df34827e4c5f1b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.9 MB (371873821 bytes)**  
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
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015728f8ea03f55f6c5b7ca44b076e4aac150c37f6aff1139cca58f6ea6f44ef`  
		Last Modified: Thu, 02 Nov 2023 23:42:29 GMT  
		Size: 15.9 MB (15923814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dc53f8fece35e7a606ecf2d74ea97067debed5d7e4401994becd471c89e2fc`  
		Last Modified: Thu, 02 Nov 2023 23:42:26 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f78d2c197d4c7b9792c23b877de63790c1c76271c19a95913d6b8d61bd24afe`  
		Last Modified: Thu, 02 Nov 2023 23:42:25 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7beaa1caa245b0a2564e7b58a622c93add531eb1c010b53439855ec4ae5f20`  
		Last Modified: Thu, 02 Nov 2023 23:42:26 GMT  
		Size: 16.5 MB (16460475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f99c0a4d10a5fd5a649413d2f4ef7d7a0a5546a88c72cfb6e9ffd95bf4d31e`  
		Last Modified: Thu, 02 Nov 2023 23:42:25 GMT  
		Size: 5.3 KB (5298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55aeaa657db921fde3ced56022349119d650746b7753b1f3d7b6dd2aaa491604`  
		Last Modified: Thu, 02 Nov 2023 23:42:52 GMT  
		Size: 312.1 MB (312083646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85292abfe347395b33ca3c07f182cecd4e15e8b397dbb8127a3ac443cf469829`  
		Last Modified: Thu, 02 Nov 2023 23:42:24 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60c78c3526c57aea1a7c0ca51677556b35d537854f07879fc6511dea4287003`  
		Last Modified: Thu, 02 Nov 2023 23:42:22 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06b330f982e092518dbb68803bfea51654a9acdcabd4ebad153a8c51ef1e5dd`  
		Last Modified: Thu, 02 Nov 2023 23:42:22 GMT  
		Size: 4.5 KB (4509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cdfb6ec996f352f0f9a6f1ec7ca445b28573c57448fddc05a0c0b811e900b`  
		Last Modified: Thu, 02 Nov 2023 23:42:22 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eeba035be7ecaddea4b02a824a7dc5339b4f6ade3c211081aebd4eb747300e1`  
		Last Modified: Thu, 02 Nov 2023 23:42:22 GMT  
		Size: 183.4 KB (183410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8251dcc955f00d46ed8f7225e656b58b1342f3b78493c634c0e80ff43ad65446`  
		Last Modified: Thu, 02 Nov 2023 23:42:22 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.10.3`

```console
$ docker pull kibana@sha256:a42b58a2a7337a2a45f3057792b2e8ebdd33f35b982b472135862be52861af51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.10.3` - linux; amd64

```console
$ docker pull kibana@sha256:5a7d7bd51c9f98613d102112c0b2e5b4e9ca1311492c0712723e62c62b8a28e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.6 MB (374576261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861082eb14770de055460d85150fcd270e3dcdbae6fc1197b16380b7a337a2b6`
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
# Thu, 05 Oct 2023 13:52:16 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 05 Oct 2023 13:52:16 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 05 Oct 2023 13:52:17 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 05 Oct 2023 13:52:17 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 05 Oct 2023 13:52:18 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 05 Oct 2023 13:52:18 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 05 Oct 2023 13:52:19 GMT
RUN fc-cache -v # buildkit
# Thu, 05 Oct 2023 13:54:24 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 05 Oct 2023 13:54:24 GMT
WORKDIR /usr/share/kibana
# Thu, 05 Oct 2023 13:54:25 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 05 Oct 2023 13:54:25 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 05 Oct 2023 13:54:25 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 13:54:25 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 05 Oct 2023 13:54:25 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 05 Oct 2023 13:54:26 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 05 Oct 2023 13:54:26 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 05 Oct 2023 13:54:27 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 05 Oct 2023 13:54:27 GMT
LABEL org.label-schema.build-date=2023-10-05T13:17:32.125Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=5aee3c4fba328838fcf0be6a3ff2248a4c0120dd org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.10.3 org.opencontainers.image.created=2023-10-05T13:17:32.125Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=5aee3c4fba328838fcf0be6a3ff2248a4c0120dd org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.10.3
# Thu, 05 Oct 2023 13:54:27 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 05 Oct 2023 13:54:27 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 05 Oct 2023 13:54:27 GMT
USER kibana
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755c91266cb04275d491b7eac1e6e2d08ff4ce905b77fbea02847fee85412619`  
		Last Modified: Mon, 16 Oct 2023 04:51:42 GMT  
		Size: 17.1 MB (17122539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e487d71afbd6beedb3241d92e3c700f751929a06a93cad26ae41ed3f3a3e27`  
		Last Modified: Mon, 16 Oct 2023 04:51:14 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e65c730b339c0e79f210c4ed68a9cd2c9ab34369898401fb0682e902044f078`  
		Last Modified: Mon, 16 Oct 2023 04:51:14 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b845086fc3608366d0d07a2fc4bc8935b7959928b3c03f5038b04d66aa23ded`  
		Last Modified: Mon, 16 Oct 2023 04:51:44 GMT  
		Size: 16.5 MB (16460486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55f6953d77b70053efd099b783ef222fb6d33c1c2a5a6a3020568a8437c263e`  
		Last Modified: Mon, 16 Oct 2023 04:51:12 GMT  
		Size: 5.3 KB (5300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e63249088cefbbb2e0037e20ac222a091b45f67208dd940ad67b331a13c4d02`  
		Last Modified: Mon, 16 Oct 2023 04:52:35 GMT  
		Size: 312.2 MB (312200790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38158e8c773e21fcf0ea58d59bbe044bb3bd6d44cdedf83eceda1c611a49c64`  
		Last Modified: Mon, 16 Oct 2023 04:51:12 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5e3dc65d38d871401d63477fa3e8f3d8bc6ae7e1f10a53867ff1b18a3142d`  
		Last Modified: Mon, 16 Oct 2023 04:51:11 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e354c7bdeb7241a675ce4b296a21e1cc686ab83a0ace641b2df72c8990fecf8`  
		Last Modified: Mon, 16 Oct 2023 04:51:10 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0338c6a14a736fbcfb3e37660f1b9cae3a8325a213467cb75406f168c4a799c5`  
		Last Modified: Mon, 16 Oct 2023 04:51:10 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ac00d5ef1bf750579dd0a3252f5e0299eda336a3570dfb37ba9af223ec644`  
		Last Modified: Mon, 16 Oct 2023 04:51:10 GMT  
		Size: 189.4 KB (189407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200c9d29ca12f8c9bc46deae6a5f951a4322f8fd0e11200ddaead3a36899d46a`  
		Last Modified: Mon, 16 Oct 2023 04:51:10 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.10.3` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:520f6fe201fae8fb3095cbcba4e28fdf4e17d6471facf64c488bf60df5124683
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.5 MB (384492517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26a7a846b776907e2c6cea528d1b8cd3fc09025712fd1740737b93a32ffc5958`
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
# Thu, 05 Oct 2023 13:56:50 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 05 Oct 2023 13:56:50 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 05 Oct 2023 13:56:52 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 05 Oct 2023 13:56:52 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 05 Oct 2023 13:56:55 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 05 Oct 2023 13:56:56 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 05 Oct 2023 13:56:57 GMT
RUN fc-cache -v # buildkit
# Thu, 05 Oct 2023 13:58:42 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 05 Oct 2023 13:58:42 GMT
WORKDIR /usr/share/kibana
# Thu, 05 Oct 2023 13:58:42 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 05 Oct 2023 13:58:42 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 05 Oct 2023 13:58:42 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 13:58:42 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 05 Oct 2023 13:58:42 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 05 Oct 2023 13:58:44 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 05 Oct 2023 13:58:45 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 05 Oct 2023 13:58:45 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 05 Oct 2023 13:58:45 GMT
LABEL org.label-schema.build-date=2023-10-05T13:17:32.125Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=5aee3c4fba328838fcf0be6a3ff2248a4c0120dd org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.10.3 org.opencontainers.image.created=2023-10-05T13:17:32.125Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=5aee3c4fba328838fcf0be6a3ff2248a4c0120dd org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.10.3
# Thu, 05 Oct 2023 13:58:45 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 05 Oct 2023 13:58:45 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 05 Oct 2023 13:58:45 GMT
USER kibana
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5f4fe98c8c5cbeee06a406c9ef22c7380c1ae3830e6fef1d736e86ea53228f`  
		Last Modified: Sat, 04 Nov 2023 01:33:18 GMT  
		Size: 15.9 MB (15923742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5972d02ef5de9d14c3a6c9ee587f5206a9baa552b3ecb24235696bac27d97ae`  
		Last Modified: Sat, 04 Nov 2023 01:33:16 GMT  
		Size: 9.1 KB (9098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85548e162bc722e101604c108d5f846088e47a7a9bdb3b5e40e39b1368260514`  
		Last Modified: Sat, 04 Nov 2023 01:33:14 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9a9be1ba3a9a4204e8b41e2c2971a86351f16333408214c616b46a9e296557`  
		Last Modified: Sat, 04 Nov 2023 01:33:15 GMT  
		Size: 16.5 MB (16460498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886388f7ad7f9d88b2a231b689b08cc193c17f360f0f59e0d8443b92098948bc`  
		Last Modified: Sat, 04 Nov 2023 01:33:14 GMT  
		Size: 5.3 KB (5310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e06f9cd2f3d0afc9181eac0acafdcc6bd694396942ae3b8e72896578db07827`  
		Last Modified: Sat, 04 Nov 2023 01:33:46 GMT  
		Size: 324.7 MB (324702332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504b4f348bb66d7d08acd84b93f68d64317f27523fcd91518c0ca379727001fc`  
		Last Modified: Sat, 04 Nov 2023 01:33:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f05e37045363246bdaff0de4dfc1a14851ff03822f4ef029456dfe50fa3ae19`  
		Last Modified: Sat, 04 Nov 2023 01:33:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0381da79d312b2612a370c2dc872f5cbec2d792e488664f9cb0938e120519f6`  
		Last Modified: Sat, 04 Nov 2023 01:33:12 GMT  
		Size: 4.6 KB (4555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097adb7e3ae46b655e04d751108f7bba33a1c46a74a7f2eb79f72de6d3abd63`  
		Last Modified: Sat, 04 Nov 2023 01:33:12 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7747af61944a43e3f589bba25464a68dc753bef799c6a7ada7536f60a8ea397`  
		Last Modified: Sat, 04 Nov 2023 01:33:12 GMT  
		Size: 183.4 KB (183411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145098f20b30c3f2e6a10216310a06f7981028c82524a487f55c2f5bcb510a92`  
		Last Modified: Sat, 04 Nov 2023 01:33:12 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.10.4`

```console
$ docker pull kibana@sha256:f8d8f4dde97fc22639081844fd685d3d048b79dc7cf53e633ac337905ad32cb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.10.4` - linux; amd64

```console
$ docker pull kibana@sha256:3de56e934027691dbdd7a65c605b93e781df1dfc206c22f0ecdfc769491aa9bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.6 MB (374569143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0389c1ec7f1c1dadf6089ffea9470358aafc712f6c50cd045a6f28224abdefd8`
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
# Wed, 11 Oct 2023 20:42:31 GMT
EXPOSE map[5601/tcp:{}]
# Wed, 11 Oct 2023 20:42:31 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Wed, 11 Oct 2023 20:42:32 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Wed, 11 Oct 2023 20:42:32 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Wed, 11 Oct 2023 20:42:33 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Wed, 11 Oct 2023 20:42:33 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Wed, 11 Oct 2023 20:42:34 GMT
RUN fc-cache -v # buildkit
# Wed, 11 Oct 2023 20:44:33 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Wed, 11 Oct 2023 20:44:33 GMT
WORKDIR /usr/share/kibana
# Wed, 11 Oct 2023 20:44:34 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Wed, 11 Oct 2023 20:44:34 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 11 Oct 2023 20:44:34 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 20:44:34 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Wed, 11 Oct 2023 20:44:34 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Wed, 11 Oct 2023 20:44:34 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Wed, 11 Oct 2023 20:44:35 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Wed, 11 Oct 2023 20:44:36 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Wed, 11 Oct 2023 20:44:36 GMT
LABEL org.label-schema.build-date=2023-10-11T20:06:54.391Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=976088dd04c6fd3b907fd2bb92af306e7d77ce4c org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.10.4 org.opencontainers.image.created=2023-10-11T20:06:54.391Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=976088dd04c6fd3b907fd2bb92af306e7d77ce4c org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.10.4
# Wed, 11 Oct 2023 20:44:36 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 11 Oct 2023 20:44:36 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Wed, 11 Oct 2023 20:44:36 GMT
USER kibana
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06edee18d747ff77ee7337ee29663e5049af1832e8e0adeed4f65dd4079bea0`  
		Last Modified: Wed, 25 Oct 2023 16:46:49 GMT  
		Size: 17.1 MB (17122356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cd15c6529cc3632dc209827ec252729e21ab4acdb4ff0ee431908eddf7a6f7`  
		Last Modified: Wed, 25 Oct 2023 16:46:45 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5610d99886cfb77172b65afc94892d0cc9f25b5a267b64e1deb61fbcf5393d26`  
		Last Modified: Wed, 25 Oct 2023 16:46:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6e140d9f19bdca0dfa514c428b82bbc8e1fd323eebccc1ae7867f7c9cfa07d`  
		Last Modified: Wed, 25 Oct 2023 16:46:46 GMT  
		Size: 16.5 MB (16460485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da8f6d450f34ad09bf4cd6218533bbfabe6bee359ce57f60a13d925a776577a`  
		Last Modified: Wed, 25 Oct 2023 16:46:44 GMT  
		Size: 5.3 KB (5303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef145f2c4ece6c200179283301129bb531dcbadb5469bfd75dc16f050a276c2`  
		Last Modified: Wed, 25 Oct 2023 16:47:58 GMT  
		Size: 312.2 MB (312193861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f369cc1b3d14b78b255f3cc125291810f8918992c608a72431ce2f75dbdf2ed2`  
		Last Modified: Wed, 25 Oct 2023 16:46:44 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f72199a988aa2e317f2812ea878f3739a8f2c14906b9a6b27639597ac7a77`  
		Last Modified: Wed, 25 Oct 2023 16:46:43 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac616300b2d654b8fb4ff8898d6b35be38c2f093e173c41216187949182c7ea`  
		Last Modified: Wed, 25 Oct 2023 16:46:42 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4373af135f431b6780ca12e1e7a45ed9b1ae7224c01e79eb4a113153b3830ca`  
		Last Modified: Wed, 25 Oct 2023 16:46:42 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d62bcd64fd04f54514d0d0bfa67108955e5f7b60ed5e18fa48457fbd9b222d5`  
		Last Modified: Wed, 25 Oct 2023 16:46:42 GMT  
		Size: 189.4 KB (189407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d10c267424ce5a02121460230b78badcb3b82e4dfda99f90d7856681aea8b1`  
		Last Modified: Wed, 25 Oct 2023 16:46:42 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.10.4` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:e16c96c8564da9825090ab44ed90bee04a5b09e3270a22e22c04f3718293ca69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.5 MB (384484536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e5e36fedbd1acab3aa939a29a569ee6c643de08a1e18dcd025ab89312d062ef`
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
# Wed, 11 Oct 2023 20:47:01 GMT
EXPOSE map[5601/tcp:{}]
# Wed, 11 Oct 2023 20:47:01 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Wed, 11 Oct 2023 20:47:03 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Wed, 11 Oct 2023 20:47:03 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Wed, 11 Oct 2023 20:47:06 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Wed, 11 Oct 2023 20:47:07 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Wed, 11 Oct 2023 20:47:07 GMT
RUN fc-cache -v # buildkit
# Wed, 11 Oct 2023 20:49:05 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Wed, 11 Oct 2023 20:49:05 GMT
WORKDIR /usr/share/kibana
# Wed, 11 Oct 2023 20:49:05 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Wed, 11 Oct 2023 20:49:05 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 11 Oct 2023 20:49:05 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 20:49:05 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Wed, 11 Oct 2023 20:49:05 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Wed, 11 Oct 2023 20:49:06 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Wed, 11 Oct 2023 20:49:07 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Wed, 11 Oct 2023 20:49:08 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Wed, 11 Oct 2023 20:49:08 GMT
LABEL org.label-schema.build-date=2023-10-11T20:06:54.391Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=976088dd04c6fd3b907fd2bb92af306e7d77ce4c org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.10.4 org.opencontainers.image.created=2023-10-11T20:06:54.391Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=976088dd04c6fd3b907fd2bb92af306e7d77ce4c org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.10.4
# Wed, 11 Oct 2023 20:49:08 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 11 Oct 2023 20:49:08 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Wed, 11 Oct 2023 20:49:08 GMT
USER kibana
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3455bc79e0cd78ee160c19f82dcbf9946f2bd6f4fddd8b05a10ad16977b2dae`  
		Last Modified: Thu, 02 Nov 2023 23:41:47 GMT  
		Size: 15.9 MB (15923217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ca742d3642a991a7fc72780649d066ec22837bb26bc163c5b09f58b6f890d8`  
		Last Modified: Thu, 02 Nov 2023 23:41:45 GMT  
		Size: 9.1 KB (9100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69590ece7831c51dba72d67090f26a85fc7341f6bf97eb1c906fc67c613f7c6b`  
		Last Modified: Thu, 02 Nov 2023 23:41:44 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93e8eb8fb661c8213fa20e426e63338f6191829c26e13f17a608f1e12ed18ca`  
		Last Modified: Thu, 02 Nov 2023 23:41:45 GMT  
		Size: 16.5 MB (16460473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cbe0bbedff45cc26eedd6fe509d24d4c14f37c0cdf84c6ce1a00a05b99c6ce`  
		Last Modified: Thu, 02 Nov 2023 23:41:43 GMT  
		Size: 5.3 KB (5290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60407e2c8d37f518e80d8cc3fc32e4af5cf771e1f1f2ee2ef6569cf6a0318cdf`  
		Last Modified: Thu, 02 Nov 2023 23:42:15 GMT  
		Size: 324.7 MB (324694912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4793da589290a6847141e34b95e224bbbd9161e560761de39ca15282cccca717`  
		Last Modified: Thu, 02 Nov 2023 23:41:43 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299beb397f9d75cdd4e4ec8db976a8b2ca51ee920d90c4cce84c3974e66b6ce2`  
		Last Modified: Thu, 02 Nov 2023 23:41:40 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79427a198b33428e40a842b1f6f3d312dba0294b1d768298f0a27693224de073`  
		Last Modified: Thu, 02 Nov 2023 23:41:40 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419186b132cc8073c04f213627490007a0bcda34968d7e62b0e5bbd59ec03702`  
		Last Modified: Thu, 02 Nov 2023 23:41:40 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e300f4e6bcb4ad796f8d29b14e5bf0b3ffb0755569ea15127d82d4ca0d0dcc4`  
		Last Modified: Thu, 02 Nov 2023 23:41:41 GMT  
		Size: 183.4 KB (183412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47575bf38e08f475cea7fc21709390397391ef8442fcf5a48e799fb747dcfbd`  
		Last Modified: Thu, 02 Nov 2023 23:41:42 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
