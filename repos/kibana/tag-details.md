<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.14`](#kibana71714)
-	[`kibana:8.11.0`](#kibana8110)

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

## `kibana:8.11.0`

**does not exist** (yet?)
