<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.8`](#kibana7178)
-	[`kibana:8.5.3`](#kibana853)

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

## `kibana:8.5.3`

```console
$ docker pull kibana@sha256:bb02932d930f2f23c9ef3047b990095b07b5e8b04c7f1831dd0c99cd199a57ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.5.3` - linux; amd64

```console
$ docker pull kibana@sha256:e4c62bc2c36b0d2d2b8246cd11d0a759ce622dc03fec5fae1a6abe7d4fc86696
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.2 MB (284165490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1215bb66460ce6ba56571c497bd313ffc1e324a16ed748f2902ed5eea7c176ee`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Mon, 05 Dec 2022 12:32:19 GMT
EXPOSE map[5601/tcp:{}]
# Mon, 05 Dec 2022 12:32:19 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Mon, 05 Dec 2022 12:32:20 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Mon, 05 Dec 2022 12:32:20 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Mon, 05 Dec 2022 12:32:21 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Mon, 05 Dec 2022 12:32:21 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Mon, 05 Dec 2022 12:32:22 GMT
RUN fc-cache -v # buildkit
# Mon, 05 Dec 2022 12:33:17 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Mon, 05 Dec 2022 12:33:17 GMT
WORKDIR /usr/share/kibana
# Mon, 05 Dec 2022 12:33:17 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Mon, 05 Dec 2022 12:33:17 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 05 Dec 2022 12:33:17 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Dec 2022 12:33:17 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Mon, 05 Dec 2022 12:33:17 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Mon, 05 Dec 2022 12:33:17 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Mon, 05 Dec 2022 12:33:18 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Mon, 05 Dec 2022 12:33:19 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Mon, 05 Dec 2022 12:33:19 GMT
LABEL org.label-schema.build-date=2022-12-05T12:09:50.062Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=93852c98d9e9902fe166302fae10bc8c5f3502fb org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.5.3 org.opencontainers.image.created=2022-12-05T12:09:50.062Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=93852c98d9e9902fe166302fae10bc8c5f3502fb org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.5.3
# Mon, 05 Dec 2022 12:33:19 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 05 Dec 2022 12:33:19 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Mon, 05 Dec 2022 12:33:19 GMT
USER kibana
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f93648d1f263dbc6736df193bfef73dee89bf44efad917cdbae9723754e9331`  
		Last Modified: Sat, 10 Dec 2022 17:31:06 GMT  
		Size: 11.7 MB (11714726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9641f0c3ca5c8edd6556cbeff2b62c801726d2f27edc4ef93e5e1e99d8ba6d5`  
		Last Modified: Sat, 10 Dec 2022 17:31:03 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e76b7b06ec5d1ab4ff40d0f79185feeb650d8ef3d72a86164b7b08175a34b3`  
		Last Modified: Sat, 10 Dec 2022 17:31:02 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c76daa2f44333d6274ed9510b0a5f311c6bca929132f94a3ea5996022c75b1`  
		Last Modified: Sat, 10 Dec 2022 17:31:02 GMT  
		Size: 16.5 MB (16460491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3f0936ca5e3de0da187d8da00fd13c243868915b738f48547ce665704609d4`  
		Last Modified: Sat, 10 Dec 2022 17:31:01 GMT  
		Size: 5.3 KB (5283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80add0185acb998d18803d77ccf2a12fa47f6024c52e3943ddc8df105d875eba`  
		Last Modified: Sat, 10 Dec 2022 17:31:20 GMT  
		Size: 227.2 MB (227200842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fea072139e146de6a2fe129b6f2bfb26640284519ab685ea12746fdc88e48d0`  
		Last Modified: Sat, 10 Dec 2022 17:31:01 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02de50b0a9a6419b484b3a247cea90249f8b3609d72153f2a2ef0b6b9c218e4b`  
		Last Modified: Sat, 10 Dec 2022 17:30:57 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19dd1fc862b2fc9bae65d30a19385f748f0641b4092b2c9638e5ea500d3dcd4`  
		Last Modified: Sat, 10 Dec 2022 17:30:57 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692365e4b6108fda7a2f3bee1ac7fb6863650521d4afcf3eff825ce57eaf671a`  
		Last Modified: Sat, 10 Dec 2022 17:30:57 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d61275a07495248fa55aa1967588cf682c86feb0edd11a88de4602e709c5b5`  
		Last Modified: Sat, 10 Dec 2022 17:30:58 GMT  
		Size: 189.4 KB (189393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbe03850766b412a13db5a472217dda1ec238a6fe743c7b3bd3c2473bc973e4`  
		Last Modified: Sat, 10 Dec 2022 17:30:58 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.5.3` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:01cc47be65f46448fefcaf96b1a9a3f6f3e1175a0de9002bd599430a69252629
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.0 MB (299028996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:760fe093b49b0473cc4f0d53f4f4721be6640e5c0790291af8d120348ecf7ed8`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Mon, 05 Dec 2022 12:35:13 GMT
EXPOSE map[5601/tcp:{}]
# Mon, 05 Dec 2022 12:35:13 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Mon, 05 Dec 2022 12:35:15 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Mon, 05 Dec 2022 12:35:15 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Mon, 05 Dec 2022 12:35:18 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Mon, 05 Dec 2022 12:35:18 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Mon, 05 Dec 2022 12:35:19 GMT
RUN fc-cache -v # buildkit
# Mon, 05 Dec 2022 12:36:10 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Mon, 05 Dec 2022 12:36:10 GMT
WORKDIR /usr/share/kibana
# Mon, 05 Dec 2022 12:36:11 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Mon, 05 Dec 2022 12:36:11 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 05 Dec 2022 12:36:11 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Dec 2022 12:36:11 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Mon, 05 Dec 2022 12:36:11 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Mon, 05 Dec 2022 12:36:12 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Mon, 05 Dec 2022 12:36:12 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Mon, 05 Dec 2022 12:36:13 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Mon, 05 Dec 2022 12:36:13 GMT
LABEL org.label-schema.build-date=2022-12-05T12:09:50.062Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=93852c98d9e9902fe166302fae10bc8c5f3502fb org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.5.3 org.opencontainers.image.created=2022-12-05T12:09:50.062Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=93852c98d9e9902fe166302fae10bc8c5f3502fb org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.5.3
# Mon, 05 Dec 2022 12:36:13 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Mon, 05 Dec 2022 12:36:13 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Mon, 05 Dec 2022 12:36:13 GMT
USER kibana
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5a5ebe482c22541ff90f3cc14b77d88be561a2bcd658986eed35d865173673`  
		Last Modified: Mon, 12 Dec 2022 19:51:29 GMT  
		Size: 11.6 MB (11562280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c9894ba5d308c91010743c451d4793a7440c00f0babf7a4691fc77b899b0a0`  
		Last Modified: Mon, 12 Dec 2022 19:51:28 GMT  
		Size: 9.1 KB (9101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe3981496bc9acffc6fddeeeeae9beb370217ff04c345f5b6e121321e3d51fb`  
		Last Modified: Mon, 12 Dec 2022 19:51:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c17446c914cc876dbee5b5254ffef49ccc58adb23b29047def9a13da55c6b2`  
		Last Modified: Mon, 12 Dec 2022 19:51:27 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4914f5f154324530a38f1d57dee555c839617cdea8cc396c7a10aaeb295c7e40`  
		Last Modified: Mon, 12 Dec 2022 19:51:26 GMT  
		Size: 5.3 KB (5287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b214eb1f8951b562bfd0b43b60a9676e3c503db2110cbc449ba1c3c23d6da691`  
		Last Modified: Mon, 12 Dec 2022 19:51:51 GMT  
		Size: 243.6 MB (243605052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc5a0fe191c8607c975dfb4af992ed0d0d0f45eb20578e0b4bec42466787dd`  
		Last Modified: Mon, 12 Dec 2022 19:51:26 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00f25185579045d6672a7a353392d5f19b7bf7c39c50ae1efa413fc724e6b30`  
		Last Modified: Mon, 12 Dec 2022 19:51:23 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e0b232301bcc60fef986763957d21f5e338a935db30e3dac5936450e8c8e4b`  
		Last Modified: Mon, 12 Dec 2022 19:51:24 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3604dc607acf28687229bb57c185a2281133cdbdef557ed27d017ea772172e3`  
		Last Modified: Mon, 12 Dec 2022 19:51:24 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59e47c8ed9d02ba98e6ce771881f5e68a94876ad9ca06916182a364833ddd30`  
		Last Modified: Mon, 12 Dec 2022 19:51:24 GMT  
		Size: 183.4 KB (183394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5422643eb1eed06b30b41144e96c73c8a733c3a17150ef3dac3f535e6b3e06d9`  
		Last Modified: Mon, 12 Dec 2022 19:51:24 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
