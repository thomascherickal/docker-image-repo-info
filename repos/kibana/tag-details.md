<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.13`](#kibana71713)
-	[`kibana:8.9.2`](#kibana892)

## `kibana:7.17.13`

```console
$ docker pull kibana@sha256:c96bb821705aa2a203e45622b67d8cc4009d401aeb97049333ea75da654c4a41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

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
$ docker pull kibana@sha256:646be2c3cebb8d6eb10488bcf957a3ce56bf580edd5a5e3f5662e4d9daabe480
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

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
