<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.23`](#kibana6823)
-	[`kibana:7.16.3`](#kibana7163)

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

## `kibana:7.16.3`

```console
$ docker pull kibana@sha256:a9bb1d796ca13a9d658c7ca4e3ca78ec555e532256ee3246addcf7606cc55527
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.16.3` - linux; amd64

```console
$ docker pull kibana@sha256:6ec603a4582b930ee5c1cd8c03ac77327fcbe1c7bdc3e58829d884c21d160df9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **480.8 MB (480774472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df64a680d59063159ca7e671a615b184d41b7e6fb0deb66ae508f09e2a4e1dfc`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Fri, 07 Jan 2022 00:10:45 GMT
EXPOSE 5601
# Fri, 07 Jan 2022 00:11:31 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y         fontconfig freetype shadow-utils nss  &&       yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Fri, 07 Jan 2022 00:11:34 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Fri, 07 Jan 2022 00:11:35 GMT
RUN mkdir /usr/share/fonts/local
# Fri, 07 Jan 2022 00:11:36 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Fri, 07 Jan 2022 00:11:37 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Fri, 07 Jan 2022 00:11:37 GMT
RUN fc-cache -v
# Fri, 07 Jan 2022 00:12:05 GMT
COPY --chown=1000:0dir:bbe5f270f484e39d3d8fb4237b50b26d742a33ad595751093ad07bab9c2dae5d in /usr/share/kibana 
# Fri, 07 Jan 2022 00:12:15 GMT
WORKDIR /usr/share/kibana
# Fri, 07 Jan 2022 00:12:16 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Fri, 07 Jan 2022 00:12:16 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 07 Jan 2022 00:12:16 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 00:12:16 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Fri, 07 Jan 2022 00:12:16 GMT
COPY file:4b05cc4ee8dc464b192dc25102b9385329fd96ca9e48428d3b36b7d2a9e4be58 in /usr/local/bin/ 
# Fri, 07 Jan 2022 00:12:18 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Fri, 07 Jan 2022 00:12:19 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Fri, 07 Jan 2022 00:12:20 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Fri, 07 Jan 2022 00:12:20 GMT
LABEL org.label-schema.build-date=2022-01-06T23:17:40.113Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=33b4188edcdda8e9636e397d3832a98bc7dcbae3 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.16.3 org.opencontainers.image.created=2022-01-06T23:17:40.113Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=33b4188edcdda8e9636e397d3832a98bc7dcbae3 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.16.3
# Fri, 07 Jan 2022 00:12:20 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Fri, 07 Jan 2022 00:12:20 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Fri, 07 Jan 2022 00:12:20 GMT
USER kibana
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece649e3968877b1cd767d74eac75a87006d4a2a9a25f04e42b644442b28f227`  
		Last Modified: Thu, 13 Jan 2022 19:08:09 GMT  
		Size: 94.4 MB (94423594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd6b9c45632f14db5444b9c8b73e465393962e4846f88138b00a53f3b7574bf`  
		Last Modified: Thu, 13 Jan 2022 19:07:40 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c7b1b7aa2e61c8da59787232fac30825f0f3aae0bc4b5905e69b05ca4334cf`  
		Last Modified: Thu, 13 Jan 2022 19:07:38 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a203df98829e43e468b540ba36dd34a8b95d31a529fc51eb1b4ed9f9732485`  
		Last Modified: Thu, 13 Jan 2022 19:07:40 GMT  
		Size: 16.5 MB (16460496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95f2a43b95a0c1c5e71f4bdc9fed21c5e3d65836a7d761ac0cc776a02ba45ea`  
		Last Modified: Thu, 13 Jan 2022 19:07:37 GMT  
		Size: 8.3 KB (8260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30179b8b9d9c502c4c0c7cc9ccf962b3f9c58cfbfb7b819ce171ae8d159aba78`  
		Last Modified: Thu, 13 Jan 2022 19:08:38 GMT  
		Size: 286.2 MB (286150589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135351880c104dbe226bf7e7f4d94910c1cf2e716641c3749edf842fbd173df8`  
		Last Modified: Thu, 13 Jan 2022 19:07:37 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f6f09b28632494b3f7302e0be7f6f6da0daef19d85cb1e12dc05d0cc8d25a6`  
		Last Modified: Thu, 13 Jan 2022 19:07:35 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b6675fb6111310d55665bb536bc28145a8b13bf894c14d53b90b4e08ed8163`  
		Last Modified: Thu, 13 Jan 2022 19:07:34 GMT  
		Size: 4.5 KB (4489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f7787dea6306e632ace47017732bed1f37107a530d25fc8cc43336d55cc915`  
		Last Modified: Thu, 13 Jan 2022 19:07:34 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6cee7acae6df6ccfa56c48b802e3f301c92de9154345761ed37cb3cc763cb3`  
		Last Modified: Thu, 13 Jan 2022 19:07:34 GMT  
		Size: 196.4 KB (196449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202ad6edd4a0b370db2d38ac5d3be569bd9ee6b93d6a65220c48e2c63e5101f7`  
		Last Modified: Thu, 13 Jan 2022 19:07:34 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.16.3` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:59ed297f693f890f543beb3041101a2c8b7720fcba10febe743cd29b730e3338
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **495.7 MB (495748103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e1333a1fb27bc05fff821f581cbe2c78e39e295c648a0e70afc0bad5046046c`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 15 Sep 2021 17:39:41 GMT
ADD file:420712a90b0934202b326dc06b73638ab8e4603d12be2c23d67d834eb6cfc052 in / 
# Wed, 15 Sep 2021 17:39:42 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 17:39:42 GMT
CMD ["/bin/bash"]
# Fri, 07 Jan 2022 01:44:57 GMT
EXPOSE 5601
# Fri, 07 Jan 2022 01:46:10 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y         fontconfig freetype shadow-utils nss  &&       yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Fri, 07 Jan 2022 01:46:14 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Fri, 07 Jan 2022 01:46:15 GMT
RUN mkdir /usr/share/fonts/local
# Fri, 07 Jan 2022 01:46:23 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Fri, 07 Jan 2022 01:46:24 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Fri, 07 Jan 2022 01:46:25 GMT
RUN fc-cache -v
# Fri, 07 Jan 2022 01:47:03 GMT
COPY --chown=1000:0dir:f36323a73c1419b11a8eab7189c8aa46bcaad3343c3bdca39e22afce41f7010d in /usr/share/kibana 
# Fri, 07 Jan 2022 01:47:17 GMT
WORKDIR /usr/share/kibana
# Fri, 07 Jan 2022 01:47:17 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Fri, 07 Jan 2022 01:47:17 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 07 Jan 2022 01:47:18 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 01:47:18 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Fri, 07 Jan 2022 01:47:18 GMT
COPY file:4b05cc4ee8dc464b192dc25102b9385329fd96ca9e48428d3b36b7d2a9e4be58 in /usr/local/bin/ 
# Fri, 07 Jan 2022 01:47:19 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Fri, 07 Jan 2022 01:47:21 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Fri, 07 Jan 2022 01:47:22 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Fri, 07 Jan 2022 01:47:22 GMT
LABEL org.label-schema.build-date=2022-01-07T01:40:23.503Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=33b4188edcdda8e9636e397d3832a98bc7dcbae3 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.16.3 org.opencontainers.image.created=2022-01-07T01:40:23.503Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=33b4188edcdda8e9636e397d3832a98bc7dcbae3 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.16.3
# Fri, 07 Jan 2022 01:47:22 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Fri, 07 Jan 2022 01:47:22 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Fri, 07 Jan 2022 01:47:22 GMT
USER kibana
```

-	Layers:
	-	`sha256:52f9ef134af7dd14738733e567402af86136287d9468978d044780a6435a1193`  
		Last Modified: Wed, 15 Sep 2021 17:40:42 GMT  
		Size: 83.9 MB (83941353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218880aa1396fb8caaa0fa3c06b891dfcb590b0e115e4f46e0fe46b38e2d8b4e`  
		Last Modified: Fri, 14 Jan 2022 01:41:36 GMT  
		Size: 94.3 MB (94348610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1191274aa6f43a952b0f22866b313d2d163629207d6caac3330d24910186bcd`  
		Last Modified: Fri, 14 Jan 2022 01:41:21 GMT  
		Size: 9.1 KB (9094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469445f08222c2eed8a7bd0d7e71f9526eaa17c9431fb47d75bfaf67e61ccef6`  
		Last Modified: Fri, 14 Jan 2022 01:41:19 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3ec0ed6eaceeab0c00e9d364053b4b6f007caabcf9a2401593e9dd651fc0c0`  
		Last Modified: Fri, 14 Jan 2022 01:41:21 GMT  
		Size: 16.5 MB (16460477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f238123265b55e987cd7b47e785a633173119769cc61acc7c8591cb275bc1df`  
		Last Modified: Fri, 14 Jan 2022 01:41:18 GMT  
		Size: 8.3 KB (8260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdc7d8e9e436d082ef37e1fe9dccae4b5e70af10a8b164319f63ca78042b73b`  
		Last Modified: Fri, 14 Jan 2022 01:42:00 GMT  
		Size: 300.8 MB (300775590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ad0f3536ffb37443852e8ae6198418d3a8643e04dbe8a3c1558a060e2a6d32`  
		Last Modified: Fri, 14 Jan 2022 01:41:18 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85e271bd92e4f5e40b96967db22a5762debb89b4af694ae9ff977bd317f2b9`  
		Last Modified: Fri, 14 Jan 2022 01:41:16 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96da6594fbfd3b933a06d00c08d0a7c0578a96011f387ab4c067d5163825c1ff`  
		Last Modified: Fri, 14 Jan 2022 01:41:16 GMT  
		Size: 4.5 KB (4486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223f3c2384373a1b2fc9e68467e0cb69bbd9072445e6fff562b878a887605d7a`  
		Last Modified: Fri, 14 Jan 2022 01:41:16 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec58fd683b481039b69add0dd93bf7d338c411506be4ee8a7c1028588a0d475`  
		Last Modified: Fri, 14 Jan 2022 01:41:16 GMT  
		Size: 197.2 KB (197248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448000858e50e0ad71173ce118f157aea338fb197ef68d2fe8870f7dd5473c52`  
		Last Modified: Fri, 14 Jan 2022 01:41:16 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
