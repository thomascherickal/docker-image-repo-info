<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.13`](#kibana71713)
-	[`kibana:8.9.2`](#kibana892)

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

## `kibana:8.9.2`

```console
$ docker pull kibana@sha256:82209b3ed176ffa5996752c98a58715777e864f9e00592a4521e71f7fc15f5a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.9.2` - linux; amd64

```console
$ docker pull kibana@sha256:14a00c1fec6f55d0ff39ec298be6c1cd2a432046ebabf754a87c981f8aaa0def
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354863155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:728f0908ac21475170879456f7009d1407d6b94ee97162062f47ab07717f7292`
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
# Wed, 30 Aug 2023 22:40:34 GMT
EXPOSE map[5601/tcp:{}]
# Wed, 30 Aug 2023 22:40:34 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Wed, 30 Aug 2023 22:40:35 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Wed, 30 Aug 2023 22:40:35 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Wed, 30 Aug 2023 22:40:36 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Wed, 30 Aug 2023 22:40:37 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Wed, 30 Aug 2023 22:40:37 GMT
RUN fc-cache -v # buildkit
# Wed, 30 Aug 2023 22:42:12 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Wed, 30 Aug 2023 22:42:12 GMT
WORKDIR /usr/share/kibana
# Wed, 30 Aug 2023 22:42:12 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Wed, 30 Aug 2023 22:42:12 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 30 Aug 2023 22:42:12 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Aug 2023 22:42:12 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Wed, 30 Aug 2023 22:42:12 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Wed, 30 Aug 2023 22:42:13 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Wed, 30 Aug 2023 22:42:14 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Wed, 30 Aug 2023 22:42:14 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Wed, 30 Aug 2023 22:42:14 GMT
LABEL org.label-schema.build-date=2023-08-30T22:08:39.111Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=21f3ebd6e951d102f41b0299c35e030c3c9e8eb6 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.9.2 org.opencontainers.image.created=2023-08-30T22:08:39.111Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=21f3ebd6e951d102f41b0299c35e030c3c9e8eb6 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.9.2
# Wed, 30 Aug 2023 22:42:14 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 30 Aug 2023 22:42:14 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Wed, 30 Aug 2023 22:42:14 GMT
USER kibana
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9224d6036826713ba13034485533a13ebfc7c1292c3504867eeca352123344d`  
		Last Modified: Fri, 08 Sep 2023 05:24:11 GMT  
		Size: 10.5 MB (10531719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab9f5e7c3a09a46157735bbb362cb98be85b4c71243fc1167926395939d686b`  
		Last Modified: Fri, 08 Sep 2023 05:24:08 GMT  
		Size: 9.5 KB (9524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb4a46d4b8b8d694a8debc05a7af83a7bbd77abc233d8be16b3ff62b11504dc`  
		Last Modified: Fri, 08 Sep 2023 05:24:08 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc11a3b790f8ff7186f86442cf5327f6fc35232fa2e9c53e9178c54bdc4fec9e`  
		Last Modified: Fri, 08 Sep 2023 05:24:07 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e2e1617de051cf10352e6fdcb1df7d943f7d7ac324dd32a68fdf5ef590618b`  
		Last Modified: Fri, 08 Sep 2023 05:24:05 GMT  
		Size: 5.3 KB (5286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148a02e57092ce22b3f7ebaa2c46f00ab513ed1ed2d2f72ee8c5ed1e7f1506fb`  
		Last Modified: Fri, 08 Sep 2023 05:24:43 GMT  
		Size: 299.1 MB (299078533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1439cc5d42a8a26659eb8f7b61702ccbaf51b64c5a64c70945924be695517090`  
		Last Modified: Fri, 08 Sep 2023 05:24:05 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b9defbe431726a88686c6a5a43ffdaa84f319dd36d6cd5317f1fd28ea8e34d`  
		Last Modified: Fri, 08 Sep 2023 05:24:03 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30dcd50c893de3d6ae77f7c6afafefb0da1ee755e4e761cb35088a4154ccff`  
		Last Modified: Fri, 08 Sep 2023 05:24:03 GMT  
		Size: 4.6 KB (4553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c19fd98eea3591d5ca89dbaddbfaec30bc2a5f8070994d585af147651cde09`  
		Last Modified: Fri, 08 Sep 2023 05:24:03 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3c202b2952e923bc23255c63b62a0bfbc4a007ea8a09f8840d7a5f589459ac`  
		Last Modified: Fri, 08 Sep 2023 05:24:03 GMT  
		Size: 189.4 KB (189404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bdb1052b9d6f556c606decc4496be5df4c030b508f201b6d9cbd356b25d51d`  
		Last Modified: Fri, 08 Sep 2023 05:24:08 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.9.2` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:3cb1d9619bfab0d451c72caedca550698d02713d21b87746b81eea3ea89c3b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.3 MB (366268520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:260b2537bf80975e954222ec7c44ad76ff9c2f44b5991845c3f6a39dbbb98da9`
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
# Wed, 30 Aug 2023 22:44:27 GMT
EXPOSE map[5601/tcp:{}]
# Wed, 30 Aug 2023 22:44:27 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Wed, 30 Aug 2023 22:44:29 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Wed, 30 Aug 2023 22:44:29 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Wed, 30 Aug 2023 22:44:32 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Wed, 30 Aug 2023 22:44:33 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Wed, 30 Aug 2023 22:44:33 GMT
RUN fc-cache -v # buildkit
# Wed, 30 Aug 2023 22:46:07 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Wed, 30 Aug 2023 22:46:07 GMT
WORKDIR /usr/share/kibana
# Wed, 30 Aug 2023 22:46:07 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Wed, 30 Aug 2023 22:46:07 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 30 Aug 2023 22:46:07 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Aug 2023 22:46:07 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Wed, 30 Aug 2023 22:46:07 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Wed, 30 Aug 2023 22:46:08 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Wed, 30 Aug 2023 22:46:10 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Wed, 30 Aug 2023 22:46:10 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Wed, 30 Aug 2023 22:46:10 GMT
LABEL org.label-schema.build-date=2023-08-30T22:08:39.111Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=21f3ebd6e951d102f41b0299c35e030c3c9e8eb6 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.9.2 org.opencontainers.image.created=2023-08-30T22:08:39.111Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=21f3ebd6e951d102f41b0299c35e030c3c9e8eb6 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.9.2
# Wed, 30 Aug 2023 22:46:10 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 30 Aug 2023 22:46:10 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Wed, 30 Aug 2023 22:46:10 GMT
USER kibana
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a681bd6a2e67cc1665939c0ff50d2b6f8d7d36578e6b34ec82938ff47df0114e`  
		Last Modified: Thu, 07 Sep 2023 23:40:54 GMT  
		Size: 10.4 MB (10399393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8940e828831a853a279df933e65c8cd6e3d85691583f16a5d8d5fd57ec5e8b85`  
		Last Modified: Thu, 07 Sep 2023 23:40:51 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbd0a6857817b104a7c2b791ae34477aa22b1e5e4000494b113e091300d1f04`  
		Last Modified: Thu, 07 Sep 2023 23:40:51 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbc692af8f6c570d4db711cb1ae213ba5ade084b4451b2eec1381cf0da9460d`  
		Last Modified: Thu, 07 Sep 2023 23:40:51 GMT  
		Size: 16.5 MB (16460476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd0dd5e0418bd9c7a8c3f9e812c53b126023088a0e19b604f1850bde16f6f8f`  
		Last Modified: Thu, 07 Sep 2023 23:40:50 GMT  
		Size: 5.3 KB (5308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2accd15e44a59b5a04ad9a6b106ff3fa12c058e049586a941280226bffb30f2`  
		Last Modified: Thu, 07 Sep 2023 23:41:20 GMT  
		Size: 312.0 MB (312002720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e48396b49f5c75a23c8ff4905dc8716955045496ff124f72719b3a2f0d1a84c`  
		Last Modified: Thu, 07 Sep 2023 23:40:49 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c544202975714672d393b25cbd5e749affdf4660b3f66e11415ceafe3dd512`  
		Last Modified: Thu, 07 Sep 2023 23:40:47 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d859a53b5c98f02c28d3e40af98538239cc9ee3c90ca0536179631829fe184f7`  
		Last Modified: Thu, 07 Sep 2023 23:40:47 GMT  
		Size: 4.6 KB (4551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3adb45c185486e1a32783fbd6d1d8e2a7400aa6999a30ae6add488e98f970e`  
		Last Modified: Thu, 07 Sep 2023 23:40:47 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc4de32086bc6f2037579bf18353fa6537e2b5374d15c59d6c979a1b6e20bbc`  
		Last Modified: Thu, 07 Sep 2023 23:40:47 GMT  
		Size: 183.4 KB (183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4037b814c89b46f73642a778da49afb22ba3bc14af54be2cfcf113d541c1210c`  
		Last Modified: Thu, 07 Sep 2023 23:40:49 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
