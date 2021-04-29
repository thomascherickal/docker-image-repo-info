<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.15`](#kibana6815)
-	[`kibana:7.12.1`](#kibana7121)

## `kibana:6.8.15`

```console
$ docker pull kibana@sha256:38ffc2983bcd8cdb8c7f95e3a3c6738ef1bf499626cb6cdc35bfd51a1c6ccc27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kibana:6.8.15` - linux; amd64

```console
$ docker pull kibana@sha256:5c1c8ed95ebecf6d18411cf1f170900745f7f0f9fd1c064ef6ab59d5ee54d95f
```

-	Docker Version: 20.10.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.6 MB (314626486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4a537fe34abc5fbfcede68ae38ca51b9455879ff505d9d7cb0e13efc71e05c6`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 07:49:24 GMT
EXPOSE 5601
# Thu, 18 Mar 2021 07:50:12 GMT
RUN yum update -y && yum install -y fontconfig freetype && yum clean all
# Thu, 18 Mar 2021 07:50:58 GMT
COPY --chown=1000:0dir:a3b754e1ecd28b83226d08d7d4eb4d0bfb72949bf2994f298eaae6c5551583fd in /usr/share/kibana 
# Thu, 18 Mar 2021 07:51:00 GMT
WORKDIR /usr/share/kibana
# Thu, 18 Mar 2021 07:51:01 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 18 Mar 2021 07:51:02 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 18 Mar 2021 07:51:02 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Mar 2021 07:51:03 GMT
COPY --chown=1000:0file:60b6181f28c99b362092ea6139b6d4112ddd0bef32d52563c33b26bdc2b51318 in /usr/share/kibana/config/kibana.yml 
# Thu, 18 Mar 2021 07:51:03 GMT
COPY --chown=1000:0file:7d472d1939e23e2f10e7c5fd1e9166eefd646214aa0d8a1c09d92af71c9cbd87 in /usr/local/bin/ 
# Thu, 18 Mar 2021 07:51:06 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 18 Mar 2021 07:51:08 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Thu, 18 Mar 2021 07:51:09 GMT
USER kibana
# Thu, 18 Mar 2021 07:51:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=6.8.15 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License license=Elastic License
# Thu, 18 Mar 2021 07:51:10 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b5fe0e7184ef1f08feb2eab326b3c15480614fe92c59082059dc7320a3afb5`  
		Last Modified: Tue, 23 Mar 2021 13:50:35 GMT  
		Size: 48.7 MB (48744206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68a75e92c26a03c79ae2cee282983b7e0cdc9454cc5cdc957264a0c114d071f`  
		Last Modified: Tue, 23 Mar 2021 13:50:51 GMT  
		Size: 189.8 MB (189780368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a240b339bd1bd4fa8fb16efd281d7051c59b1b7d4f39c1bbeea862f0093c812c`  
		Last Modified: Tue, 23 Mar 2021 13:50:24 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee4772120b1dbf5184da996b9d97a9112aed558fdf4602cbea1ef8bbe24c693`  
		Last Modified: Tue, 23 Mar 2021 13:50:23 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cedb5e5b853d97389f038e432a7967e7da566c715b56ecfbcc2a3b1509d144ab`  
		Last Modified: Tue, 23 Mar 2021 13:50:21 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e4d1664c7d2285d5e800f0d51b9c0d1d56fc0fb515a7906e1a37aad063a50`  
		Last Modified: Tue, 23 Mar 2021 13:50:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e397c49c6ec70d0a7084fef0a9009f83ab0441a92dfeae06fc213e7a7cfe178c`  
		Last Modified: Tue, 23 Mar 2021 13:50:17 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:7.12.1`

```console
$ docker pull kibana@sha256:e96f8b6a90db0b4ba804f7023922448a1d752a85e77f6c645ec309fa0328627d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kibana:7.12.1` - linux; amd64

```console
$ docker pull kibana@sha256:db88d7069c91b586dbef1c518e33cd527b649caf0002c3976c3323faf04314c2
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.6 MB (413593936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1c9961eeb6ad29607c1b409396eada508171e95b9fdd9ace3710959fd65fb6`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 21:09:16 GMT
EXPOSE 5601
# Tue, 20 Apr 2021 21:09:59 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y         fontconfig freetype shadow-utils nss  &&       yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Tue, 20 Apr 2021 21:10:01 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Tue, 20 Apr 2021 21:10:02 GMT
RUN mkdir /usr/share/fonts/local
# Tue, 20 Apr 2021 21:10:04 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Tue, 20 Apr 2021 21:10:05 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Tue, 20 Apr 2021 21:10:05 GMT
RUN fc-cache -v
# Tue, 20 Apr 2021 21:10:36 GMT
COPY --chown=1000:0dir:19afbc2b0fb7e992851a5a431dbcfc0c8a3a7347420f37316416e966aa484132 in /usr/share/kibana 
# Tue, 20 Apr 2021 21:10:40 GMT
WORKDIR /usr/share/kibana
# Tue, 20 Apr 2021 21:10:41 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Tue, 20 Apr 2021 21:10:41 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 20 Apr 2021 21:10:41 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Apr 2021 21:10:41 GMT
COPY --chown=1000:0file:6327494502800698df48e00f1f91972c882c036b3fda354262515e3410c28d4a in /usr/share/kibana/config/kibana.yml 
# Tue, 20 Apr 2021 21:10:42 GMT
COPY --chown=1000:0file:3aafe9409fcd13028381b6c5dbcdd7342a470fb82e693e30156d50e1e02e6a23 in /usr/local/bin/ 
# Tue, 20 Apr 2021 21:10:43 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Tue, 20 Apr 2021 21:10:45 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Tue, 20 Apr 2021 21:10:46 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Tue, 20 Apr 2021 21:10:46 GMT
LABEL org.label-schema.build-date=2021-04-20T20:04:40.463Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=abb04c5543d2201630c9669fe3680864506d924e org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.12.1 org.opencontainers.image.created=2021-04-20T20:04:40.463Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=abb04c5543d2201630c9669fe3680864506d924e org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.12.1
# Tue, 20 Apr 2021 21:10:46 GMT
USER kibana
# Tue, 20 Apr 2021 21:10:46 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Tue, 20 Apr 2021 21:10:46 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a86526e9ebe966aca5405891e60960be2d3e2e5fc7eadc5c425e7159b6eda5b`  
		Last Modified: Tue, 27 Apr 2021 17:28:36 GMT  
		Size: 36.0 MB (36023380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bdbe52f520531d1fea6114aa2f8d81f2ae8c886167565c69d2f3a2f6e317ba`  
		Last Modified: Tue, 27 Apr 2021 17:28:27 GMT  
		Size: 9.5 KB (9532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3544177b28bb04b1d16b54c26cfa266898d0b1e5289dc2ba1798328c03770af`  
		Last Modified: Tue, 27 Apr 2021 17:28:24 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c4924dea71fe6a45eb8cd631fe7fe5d910ffb5250694a95ea3fd327dcfb31d`  
		Last Modified: Tue, 27 Apr 2021 17:28:25 GMT  
		Size: 16.5 MB (16460488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b707397fb84b2d68b9676a845266d2d27c6f2e799775bfa4f0b2d88b235884`  
		Last Modified: Tue, 27 Apr 2021 17:28:23 GMT  
		Size: 8.3 KB (8307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe176c615c8395c6d82924a4ed4a38b72077d2f70b8022ddee4427164428dc40`  
		Last Modified: Tue, 27 Apr 2021 17:29:01 GMT  
		Size: 285.7 MB (285707298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d370300ee0202e70f648addca828e22b459e742a59da82a97c796a5b021779`  
		Last Modified: Tue, 27 Apr 2021 17:28:23 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ddea056c28775f22158c155647f98939373453b84fd8bc2d39422b210454eb`  
		Last Modified: Tue, 27 Apr 2021 17:28:19 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb9e99363e1af7da844a61b7ab7ba6acc85bd617a4e369339feeb4b187061d6`  
		Last Modified: Tue, 27 Apr 2021 17:28:19 GMT  
		Size: 3.6 KB (3581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c6179eff482e167367e0618c91405fb907d866c6ced122c1bad625848b1a15`  
		Last Modified: Tue, 27 Apr 2021 17:28:20 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419632bc6dfe4e9df8e87e579b95c0ff4367bd6a1aa8e367cd7e2db6dd5fd2d1`  
		Last Modified: Tue, 27 Apr 2021 17:28:19 GMT  
		Size: 196.4 KB (196391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c05d50f8ca5814633dae468d1fc9e570fe497b4d86cb17e6a738f7073160c1b`  
		Last Modified: Tue, 27 Apr 2021 17:28:19 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
