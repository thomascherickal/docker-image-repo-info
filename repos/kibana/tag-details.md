<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.8`](#kibana7178)
-	[`kibana:8.6.1`](#kibana861)

## `kibana:7.17.8`

```console
$ docker pull kibana@sha256:c5781ba340ef89d630f9f05a904579d9cf614c4188920b8e4f293ce87000eebe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.17.8` - linux; amd64

```console
$ docker pull kibana@sha256:0732aac8c9f619102bfb38abf2de7eb9c3fe9ba0f13db71a8478df92415c5856
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.9 MB (329947475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e0bd482ac7a01ef8249fa76f64832af2b9dc12525f030ce9df4fde0806de90`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Fri, 02 Dec 2022 12:36:45 GMT
EXPOSE map[5601/tcp:{}]
# Fri, 02 Dec 2022 12:36:45 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Fri, 02 Dec 2022 12:36:47 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Fri, 02 Dec 2022 12:36:47 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Fri, 02 Dec 2022 12:36:48 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Fri, 02 Dec 2022 12:36:48 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Fri, 02 Dec 2022 12:36:49 GMT
RUN fc-cache -v # buildkit
# Fri, 02 Dec 2022 12:37:48 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Fri, 02 Dec 2022 12:37:48 GMT
WORKDIR /usr/share/kibana
# Fri, 02 Dec 2022 12:37:48 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Fri, 02 Dec 2022 12:37:48 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 02 Dec 2022 12:37:48 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Dec 2022 12:37:48 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Fri, 02 Dec 2022 12:37:48 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Fri, 02 Dec 2022 12:37:49 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Fri, 02 Dec 2022 12:37:50 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Fri, 02 Dec 2022 12:37:50 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Fri, 02 Dec 2022 12:37:50 GMT
LABEL org.label-schema.build-date=2022-12-02T12:10:17.323Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=6932e2bff5c5d630510e463852e16423ff8db3fb org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.8 org.opencontainers.image.created=2022-12-02T12:10:17.323Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=6932e2bff5c5d630510e463852e16423ff8db3fb org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.8
# Fri, 02 Dec 2022 12:37:50 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Fri, 02 Dec 2022 12:37:50 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Fri, 02 Dec 2022 12:37:50 GMT
USER kibana
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04b48ebd73430801c941d160ca56aa6c4efbbb013a35b346e08133d50ba341c`  
		Last Modified: Thu, 08 Dec 2022 19:24:30 GMT  
		Size: 11.7 MB (11714842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defe962e211750322d6496dca4e37450f4dc3897683b774614eb927b29b73b6f`  
		Last Modified: Thu, 08 Dec 2022 19:24:28 GMT  
		Size: 9.5 KB (9530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f0651d1c1e372d4706330ac8723e1fa4eaa0c6876adc5438d9d2ab806ff74d`  
		Last Modified: Thu, 08 Dec 2022 19:24:27 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6263e00ebb0160570401c83c36bd4ead554c0a6ed8336339e28d8f1e3207740c`  
		Last Modified: Thu, 08 Dec 2022 19:24:27 GMT  
		Size: 16.5 MB (16460488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954d70cf9c1cc22e9792ee52012e642b78231b1fcfa82716888a415f0c24d7b5`  
		Last Modified: Thu, 08 Dec 2022 19:24:26 GMT  
		Size: 5.3 KB (5287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c87fe21ee7582a0a851ebb66fdb4802178000c1e5eca4f18de0d224c420f63`  
		Last Modified: Thu, 08 Dec 2022 19:24:58 GMT  
		Size: 273.0 MB (272982631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28cfeb29d506090ae27508637a9db02dc53b1cfe6d9c293771a912bed42471f`  
		Last Modified: Thu, 08 Dec 2022 19:24:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecaf7a5da8fdcf83439f99f3c0cc94fb9a06be2b40572adfe818cb7b605d276`  
		Last Modified: Thu, 08 Dec 2022 19:24:23 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bee9f5efc3be5a5754aacfbcf951bafef9d133002eb4e9a322e8abc6454ccd5`  
		Last Modified: Thu, 08 Dec 2022 19:24:23 GMT  
		Size: 4.5 KB (4504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9691dcae52725cf4a966887b4769dc1f45be1727162c822530eae6029e1f091a`  
		Last Modified: Thu, 08 Dec 2022 19:24:23 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aced9fc65582598057ae1bd23d915aed0662b5ea7dade802351c94085f5a7528`  
		Last Modified: Thu, 08 Dec 2022 19:24:23 GMT  
		Size: 189.4 KB (189393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c7dcac3cb19995076be632f659a17314af4183972dd66e1070f7c3ea050377`  
		Last Modified: Thu, 08 Dec 2022 19:24:26 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.17.8` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:bb5babf893769e924dbe713903ae128f3c19a6a9b742234d0fb0c30292588300
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344853258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d0b7c25750636dbb7316253e0b280add79abc4c00bb088ffee55460259d370`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Fri, 02 Dec 2022 12:39:52 GMT
EXPOSE map[5601/tcp:{}]
# Fri, 02 Dec 2022 12:39:52 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Fri, 02 Dec 2022 12:39:54 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Fri, 02 Dec 2022 12:39:54 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Fri, 02 Dec 2022 12:39:57 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Fri, 02 Dec 2022 12:39:57 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Fri, 02 Dec 2022 12:39:58 GMT
RUN fc-cache -v # buildkit
# Fri, 02 Dec 2022 12:40:56 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Fri, 02 Dec 2022 12:40:56 GMT
WORKDIR /usr/share/kibana
# Fri, 02 Dec 2022 12:40:56 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Fri, 02 Dec 2022 12:40:56 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 02 Dec 2022 12:40:56 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Dec 2022 12:40:56 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Fri, 02 Dec 2022 12:40:56 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Fri, 02 Dec 2022 12:40:57 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Fri, 02 Dec 2022 12:40:58 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Fri, 02 Dec 2022 12:40:59 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Fri, 02 Dec 2022 12:40:59 GMT
LABEL org.label-schema.build-date=2022-12-02T12:10:17.323Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=6932e2bff5c5d630510e463852e16423ff8db3fb org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.8 org.opencontainers.image.created=2022-12-02T12:10:17.323Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=6932e2bff5c5d630510e463852e16423ff8db3fb org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.8
# Fri, 02 Dec 2022 12:40:59 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Fri, 02 Dec 2022 12:40:59 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Fri, 02 Dec 2022 12:40:59 GMT
USER kibana
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a7bcc73093cd2bfbe3f38c93710b78ba17a7f74f69a0ec9273e570d813b340`  
		Last Modified: Thu, 08 Dec 2022 18:43:30 GMT  
		Size: 11.6 MB (11562259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274f7f47ce5a2e9347133465afb0f49bbfee9b5b8b5cba988ba6b0e8a769f995`  
		Last Modified: Thu, 08 Dec 2022 18:43:27 GMT  
		Size: 9.1 KB (9100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4277c11787d8984dd6330fcb268ce5e9954d66379b35b967f6c84526aa8a99d6`  
		Last Modified: Thu, 08 Dec 2022 18:43:26 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f984ea1d55ef1e447e4d751e7c1326142f16e731f25f1785d1d7b262c4f663`  
		Last Modified: Thu, 08 Dec 2022 18:43:26 GMT  
		Size: 16.5 MB (16460475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e49f27af693d93f12853b9ab41a56f591c97ff59d10f3b29ba0ecd841cfc540`  
		Last Modified: Thu, 08 Dec 2022 18:43:24 GMT  
		Size: 5.3 KB (5294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d7112d02d9fce86db5a9018a5222bf35b557c944aa97c83ef84433bcb94d88`  
		Last Modified: Thu, 08 Dec 2022 18:43:52 GMT  
		Size: 289.4 MB (289429253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b6a5cf98a8a0bfcceeca20266c7bf448ea10c3211a9fe486bc98088beb40fc`  
		Last Modified: Thu, 08 Dec 2022 18:43:24 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a267bd5a81889e6e47acb556ac3cd423ab48375f30e6da340ae869b98d19ad25`  
		Last Modified: Thu, 08 Dec 2022 18:43:22 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26de877b72d79ad980ceab8446c972a59eb0e308a9349e03faa1a57aea196d7`  
		Last Modified: Thu, 08 Dec 2022 18:43:22 GMT  
		Size: 4.5 KB (4506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b7e9f22349c3402de8d54e621ea853753c4e3ce21b95f3ec2a251129cb607`  
		Last Modified: Thu, 08 Dec 2022 18:43:22 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0025d6ac508f7857ab776230634817d719502b3e9a5e87373a9abe989642a5`  
		Last Modified: Thu, 08 Dec 2022 18:43:22 GMT  
		Size: 183.4 KB (183393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485fb4d88cc96f4910230c8c885d283ebeceb0c5906c23a8bc4806b5d9269b33`  
		Last Modified: Thu, 08 Dec 2022 18:43:28 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.6.1`

```console
$ docker pull kibana@sha256:a75691a747f3d1edee40bb638dec4374908a4a3df6bb25291cac17f29365ccf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.6.1` - linux; amd64

```console
$ docker pull kibana@sha256:225565bbc6d6ba90be5a173c458e68b3c355a2772190838b8d61a85c4a262c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.0 MB (284961948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ee129133d3e0a6faa26c71dd8ca0691bad7bb7ec924efa16957422387e5a47f`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 24 Jan 2023 21:14:53 GMT
EXPOSE map[5601/tcp:{}]
# Tue, 24 Jan 2023 21:14:53 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Tue, 24 Jan 2023 21:14:55 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Tue, 24 Jan 2023 21:14:55 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Tue, 24 Jan 2023 21:14:56 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Tue, 24 Jan 2023 21:14:56 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Tue, 24 Jan 2023 21:14:56 GMT
RUN fc-cache -v # buildkit
# Tue, 24 Jan 2023 21:15:59 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Tue, 24 Jan 2023 21:15:59 GMT
WORKDIR /usr/share/kibana
# Tue, 24 Jan 2023 21:15:59 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Tue, 24 Jan 2023 21:15:59 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 24 Jan 2023 21:15:59 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:15:59 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Tue, 24 Jan 2023 21:15:59 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Tue, 24 Jan 2023 21:16:00 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Tue, 24 Jan 2023 21:16:00 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Tue, 24 Jan 2023 21:16:01 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Tue, 24 Jan 2023 21:16:01 GMT
LABEL org.label-schema.build-date=2023-01-24T20:50:57.502Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=4c2492450a50cd000fcd85edf668b75828686196 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.6.1 org.opencontainers.image.created=2023-01-24T20:50:57.502Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=4c2492450a50cd000fcd85edf668b75828686196 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.6.1
# Tue, 24 Jan 2023 21:16:01 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Tue, 24 Jan 2023 21:16:01 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Tue, 24 Jan 2023 21:16:01 GMT
USER kibana
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c022b40f2b248b0b1493d7dbb76f13252b0ef7535bc48940f52d548e8637d667`  
		Last Modified: Tue, 31 Jan 2023 18:10:39 GMT  
		Size: 10.5 MB (10506861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2190c2b6627af7802df3c5f1013c0115bcdcd3c0aea4afcf279e9f1ae0386f80`  
		Last Modified: Tue, 31 Jan 2023 18:08:52 GMT  
		Size: 9.5 KB (9530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb3547febaaa4ca4c017e431016f2446f6f6c6d4906216d094eabb6fb2374dd`  
		Last Modified: Tue, 31 Jan 2023 18:08:48 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41625281f857393b6cfe3758cd1d65d6d9ebbe5190b1a33357fb8fd25abc90bb`  
		Last Modified: Tue, 31 Jan 2023 18:10:06 GMT  
		Size: 16.5 MB (16460488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f239ba1c94c476a942ec235938a1d69474fadd38809f16a0b4778cdd84e3f884`  
		Last Modified: Tue, 31 Jan 2023 18:08:49 GMT  
		Size: 5.3 KB (5298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e2838ca19f9c46a825e42f5ec49388211a61716f2ef6f4fa40933b385411ec`  
		Last Modified: Tue, 31 Jan 2023 18:27:06 GMT  
		Size: 229.2 MB (229206055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58417207101b0b03d9b8569c7d5207f9c73616be4ab6e45dedfd06cc77a51898`  
		Last Modified: Tue, 31 Jan 2023 18:08:43 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca139084444340f6a2ddfc3a1dc1f84e4c34e5a5caa0b5abf5e89fcca9ed5ec9`  
		Last Modified: Tue, 31 Jan 2023 18:08:43 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88477b90f1f7984ac4704cfd0121dbee09f6ed71fb7ec81af0f9a835f7a7737`  
		Last Modified: Tue, 31 Jan 2023 18:08:42 GMT  
		Size: 4.5 KB (4475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7259a8c2aa2e05204b3e1142e522d6646f720bfe4fe121b3814144aae582e035`  
		Last Modified: Tue, 31 Jan 2023 18:08:39 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d806c80d99dd2858e29fbf777995549138a379f05f1369d1139f1bb76ab64f`  
		Last Modified: Tue, 31 Jan 2023 18:08:40 GMT  
		Size: 189.4 KB (189391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03ffd0b8fed29c391b52433d3c3336c13562bfd84b573accfaa1f60d9a2664`  
		Last Modified: Tue, 31 Jan 2023 18:08:39 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.6.1` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:d880bca9e4abf5e6a9c0cab9d625854ea84495ffad589b9a2177fb232e9107d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.9 MB (299866118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:698b682cc5614791b642e50794b96a1cb476a3b5a2429a8f45f3ae6b25cad622`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Tue, 24 Jan 2023 21:17:53 GMT
EXPOSE map[5601/tcp:{}]
# Tue, 24 Jan 2023 21:17:53 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Tue, 24 Jan 2023 21:17:55 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Tue, 24 Jan 2023 21:17:56 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Tue, 24 Jan 2023 21:17:59 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Tue, 24 Jan 2023 21:17:59 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Tue, 24 Jan 2023 21:18:00 GMT
RUN fc-cache -v # buildkit
# Tue, 24 Jan 2023 21:18:58 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Tue, 24 Jan 2023 21:18:58 GMT
WORKDIR /usr/share/kibana
# Tue, 24 Jan 2023 21:18:58 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Tue, 24 Jan 2023 21:18:58 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 24 Jan 2023 21:18:58 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:18:58 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Tue, 24 Jan 2023 21:18:58 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Tue, 24 Jan 2023 21:18:59 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Tue, 24 Jan 2023 21:19:00 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Tue, 24 Jan 2023 21:19:01 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Tue, 24 Jan 2023 21:19:01 GMT
LABEL org.label-schema.build-date=2023-01-24T20:50:57.502Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=4c2492450a50cd000fcd85edf668b75828686196 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.6.1 org.opencontainers.image.created=2023-01-24T20:50:57.502Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=4c2492450a50cd000fcd85edf668b75828686196 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.6.1
# Tue, 24 Jan 2023 21:19:01 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Tue, 24 Jan 2023 21:19:01 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Tue, 24 Jan 2023 21:19:01 GMT
USER kibana
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf84f9ddf5d70d7c61dd4fb5f24282540cfffb217cfb56ee4a557f0019edbb28`  
		Last Modified: Wed, 01 Feb 2023 22:17:04 GMT  
		Size: 10.4 MB (10376037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b8d9e1d3b51ecd573e86b1292bae5dbd499bb629567552037beacec72f8a82`  
		Last Modified: Wed, 01 Feb 2023 22:17:01 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012bfcd12fc094d9cd08f1647207c3f41750c1ffb7990aae03edab64a88ca460`  
		Last Modified: Wed, 01 Feb 2023 22:17:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b001e14a4475f17556be030773c4c35135e8577f92bdf0690c4163f67e45fb5`  
		Last Modified: Wed, 01 Feb 2023 22:17:01 GMT  
		Size: 16.5 MB (16460490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74696c4bca805020f59e48a96ec5920a79168626c78c35de53f4ff28175ab9ce`  
		Last Modified: Wed, 01 Feb 2023 22:16:59 GMT  
		Size: 5.3 KB (5301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aa5e430296c6895a4662d5a581469eeea69c5c6c24f017d98121e5b3cd30a8`  
		Last Modified: Wed, 01 Feb 2023 22:17:24 GMT  
		Size: 245.6 MB (245631191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b74574e3b2feb22f744814f24e28ac22ebf5a32c21c655a4e4bcb39c0fdbfe`  
		Last Modified: Wed, 01 Feb 2023 22:16:58 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4099d14ec817f1a313ea352368f621203bb4b5bb4761977028560c9507699c5`  
		Last Modified: Wed, 01 Feb 2023 22:16:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cdfd2fb00b50b8dedc144f5f26f1a91c8e819480d3e82c73096af577c2d0a0`  
		Last Modified: Wed, 01 Feb 2023 22:16:56 GMT  
		Size: 4.5 KB (4474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09666dd0d58a8828d6b0db152209a7e033ac087d8817281d9c7d67c960dd9905`  
		Last Modified: Wed, 01 Feb 2023 22:16:56 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095ae2e4b1f3102a1f68e8e2173c977716187de11cf56eff602e725c7b27d52a`  
		Last Modified: Wed, 01 Feb 2023 22:16:56 GMT  
		Size: 183.4 KB (183393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b78320fd7d03992b78ae90254273d4f2aff6c38f37a61dc7a011431a68d14`  
		Last Modified: Wed, 01 Feb 2023 22:17:02 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
