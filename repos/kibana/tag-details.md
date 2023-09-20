<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.13`](#kibana71713)
-	[`kibana:8.10.1`](#kibana8101)

## `kibana:7.17.13`

```console
$ docker pull kibana@sha256:cbb3a6e86a1347600bde34f4643c8b28db0b561e0d895ed5312917c12947cba2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.17.13` - linux; amd64

```console
$ docker pull kibana@sha256:dce4cbbf3938ce6288dacce0de9fdde95f8f530a02efda9be8e4cb1c5f068289
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.3 MB (364345500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:455264e8b0859fca12dc9487f792d374d069c56b03e44e13d4f07c432f582283`
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
# Thu, 31 Aug 2023 11:39:37 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 31 Aug 2023 11:39:37 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 31 Aug 2023 11:39:38 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 31 Aug 2023 11:39:39 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 31 Aug 2023 11:39:39 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 31 Aug 2023 11:39:40 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 31 Aug 2023 11:39:40 GMT
RUN fc-cache -v # buildkit
# Thu, 31 Aug 2023 11:40:48 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 31 Aug 2023 11:40:49 GMT
WORKDIR /usr/share/kibana
# Thu, 31 Aug 2023 11:40:49 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 31 Aug 2023 11:40:49 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 31 Aug 2023 11:40:49 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 11:40:49 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 31 Aug 2023 11:40:49 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 31 Aug 2023 11:40:49 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 31 Aug 2023 11:40:50 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 31 Aug 2023 11:40:51 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 31 Aug 2023 11:40:51 GMT
LABEL org.label-schema.build-date=2023-08-31T11:10:13.696Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=8791f8bf89c9d2080fade55c42a40d03b91939f4 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.13 org.opencontainers.image.created=2023-08-31T11:10:13.696Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=8791f8bf89c9d2080fade55c42a40d03b91939f4 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.13
# Thu, 31 Aug 2023 11:40:51 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 31 Aug 2023 11:40:51 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 31 Aug 2023 11:40:51 GMT
USER kibana
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4ccc0478e3263905721067e2e66fc6e9307d1de3575ddd9772b2d173150da9`  
		Last Modified: Fri, 08 Sep 2023 05:24:55 GMT  
		Size: 10.5 MB (10531750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd5d3bd05ca254a97e1133e0261796a629047b2416ef4d30abe17ed7d2ce91`  
		Last Modified: Fri, 08 Sep 2023 05:24:53 GMT  
		Size: 9.5 KB (9525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327b6efa957df5a31f2d4edca2f632bb679ae6c718135f99bec48e5cb74660a4`  
		Last Modified: Fri, 08 Sep 2023 05:24:51 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd245b2cd22d9a335556a530ab61cd1ed6a1ee2e09c296d922e76676c42fb0b`  
		Last Modified: Fri, 08 Sep 2023 05:24:53 GMT  
		Size: 16.5 MB (16460491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffa61183fb32aa74914bb17239d1adae7921872f47631988b6d06f6f342668e`  
		Last Modified: Fri, 08 Sep 2023 05:24:51 GMT  
		Size: 5.3 KB (5294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbebb4e44b16718a0550c9d2e5f2701f925571cc702b2985d89d6a48ed3adc2d`  
		Last Modified: Fri, 08 Sep 2023 05:25:26 GMT  
		Size: 308.6 MB (308560880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b55b12c15764f6ab8868ae711f6890423dc93ea04321d8d66531e7434d25e33`  
		Last Modified: Fri, 08 Sep 2023 05:24:51 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd91fb1a78c3bad1b100afc45b5249d276dbd1332cccba33d5a5b2c5c9d9ffc`  
		Last Modified: Fri, 08 Sep 2023 05:24:49 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a3014a0de9adecc0e0d582ad261c8989a98bd4e86d75a816694fdd3196a369`  
		Last Modified: Fri, 08 Sep 2023 05:24:49 GMT  
		Size: 4.5 KB (4508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06412d076a50d1459a5dedab1c02d3339a12c5ce84b69288aeeaa3dba511fc42`  
		Last Modified: Fri, 08 Sep 2023 05:24:49 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1690e39505c217af9e87f79d2cee43bbe5087869db76d38afdc9ab08baa76`  
		Last Modified: Fri, 08 Sep 2023 05:24:49 GMT  
		Size: 189.4 KB (189405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80017efa434a3448bda2d320fbef06d60bc95339731b9931ff52efb474f6356`  
		Last Modified: Fri, 08 Sep 2023 05:24:49 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.17.13` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:4589111220afc31853cc6c849501f8d4049a9362813f48a9f9c83ed5c26b81d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.9 MB (374891371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be38c397da4706913a30b8b44597da63200e3e079166fc40e7dc86cab139594d`
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
# Thu, 31 Aug 2023 11:43:03 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 31 Aug 2023 11:43:03 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 31 Aug 2023 11:43:05 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 31 Aug 2023 11:43:05 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 31 Aug 2023 11:43:08 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 31 Aug 2023 11:43:08 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 31 Aug 2023 11:43:09 GMT
RUN fc-cache -v # buildkit
# Thu, 31 Aug 2023 11:44:16 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 31 Aug 2023 11:44:16 GMT
WORKDIR /usr/share/kibana
# Thu, 31 Aug 2023 11:44:16 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 31 Aug 2023 11:44:16 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 31 Aug 2023 11:44:16 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 11:44:16 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 31 Aug 2023 11:44:16 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 31 Aug 2023 11:44:17 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 31 Aug 2023 11:44:18 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 31 Aug 2023 11:44:18 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 31 Aug 2023 11:44:18 GMT
LABEL org.label-schema.build-date=2023-08-31T11:10:13.696Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=8791f8bf89c9d2080fade55c42a40d03b91939f4 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.13 org.opencontainers.image.created=2023-08-31T11:10:13.696Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=8791f8bf89c9d2080fade55c42a40d03b91939f4 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.13
# Thu, 31 Aug 2023 11:44:18 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 31 Aug 2023 11:44:18 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 31 Aug 2023 11:44:18 GMT
USER kibana
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcec88b593a59b4961daa11145482cbbd4e623aeaee39f5fa74d31bb193fc22`  
		Last Modified: Thu, 07 Sep 2023 23:41:33 GMT  
		Size: 10.4 MB (10399328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a07605f74576d843933b6f2f80061552111172ee42119d60c0519cf4fa583`  
		Last Modified: Thu, 07 Sep 2023 23:41:32 GMT  
		Size: 9.1 KB (9099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d7a55bd435941d1d281ed08cacb1ba3f7afe3d3dad9ef4fcd68aadc2a0a2eb`  
		Last Modified: Thu, 07 Sep 2023 23:41:30 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7480e4203fc2c8eb30be342484638b285dcc2ca5718efbd63b36298e8e937764`  
		Last Modified: Thu, 07 Sep 2023 23:41:31 GMT  
		Size: 16.5 MB (16460497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341d5261be208cb9503636820d830f99d06f9ea16f1aca8fb81644ba2d86de98`  
		Last Modified: Thu, 07 Sep 2023 23:41:30 GMT  
		Size: 5.3 KB (5289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d554cc3386ed8df8130409f73cd37a95e0c2ae433485b8f1c6b92342ff8db510`  
		Last Modified: Thu, 07 Sep 2023 23:42:01 GMT  
		Size: 320.6 MB (320625679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340fb529cdc657058e48c8d09bd01ae0b6b475b7041b46b4faed922a7f4962e2`  
		Last Modified: Thu, 07 Sep 2023 23:41:30 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa61e43a8a3c176851a044fb082d46cdb4693c0c09665303567f1e6f03745f1`  
		Last Modified: Thu, 07 Sep 2023 23:41:28 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6741c1dc0f03fa7b06890a952e1eda2749c66ec868907398d54798bd87c913`  
		Last Modified: Thu, 07 Sep 2023 23:41:28 GMT  
		Size: 4.5 KB (4508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3176d9ced454c06886a132501adb1593547bf2b786c4bd762f8de69e4e74eb`  
		Last Modified: Thu, 07 Sep 2023 23:41:28 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e151befe6dc49aae6a13532ddcb2dbe7a0ef7d1e1442003a05b3372e57514642`  
		Last Modified: Thu, 07 Sep 2023 23:41:28 GMT  
		Size: 183.4 KB (183410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c617383aba737c9061270980206d48786e6d00a62da8cbbe6392c65bd2a3406`  
		Last Modified: Thu, 07 Sep 2023 23:41:28 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.10.1`

```console
$ docker pull kibana@sha256:a8a7325b2db4267d02371e9c03e747098734aec9b57477f8fa520ffab324e20e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.10.1` - linux; amd64

```console
$ docker pull kibana@sha256:d1faf8531d3029c028a76bcf01ad24c878fc940c2ca1155809e1fd1b2684a11a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.1 MB (377115505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec081fe34a45665608fc68b80473e3600c27ce60f298650537116e8e146ce5f2`
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
# Thu, 14 Sep 2023 23:57:18 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 14 Sep 2023 23:57:18 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 14 Sep 2023 23:57:21 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 14 Sep 2023 23:57:21 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 14 Sep 2023 23:57:22 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 14 Sep 2023 23:57:23 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 14 Sep 2023 23:57:23 GMT
RUN fc-cache -v # buildkit
# Thu, 14 Sep 2023 23:59:13 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 14 Sep 2023 23:59:13 GMT
WORKDIR /usr/share/kibana
# Thu, 14 Sep 2023 23:59:14 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 14 Sep 2023 23:59:14 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 14 Sep 2023 23:59:14 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 23:59:14 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 14 Sep 2023 23:59:14 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 14 Sep 2023 23:59:14 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 14 Sep 2023 23:59:15 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 14 Sep 2023 23:59:16 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 14 Sep 2023 23:59:16 GMT
LABEL org.label-schema.build-date=2023-09-14T23:20:42.888Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=6957ba896ec80fbaeaa269debfdce1478bdde661 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.10.1 org.opencontainers.image.created=2023-09-14T23:20:42.888Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=6957ba896ec80fbaeaa269debfdce1478bdde661 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.10.1
# Thu, 14 Sep 2023 23:59:16 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 14 Sep 2023 23:59:16 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 14 Sep 2023 23:59:16 GMT
USER kibana
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88c83457f775e5bb7b18e321875881753d4a7e60eb65d33cc6b63240113641b`  
		Last Modified: Mon, 18 Sep 2023 22:51:18 GMT  
		Size: 10.5 MB (10531753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa55d793dede38eeff8cd307d3fc4b3b7a1a14fae1768a1a3229e0c7c5b54e17`  
		Last Modified: Mon, 18 Sep 2023 22:49:37 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fd4d40338dcc0dd07c10be0758783094573f2b71f63d683a8f029b429c82df`  
		Last Modified: Mon, 18 Sep 2023 22:49:34 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4055a2a34aa522537e8e8532adcef122275b79e1b6824e00e5221b0e891de111`  
		Last Modified: Mon, 18 Sep 2023 22:51:28 GMT  
		Size: 16.5 MB (16460477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0afa4b4c6e326a92876ebc2f3921b676b677f4ef738b9670201ff7849af904`  
		Last Modified: Mon, 18 Sep 2023 22:49:30 GMT  
		Size: 5.3 KB (5302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24409d2c96054652308c6a97564af611c01ecfcea7dadbc3d838e378a8e970ae`  
		Last Modified: Mon, 18 Sep 2023 23:07:52 GMT  
		Size: 321.3 MB (321330832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4dafd6d791ed40e0d8a47c90eeef0c5a33eb0d0af9c14fec4a02931ed7f6cc`  
		Last Modified: Mon, 18 Sep 2023 22:49:28 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d1ba66a52cfb12793219f7e79e45ea71e5bfdead559c3c58c6f57fd563076b`  
		Last Modified: Mon, 18 Sep 2023 22:49:21 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65050c9b9ddf601399b59949fd243415903ccbaa137c31fa722edd7a9e71d907`  
		Last Modified: Mon, 18 Sep 2023 22:49:21 GMT  
		Size: 4.6 KB (4556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6533161b51dff5cae531c8c6477ba27a6040e76baa1a651f10101efc197dd41f`  
		Last Modified: Mon, 18 Sep 2023 22:49:21 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4ae6e71187bfc1b16f8437be3dd9cf85280fea4accb306d3c8d53a4409d8a5`  
		Last Modified: Mon, 18 Sep 2023 22:49:23 GMT  
		Size: 189.4 KB (189407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb742a3ec4c615a90d8b58e0e2bac918cb642cf94c5ffb1ca6400b7bcc0fd67`  
		Last Modified: Mon, 18 Sep 2023 22:49:21 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.10.1` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:5733834b4d466b35d87953a0bdd29f22d4513a4ee0df26b63f3d5cd25e31c627
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.6 MB (387643962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e2c2769485f712367a30ad520d1dc98c359983a52542986aa751247c0aeb49b`
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
# Fri, 15 Sep 2023 00:01:38 GMT
EXPOSE map[5601/tcp:{}]
# Fri, 15 Sep 2023 00:01:38 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Fri, 15 Sep 2023 00:01:40 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Fri, 15 Sep 2023 00:01:40 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Fri, 15 Sep 2023 00:01:43 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Fri, 15 Sep 2023 00:01:44 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Fri, 15 Sep 2023 00:01:44 GMT
RUN fc-cache -v # buildkit
# Fri, 15 Sep 2023 00:03:33 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Fri, 15 Sep 2023 00:03:33 GMT
WORKDIR /usr/share/kibana
# Fri, 15 Sep 2023 00:03:33 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Fri, 15 Sep 2023 00:03:33 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 15 Sep 2023 00:03:33 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Sep 2023 00:03:33 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Fri, 15 Sep 2023 00:03:34 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Fri, 15 Sep 2023 00:03:35 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Fri, 15 Sep 2023 00:03:36 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Fri, 15 Sep 2023 00:03:37 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Fri, 15 Sep 2023 00:03:37 GMT
LABEL org.label-schema.build-date=2023-09-14T23:20:42.888Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=6957ba896ec80fbaeaa269debfdce1478bdde661 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.10.1 org.opencontainers.image.created=2023-09-14T23:20:42.888Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=6957ba896ec80fbaeaa269debfdce1478bdde661 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.10.1
# Fri, 15 Sep 2023 00:03:37 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Fri, 15 Sep 2023 00:03:37 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Fri, 15 Sep 2023 00:03:37 GMT
USER kibana
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9839fbd6a6b1efbc8b043029c2041923ee75d4dca62057a97793ac855d81068a`  
		Last Modified: Tue, 19 Sep 2023 23:40:45 GMT  
		Size: 10.4 MB (10399347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b31187ce380544780504672b8d03e44f9206daef48152ddfd74bc816ccbcd8`  
		Last Modified: Tue, 19 Sep 2023 23:40:42 GMT  
		Size: 9.1 KB (9098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa8a51e970bdaa04ac4f6b84ed234ad0d3ee22dd49a700ed851d642f3da6622`  
		Last Modified: Tue, 19 Sep 2023 23:40:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5f13500df63c888f09ed3de61f2f57fc22974eab7e467dc9b38d9112f644d9`  
		Last Modified: Tue, 19 Sep 2023 23:40:41 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09a85dd6e9fab759a7e680b147c7d5c7024fb1ee8888e54f25a9fea7fc91e22`  
		Last Modified: Tue, 19 Sep 2023 23:40:40 GMT  
		Size: 5.3 KB (5295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8d235e78a1f5e8d48c980af4c1cb4d45249a06d39bc3f93c7f95530d995fb0`  
		Last Modified: Tue, 19 Sep 2023 23:41:13 GMT  
		Size: 333.4 MB (333378195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e6dc0f802231425290a86fba3714ee5468bf6190371d4638cc0488beee173c`  
		Last Modified: Tue, 19 Sep 2023 23:40:40 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e5a45a30103bd7f02a7ff51d4c02f2826191abd452ff92ca25cd18945bbb85`  
		Last Modified: Tue, 19 Sep 2023 23:40:37 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a265232c62903bfd8c1f0742b469445d6b302aa43c2e37dba7186770e805f6e6`  
		Last Modified: Tue, 19 Sep 2023 23:40:37 GMT  
		Size: 4.6 KB (4556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd9ca4c46d9d9a787adf6a8aa4cd255f0e6be589b4ca57d6409a42a9bceac3`  
		Last Modified: Tue, 19 Sep 2023 23:40:37 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75a388f5b9abb00938a19461b716022edb082c1bd2cce135af791a592271d3e`  
		Last Modified: Tue, 19 Sep 2023 23:40:38 GMT  
		Size: 183.4 KB (183412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6787dad75ec6e9ca403b9b379de9c7fad612f264555e9b6bce7c11c8b880b68`  
		Last Modified: Tue, 19 Sep 2023 23:40:41 GMT  
		Size: 1.8 KB (1829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
