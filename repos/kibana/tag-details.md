<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.10`](#kibana71710)
-	[`kibana:8.7.1`](#kibana871)

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

## `kibana:8.7.1`

```console
$ docker pull kibana@sha256:09caa0fa6eedcad5b9cf8ecb73b4e33765b5886f12b144fb2c1ed01744d8a8ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.7.1` - linux; amd64

```console
$ docker pull kibana@sha256:8e649e606847f1ff75752cc68c2b19752292e2e5d5b24d34b76b712d81e31e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296217459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d61b43fc8156bbc4b5b070b451fa1966d39f396ecec673a44bb7800cacb6d23`
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
# Thu, 27 Apr 2023 11:33:35 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 27 Apr 2023 11:33:35 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 27 Apr 2023 11:33:36 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 27 Apr 2023 11:33:37 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 27 Apr 2023 11:33:38 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 27 Apr 2023 11:33:38 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 27 Apr 2023 11:33:38 GMT
RUN fc-cache -v # buildkit
# Thu, 27 Apr 2023 11:34:47 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 27 Apr 2023 11:34:47 GMT
WORKDIR /usr/share/kibana
# Thu, 27 Apr 2023 11:34:47 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 27 Apr 2023 11:34:47 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 27 Apr 2023 11:34:47 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Apr 2023 11:34:47 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 27 Apr 2023 11:34:47 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 11:34:48 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 27 Apr 2023 11:34:49 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 27 Apr 2023 11:34:49 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 27 Apr 2023 11:34:49 GMT
LABEL org.label-schema.build-date=2023-04-27T11:07:16.365Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=40546954e91188153267c4bc92c65c93e45c71ea org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.7.1 org.opencontainers.image.created=2023-04-27T11:07:16.365Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=40546954e91188153267c4bc92c65c93e45c71ea org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.7.1
# Thu, 27 Apr 2023 11:34:49 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 27 Apr 2023 11:34:49 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 27 Apr 2023 11:34:49 GMT
USER kibana
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aff1639b7a72e5feaaaf9fb1265772d7d1465102e95dd58852a177d799db324`  
		Last Modified: Tue, 02 May 2023 15:18:07 GMT  
		Size: 10.5 MB (10511271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672c963ef7cfdf8fb91bd13abca6cdaa2f75b4ed988e50e437e6666a9bf74760`  
		Last Modified: Tue, 02 May 2023 15:18:00 GMT  
		Size: 9.5 KB (9526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1276989a07714e2e983118e5f3ca16ff5a76356eaa96bfb436fc71650c69d6e1`  
		Last Modified: Tue, 02 May 2023 15:18:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985bada154385fa2a619a500fb9e3fae46ebcad3b7dd9efe4085b6d0dd12d872`  
		Last Modified: Tue, 02 May 2023 15:18:05 GMT  
		Size: 16.5 MB (16460477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006cc22cd9fb593210607304f5a440c390830302ee1ed8d894b3d9a6434002d1`  
		Last Modified: Tue, 02 May 2023 15:17:56 GMT  
		Size: 5.3 KB (5286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb86aa94037ffe502de80d3815660aa4391191937115fdc2096b993aceceda9`  
		Last Modified: Tue, 02 May 2023 15:19:05 GMT  
		Size: 240.5 MB (240455502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae32a243c611a664495146ea967f806ac0df318704ead7b43e00a78d1d91e9c`  
		Last Modified: Tue, 02 May 2023 15:17:53 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7026bef5b6090938648e80c86dbaca9507ecb7f6fe91db9a18355c1cfd4a2d9`  
		Last Modified: Tue, 02 May 2023 15:17:52 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c204171b59761caa9cde6376bf07b1b048b3f46eb6ed79402b0d3fd5945e3b`  
		Last Modified: Tue, 02 May 2023 15:17:52 GMT  
		Size: 4.5 KB (4481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1de35d349fcc80ece21a00dabff778f8be3891ee9a544d2c399103d41ef5df`  
		Last Modified: Tue, 02 May 2023 15:17:52 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835cb779f80bad74eaad901f0c5cfee34b9d302606e0fabe4c2c0979e77c2f78`  
		Last Modified: Tue, 02 May 2023 15:17:53 GMT  
		Size: 189.4 KB (189394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82020b9f75941e5630867ba784581e6e343c5f48c80022c6d443e76ec2bebaca`  
		Last Modified: Tue, 02 May 2023 15:17:49 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.7.1` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:a2bd1e9ab3bc1bcb9fe989233a2211eb139eab347221721c14393b984425244a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.1 MB (311110843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6fb473d4163e4232346354d23247fbd210495fca45aae11144b23e827307e8e`
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
# Thu, 27 Apr 2023 11:36:44 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 27 Apr 2023 11:36:44 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 27 Apr 2023 11:36:46 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 27 Apr 2023 11:36:47 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 27 Apr 2023 11:36:50 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 27 Apr 2023 11:36:50 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 27 Apr 2023 11:36:51 GMT
RUN fc-cache -v # buildkit
# Thu, 27 Apr 2023 11:38:13 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 27 Apr 2023 11:38:13 GMT
WORKDIR /usr/share/kibana
# Thu, 27 Apr 2023 11:38:14 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 27 Apr 2023 11:38:14 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 27 Apr 2023 11:38:14 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Apr 2023 11:38:14 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 27 Apr 2023 11:38:14 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 11:38:15 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 27 Apr 2023 11:38:15 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 27 Apr 2023 11:38:16 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 27 Apr 2023 11:38:16 GMT
LABEL org.label-schema.build-date=2023-04-27T11:07:16.365Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=40546954e91188153267c4bc92c65c93e45c71ea org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.7.1 org.opencontainers.image.created=2023-04-27T11:07:16.365Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=40546954e91188153267c4bc92c65c93e45c71ea org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.7.1
# Thu, 27 Apr 2023 11:38:16 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 27 Apr 2023 11:38:16 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 27 Apr 2023 11:38:16 GMT
USER kibana
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d650c718f705af886ae928e331eb1c68e4946955490ee23faecfde40d809e6d3`  
		Last Modified: Wed, 03 May 2023 03:43:32 GMT  
		Size: 10.4 MB (10378631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f69d70ecf3026e5848f4c1690371604de391a7ae377651b8c68fb6eb69048d0`  
		Last Modified: Wed, 03 May 2023 03:43:29 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4071b3ae5acbb079fd35573167790514f70a846811cc6e9b5a76275016545d17`  
		Last Modified: Wed, 03 May 2023 03:43:29 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a0f561f47d4ba4d5014a31fe2c6c8a53cb38b0dae69bc0a40e43b72916c6f2`  
		Last Modified: Wed, 03 May 2023 03:43:28 GMT  
		Size: 16.5 MB (16460485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d8447ec27c64b0d781196bff8c2ecfcd2098d9245cd9b59b2f0b22404d5d1b`  
		Last Modified: Wed, 03 May 2023 03:43:27 GMT  
		Size: 5.3 KB (5300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfb2d51864a059cc6195c14e9fbed00df973d9f34b48822f45b3d92228080f4`  
		Last Modified: Wed, 03 May 2023 03:43:51 GMT  
		Size: 256.9 MB (256870077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3859eb302157742d54e8cdd6b9ce937e01bbac470477585ef0e216f49ebe3f`  
		Last Modified: Wed, 03 May 2023 03:43:27 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e990e662341ec2d91dd9ac7dba47f02a2b5fc16f417a684ea3d5308cbcad9f6`  
		Last Modified: Wed, 03 May 2023 03:43:24 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020df82bc015800e10899e3dbfb2368ddca07960aaf2e988c096c9e472720a5f`  
		Last Modified: Wed, 03 May 2023 03:43:25 GMT  
		Size: 4.5 KB (4483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb013ba85b1455514886b04fc3dcd30517e9885a010bc0789b66c63dc954e8`  
		Last Modified: Wed, 03 May 2023 03:43:24 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c9180f85107e3148562db0b0ab2ecb2e56fed4ccdfc4ffd488017127aacd0a`  
		Last Modified: Wed, 03 May 2023 03:43:25 GMT  
		Size: 183.4 KB (183397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac18094d0533cf3884a5601fcbaffcafa96616d6fd61b39fc280adb27781e719`  
		Last Modified: Wed, 03 May 2023 03:43:29 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
