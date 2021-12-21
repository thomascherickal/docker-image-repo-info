<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.22`](#kibana6822)
-	[`kibana:7.16.2`](#kibana7162)

## `kibana:6.8.22`

```console
$ docker pull kibana@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `kibana:7.16.2`

```console
$ docker pull kibana@sha256:002c1867d3198e69fa17fa616b3d25f0ac49fa3d7263e8c950b66ff9c9c92a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `kibana:7.16.2` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:f4bbb4e68162da8d7b492294e5fbdb8af96fe9149b3f844445b530695327665e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **495.6 MB (495590403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bcb4cae919c78fe2a75fbe77f711ca3f8de0829edf9c5ce23928ee2e23a4e2f`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 15 Sep 2021 17:39:41 GMT
ADD file:420712a90b0934202b326dc06b73638ab8e4603d12be2c23d67d834eb6cfc052 in / 
# Wed, 15 Sep 2021 17:39:42 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 17:39:42 GMT
CMD ["/bin/bash"]
# Sat, 18 Dec 2021 22:08:36 GMT
EXPOSE 5601
# Sat, 18 Dec 2021 22:09:44 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y         fontconfig freetype shadow-utils nss  &&       yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Sat, 18 Dec 2021 22:09:48 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Sat, 18 Dec 2021 22:09:48 GMT
RUN mkdir /usr/share/fonts/local
# Sat, 18 Dec 2021 22:09:51 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Sat, 18 Dec 2021 22:09:52 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Sat, 18 Dec 2021 22:09:52 GMT
RUN fc-cache -v
# Sat, 18 Dec 2021 22:10:28 GMT
COPY --chown=1000:0dir:718a2dbb286ac29dec3fe8a243c2f9f57d62d3d3f3934b7b80ba3415274ca584 in /usr/share/kibana 
# Sat, 18 Dec 2021 22:10:32 GMT
WORKDIR /usr/share/kibana
# Sat, 18 Dec 2021 22:10:33 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Sat, 18 Dec 2021 22:10:33 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 18 Dec 2021 22:10:33 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Dec 2021 22:10:33 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Sat, 18 Dec 2021 22:10:33 GMT
COPY file:4b05cc4ee8dc464b192dc25102b9385329fd96ca9e48428d3b36b7d2a9e4be58 in /usr/local/bin/ 
# Sat, 18 Dec 2021 22:10:35 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Sat, 18 Dec 2021 22:10:37 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Sat, 18 Dec 2021 22:10:37 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Sat, 18 Dec 2021 22:10:38 GMT
LABEL org.label-schema.build-date=2021-12-18T22:05:22.047Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=9b678a13a6a3f45286f1d21856a7536a9297f42f org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.16.2 org.opencontainers.image.created=2021-12-18T22:05:22.047Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=9b678a13a6a3f45286f1d21856a7536a9297f42f org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.16.2
# Sat, 18 Dec 2021 22:10:38 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Sat, 18 Dec 2021 22:10:38 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Sat, 18 Dec 2021 22:10:38 GMT
USER kibana
```

-	Layers:
	-	`sha256:52f9ef134af7dd14738733e567402af86136287d9468978d044780a6435a1193`  
		Last Modified: Wed, 15 Sep 2021 17:40:42 GMT  
		Size: 83.9 MB (83941353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d829adaecdb949e43a3b99ef3339f4ac7d12e099d47a74da453d78e6d60045e`  
		Last Modified: Tue, 21 Dec 2021 00:41:45 GMT  
		Size: 94.4 MB (94358467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b147794101787503976957feb3fffd8db270796c37a316f5d05a7850280edc63`  
		Last Modified: Tue, 21 Dec 2021 00:41:30 GMT  
		Size: 9.1 KB (9094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a948fe82120e296f1917e7d9342b88a3566604248a28e906f1c40a4a926ecde5`  
		Last Modified: Tue, 21 Dec 2021 00:41:28 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96d1fad6c1bafeab0e55c54e972f2367d8d36b23e1b8c61e6a44875ce96558`  
		Last Modified: Tue, 21 Dec 2021 00:41:30 GMT  
		Size: 16.5 MB (16460491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8fdff7556f49ae62ccc1c570fd7e72e1e946f18c346711309df38a26a4084a`  
		Last Modified: Tue, 21 Dec 2021 00:41:28 GMT  
		Size: 8.3 KB (8304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4029b7de6ab4bd2c15ab75925a8966754c37d4b22d8b4c16926b983332d42c`  
		Last Modified: Tue, 21 Dec 2021 00:42:08 GMT  
		Size: 300.6 MB (300607965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fede2c4304b2e977a4dd8cdb3775ca61217e0f4527d5d51f6f7136dd70d714a`  
		Last Modified: Tue, 21 Dec 2021 00:41:27 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f363a710f54e9dbf00dd0a5016cb6e597265f77171a0b58c8a62cbf927719ef`  
		Last Modified: Tue, 21 Dec 2021 00:41:25 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c210b27217b62c89ffea4e21bc369effabbc4eb32052c0a95aadfdc9a9e0f254`  
		Last Modified: Tue, 21 Dec 2021 00:41:25 GMT  
		Size: 4.5 KB (4488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e18d34b40ff579d6344a33b757accd4a972ea301b3498d9f6145288159b49b`  
		Last Modified: Tue, 21 Dec 2021 00:41:25 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c47c30ffbd5d06082539eab2ac369582cfc54e041f41ba7de6aac288b523db`  
		Last Modified: Tue, 21 Dec 2021 00:41:25 GMT  
		Size: 197.2 KB (197249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edf0f691bad3fee4180726abadcd314c6ac76e8ceb8d9813a7430ae851fbd72`  
		Last Modified: Tue, 21 Dec 2021 00:41:25 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
