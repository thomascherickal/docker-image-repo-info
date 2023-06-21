<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.10`](#kibana71710)
-	[`kibana:8.8.1`](#kibana881)

## `kibana:7.17.10`

```console
$ docker pull kibana@sha256:85f56231725dfb4a2663388fa8343926de043e5ce05e787e6fbc965eac0c3b3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.17.10` - linux; amd64

```console
$ docker pull kibana@sha256:d829548dd28a5cc3f3aa0879800f43ac47d4a823cde01c5e7adc25d8c5d8cf67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.1 MB (329056301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4afcebad69491d5947eaa1a23061e0628e73200d4f3b57029d932467652448`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Sat, 22 Apr 2023 11:37:09 GMT
EXPOSE map[5601/tcp:{}]
# Sat, 22 Apr 2023 11:37:09 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Sat, 22 Apr 2023 11:37:11 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Sat, 22 Apr 2023 11:37:12 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Sat, 22 Apr 2023 11:37:13 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Sat, 22 Apr 2023 11:37:14 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Sat, 22 Apr 2023 11:37:14 GMT
RUN fc-cache -v # buildkit
# Sat, 22 Apr 2023 11:38:22 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Sat, 22 Apr 2023 11:38:22 GMT
WORKDIR /usr/share/kibana
# Sat, 22 Apr 2023 11:38:22 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Sat, 22 Apr 2023 11:38:22 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 22 Apr 2023 11:38:22 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Apr 2023 11:38:22 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Sat, 22 Apr 2023 11:38:22 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Sat, 22 Apr 2023 11:38:23 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Sat, 22 Apr 2023 11:38:23 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Sat, 22 Apr 2023 11:38:24 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Sat, 22 Apr 2023 11:38:24 GMT
LABEL org.label-schema.build-date=2023-04-22T11:11:10.120Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=6f79ab09449019d2b5e02ad4508375b5ee56e421 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.10 org.opencontainers.image.created=2023-04-22T11:11:10.120Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=6f79ab09449019d2b5e02ad4508375b5ee56e421 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.10
# Sat, 22 Apr 2023 11:38:24 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Sat, 22 Apr 2023 11:38:24 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Sat, 22 Apr 2023 11:38:24 GMT
USER kibana
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b833df53080f938d89a331a5c9c8e28dbbb19c7651c7ed76095acc3e8ec0fe9`  
		Last Modified: Wed, 03 May 2023 04:12:06 GMT  
		Size: 10.5 MB (10511426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f550a4d40b253a3a084b6cbf7cb9e8749cb5f470c2e54d28aad8f420ff25781`  
		Last Modified: Wed, 03 May 2023 04:12:04 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db648d59d34ecc0d0be7f3b4b76d32c7a17641850ac878e5892646101c74637`  
		Last Modified: Wed, 03 May 2023 04:12:03 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb1f897f694cd71cfdb39db6848cc12a7ad2b84b00121172ad3ee65803f37e0`  
		Last Modified: Wed, 03 May 2023 04:12:04 GMT  
		Size: 16.5 MB (16460475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75409cbb707e9325e124c5b4a02e0b7925f5a9b951dfefd41a994cf2fb4fd4e`  
		Last Modified: Wed, 03 May 2023 04:12:02 GMT  
		Size: 5.3 KB (5284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43502892358bae9619cd9e024635908b15c656fcc476911212610f3a7f55473b`  
		Last Modified: Wed, 03 May 2023 04:12:31 GMT  
		Size: 273.3 MB (273294168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056fa2eee2ceb92367f5d78700b63643e08b8b2584d5650d14d6c9ce4598349f`  
		Last Modified: Wed, 03 May 2023 04:12:02 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77aff48366b110a598e1262cc36cc237ad5c6c03725e53973ab998b303b7cc8d`  
		Last Modified: Wed, 03 May 2023 04:12:00 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e7789a1859fae5a44a7df04b33580a353ca5b4371a7230e0fde64010358383`  
		Last Modified: Wed, 03 May 2023 04:12:00 GMT  
		Size: 4.5 KB (4506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01160071b90f5b299393a96872f21d84f6017bb3c19ece14e56ffcea7b37ce6`  
		Last Modified: Wed, 03 May 2023 04:12:00 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f342da3964c7c16b1181cb8eb8a5f770ede187ab7755e9275beadf3841c6de8d`  
		Last Modified: Wed, 03 May 2023 04:12:00 GMT  
		Size: 189.4 KB (189391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48487d0402f9e1afeaabfb4baec81b52dc32b3bc30b549efb420a586a0814eb0`  
		Last Modified: Wed, 03 May 2023 04:12:00 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.17.10` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:515811607f7198f49063f0ee3e04d98a8c16d22f5b85b95c049d00531d94184c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.9 MB (343937998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c884f81df8b2441dcbbb15ce1a9c2e34c69dc63a9f5f80724d7d01406a977118`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Sat, 22 Apr 2023 11:40:23 GMT
EXPOSE map[5601/tcp:{}]
# Sat, 22 Apr 2023 11:40:23 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Sat, 22 Apr 2023 11:40:25 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Sat, 22 Apr 2023 11:40:25 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Sat, 22 Apr 2023 11:40:28 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Sat, 22 Apr 2023 11:40:28 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Sat, 22 Apr 2023 11:40:29 GMT
RUN fc-cache -v # buildkit
# Sat, 22 Apr 2023 11:41:34 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Sat, 22 Apr 2023 11:41:34 GMT
WORKDIR /usr/share/kibana
# Sat, 22 Apr 2023 11:41:34 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Sat, 22 Apr 2023 11:41:34 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 22 Apr 2023 11:41:34 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Apr 2023 11:41:34 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Sat, 22 Apr 2023 11:41:34 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Sat, 22 Apr 2023 11:41:35 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Sat, 22 Apr 2023 11:41:36 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Sat, 22 Apr 2023 11:41:36 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Sat, 22 Apr 2023 11:41:36 GMT
LABEL org.label-schema.build-date=2023-04-22T11:11:10.120Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=6f79ab09449019d2b5e02ad4508375b5ee56e421 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.10 org.opencontainers.image.created=2023-04-22T11:11:10.120Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=6f79ab09449019d2b5e02ad4508375b5ee56e421 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.10
# Sat, 22 Apr 2023 11:41:36 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Sat, 22 Apr 2023 11:41:36 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Sat, 22 Apr 2023 11:41:36 GMT
USER kibana
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b2202b651830e6b3c80f8c519bee227e262383eac232224c0f6f9f0a172cbe`  
		Last Modified: Wed, 03 May 2023 03:44:04 GMT  
		Size: 10.4 MB (10378704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca2486445eb8eacad7b3030df1791f6f64cdedef9b84a22f0d7692280363542`  
		Last Modified: Wed, 03 May 2023 03:44:02 GMT  
		Size: 9.1 KB (9101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015f64f76e5e2c1c0f7ca949256bbcca08626c13cb610e918f2c7d06c164f49`  
		Last Modified: Wed, 03 May 2023 03:44:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141b572f3bd6ec9736344d2a10a07fa01813c3f652c8acf2da36508b245d0`  
		Last Modified: Wed, 03 May 2023 03:44:01 GMT  
		Size: 16.5 MB (16460473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923eb1d771be4935face03f3f298493bbdcc44ce9c1a947cc59f5045a6484c2f`  
		Last Modified: Wed, 03 May 2023 03:44:00 GMT  
		Size: 5.3 KB (5303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ea610644b13eadd3c7864b5bafd15bfa44507d6729e114cb691d180d94494a`  
		Last Modified: Wed, 03 May 2023 03:44:26 GMT  
		Size: 289.7 MB (289697147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ac5d3b6020f7928184716e438428613a47df04e9be5870c30ae3179a06f27e`  
		Last Modified: Wed, 03 May 2023 03:44:00 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdddb39f097a3a160b7d56566c51a50df14bdf5fccfecaa403aef0aeb89beed`  
		Last Modified: Wed, 03 May 2023 03:43:58 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46deff03e45dcd5db483f25dd00455dd282da1bf62ef0d27f990641fd9fa63ee`  
		Last Modified: Wed, 03 May 2023 03:43:58 GMT  
		Size: 4.5 KB (4504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06745e1ee28617ea061bc3fb96c61bbaa7070c6a4dc9e9ae48c6e8daeeb8d8bd`  
		Last Modified: Wed, 03 May 2023 03:43:58 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ace21ef4debac28277b28495082277a82647051f93c422aeb2c298e89ad9e99`  
		Last Modified: Wed, 03 May 2023 03:43:58 GMT  
		Size: 183.4 KB (183397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa02512736c19144ffc9d045af237f320b63084a70672cc817150ef7a72c0175`  
		Last Modified: Wed, 03 May 2023 03:43:58 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.8.1`

```console
$ docker pull kibana@sha256:0ce1b8559ae3ecfe36b0114420b27549d539067745285667cc3f794347707c0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.8.1` - linux; amd64

```console
$ docker pull kibana@sha256:9b67a861fe5ea19e4b1bf32a983d8db1306efc269dbc3189fc17718509a1f335
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339625198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e5d657f95c72c273baa1cb520c94aaea62e67401d146778854f1cf8f862c37`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 22:39:06 GMT
EXPOSE map[5601/tcp:{}]
# Mon, 05 Jun 2023 22:39:06 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Mon, 05 Jun 2023 22:39:07 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Mon, 05 Jun 2023 22:39:07 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Mon, 05 Jun 2023 22:39:08 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Mon, 05 Jun 2023 22:39:08 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Mon, 05 Jun 2023 22:39:09 GMT
RUN fc-cache -v # buildkit
# Mon, 05 Jun 2023 22:40:27 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Mon, 05 Jun 2023 22:40:27 GMT
WORKDIR /usr/share/kibana
# Mon, 05 Jun 2023 22:40:27 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Mon, 05 Jun 2023 22:40:27 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 05 Jun 2023 22:40:27 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Jun 2023 22:40:27 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Mon, 05 Jun 2023 22:40:27 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Mon, 05 Jun 2023 22:40:28 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Mon, 05 Jun 2023 22:40:29 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Mon, 05 Jun 2023 22:40:29 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Mon, 05 Jun 2023 22:40:29 GMT
LABEL org.label-schema.build-date=2023-06-05T22:09:45.605Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=0fda51d5cd9f9b724fd0ed4356221d49f2c7af27 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.8.1 org.opencontainers.image.created=2023-06-05T22:09:45.605Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=0fda51d5cd9f9b724fd0ed4356221d49f2c7af27 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.8.1
# Mon, 05 Jun 2023 22:40:29 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 05 Jun 2023 22:40:29 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Mon, 05 Jun 2023 22:40:29 GMT
USER kibana
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a0db728ef60566b2603cdf7323dde4d3d275e2ad460f391ca7b0a58ab62385`  
		Last Modified: Wed, 21 Jun 2023 19:25:19 GMT  
		Size: 13.3 MB (13257564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfeb68e9360f01dd693c58c5dd26bb0aff8a409b05fb367bd62ead97a0ba2af6`  
		Last Modified: Wed, 21 Jun 2023 19:25:17 GMT  
		Size: 9.5 KB (9526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf974eebcd85aac83b14a9c17d265437f45a0af9c16f86fcb4a00fca3dbf16`  
		Last Modified: Wed, 21 Jun 2023 19:25:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ad54acd29734f3fd1ceaa955032c2abe72e7cd460c6d6c5520b6fa06ee7f3d`  
		Last Modified: Wed, 21 Jun 2023 19:25:16 GMT  
		Size: 16.5 MB (16460487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5270e9e6385393c91c1f477660ab4269d49ad5680f27cca07bd765fe26f8ee`  
		Last Modified: Wed, 21 Jun 2023 19:25:15 GMT  
		Size: 5.3 KB (5301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078f32ea22c22f5b440ff0facc929931fda97ec82f2ae046e1cd8050af206860`  
		Last Modified: Wed, 21 Jun 2023 19:25:48 GMT  
		Size: 281.1 MB (281116853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c55548b17baf4de2c7f876bbf8512e7c2f0ceb92aefc2990e666e9432f10ae`  
		Last Modified: Wed, 21 Jun 2023 19:25:15 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6834042aa7a073c351d9a3a151af9c670b6bbe4aad95edb4cc4d1203d0a1c5d`  
		Last Modified: Wed, 21 Jun 2023 19:25:13 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f470f83018dbecddcee74d7c9d65fa2c2ee3904fba1211ad9c00cce632116a9`  
		Last Modified: Wed, 21 Jun 2023 19:25:13 GMT  
		Size: 4.5 KB (4525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8797e3ca61eb3fbf2df12d3dac4c1551e4eba7b22e3301e3f761a9f6bfa9c51a`  
		Last Modified: Wed, 21 Jun 2023 19:25:12 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc10d670e7930a052e63cd4cd3d339aa0b80a7d04f5bae0decc70cb0fa66aa2`  
		Last Modified: Wed, 21 Jun 2023 19:25:13 GMT  
		Size: 189.4 KB (189403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8e39d379f1362de3d56327f641407a4e09e1b60e7c5802ad79fa0d0786ca1b`  
		Last Modified: Wed, 21 Jun 2023 19:25:13 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.8.1` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:13278ec8386fe4ad141f366722e69ac0f662d8debfedddf7deccb80f2ce69d93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.8 MB (350801911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5852d1e164a4de4226b3778070efa9871f7c2653ca3067169455a94748c62e5b`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 22:42:40 GMT
EXPOSE map[5601/tcp:{}]
# Mon, 05 Jun 2023 22:42:40 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Mon, 05 Jun 2023 22:42:42 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Mon, 05 Jun 2023 22:42:43 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Mon, 05 Jun 2023 22:42:45 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Mon, 05 Jun 2023 22:42:46 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Mon, 05 Jun 2023 22:42:46 GMT
RUN fc-cache -v # buildkit
# Mon, 05 Jun 2023 22:44:03 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Mon, 05 Jun 2023 22:44:03 GMT
WORKDIR /usr/share/kibana
# Mon, 05 Jun 2023 22:44:03 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Mon, 05 Jun 2023 22:44:03 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 05 Jun 2023 22:44:03 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Jun 2023 22:44:03 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Mon, 05 Jun 2023 22:44:03 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Mon, 05 Jun 2023 22:44:04 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Mon, 05 Jun 2023 22:44:05 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Mon, 05 Jun 2023 22:44:06 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Mon, 05 Jun 2023 22:44:06 GMT
LABEL org.label-schema.build-date=2023-06-05T22:09:45.605Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=0fda51d5cd9f9b724fd0ed4356221d49f2c7af27 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.8.1 org.opencontainers.image.created=2023-06-05T22:09:45.605Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=0fda51d5cd9f9b724fd0ed4356221d49f2c7af27 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.8.1
# Mon, 05 Jun 2023 22:44:06 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 05 Jun 2023 22:44:06 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Mon, 05 Jun 2023 22:44:06 GMT
USER kibana
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5653e0403b36e78350b2036be6bd0cb0f903ed8cb60ed2e87a2e6c0b0cea78a`  
		Last Modified: Wed, 21 Jun 2023 20:37:56 GMT  
		Size: 13.1 MB (13071929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c772a7a24f7425798ec27a5fdddd904f5bd5b349ccb3e6a2848604cb361b20f8`  
		Last Modified: Wed, 21 Jun 2023 20:37:53 GMT  
		Size: 9.1 KB (9093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4228e717b50bd9dcc8d8b76e731a07569b7b63c34e5a3632dcf6ef757fb041cd`  
		Last Modified: Wed, 21 Jun 2023 20:37:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481526e59a38a12865ec628228fd1c7cb770eb385a6d6f7b6fa8c74a825d7083`  
		Last Modified: Wed, 21 Jun 2023 20:37:52 GMT  
		Size: 16.5 MB (16460486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6a25cb1631ae48b6142b5accfbdc78d8484c6c5ee20c335ff7bab50b266fe0`  
		Last Modified: Wed, 21 Jun 2023 20:37:51 GMT  
		Size: 5.3 KB (5288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c46921093700c800ad14919088b56fd225114d60213344187cf268e635be78`  
		Last Modified: Wed, 21 Jun 2023 20:38:19 GMT  
		Size: 293.9 MB (293867804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610267522d91bf7396031214a26efdbc26688c61bb95282285c27f42182ef2b1`  
		Last Modified: Wed, 21 Jun 2023 20:37:51 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fb2da72cfcbe5a97d51f364403037a69298d55260e758f835889edff8b0dd6`  
		Last Modified: Wed, 21 Jun 2023 20:37:48 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b845de755af558b30ade172b15784a2cbbe808145ae2109884ab7e716c24a9e7`  
		Last Modified: Wed, 21 Jun 2023 20:37:48 GMT  
		Size: 4.5 KB (4524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2431ad9b7ee0cbe1e17baf21196b5f3ddd1af60fd6d30236c4391612bae1b990`  
		Last Modified: Wed, 21 Jun 2023 20:37:48 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5648bec2c94efd82eb2284e84c96c416ad78bbb5156b72e150c2e55c0459f02`  
		Last Modified: Wed, 21 Jun 2023 20:37:48 GMT  
		Size: 183.4 KB (183408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f88b22ecc5698deb3de5bc23410e70f2571edf81faf4e7d4e88c3071f36c01`  
		Last Modified: Wed, 21 Jun 2023 20:37:55 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
