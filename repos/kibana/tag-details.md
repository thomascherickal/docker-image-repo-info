<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.7`](#kibana7177)
-	[`kibana:8.5.1`](#kibana851)

## `kibana:7.17.7`

```console
$ docker pull kibana@sha256:414b6a159b8ab8049bcf45236d7ec86bc0238ba9ec86fbd362e948c09cc34991
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.17.7` - linux; amd64

```console
$ docker pull kibana@sha256:688e915984126d61b8602c8ab12c0e63b7d6d5d734a6743cd144baf9c92fdc24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.2 MB (325226252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5b6ca1535b5be025db5fc594ec5d1592e82653691bf7a4d7568c80f11dfa8`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Thu, 13 Oct 2022 11:33:52 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 13 Oct 2022 11:33:52 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 13 Oct 2022 11:33:54 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 13 Oct 2022 11:33:54 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 13 Oct 2022 11:33:55 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 13 Oct 2022 11:33:55 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 13 Oct 2022 11:33:56 GMT
RUN fc-cache -v # buildkit
# Thu, 13 Oct 2022 11:34:53 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 13 Oct 2022 11:34:53 GMT
WORKDIR /usr/share/kibana
# Thu, 13 Oct 2022 11:34:53 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 13 Oct 2022 11:34:53 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 13 Oct 2022 11:34:53 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Oct 2022 11:34:53 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 13 Oct 2022 11:34:53 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 13 Oct 2022 11:34:54 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 13 Oct 2022 11:34:55 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 13 Oct 2022 11:34:55 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 13 Oct 2022 11:34:55 GMT
LABEL org.label-schema.build-date=2022-10-13T11:08:08.384Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=d60b53b0f972a3e59c06c2cb1bf5818f92d1cb63 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.7 org.opencontainers.image.created=2022-10-13T11:08:08.384Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=d60b53b0f972a3e59c06c2cb1bf5818f92d1cb63 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.7
# Thu, 13 Oct 2022 11:34:55 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 13 Oct 2022 11:34:55 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 13 Oct 2022 11:34:55 GMT
USER kibana
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff10acfee0ec519331e95c95a78953d67fb530cfde3f6f3bf3fd2246da19ad0`  
		Last Modified: Thu, 27 Oct 2022 00:21:26 GMT  
		Size: 10.9 MB (10859172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389dd4b16fb3c8bbfedf30e8088075a5cca6f1de6852e8ccfa52242f33b58ad6`  
		Last Modified: Thu, 27 Oct 2022 00:21:24 GMT  
		Size: 9.5 KB (9525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a153be433adce4c78f7b2f6b3ad3048ef4304ceeb25271372f4d06e69c9e9b`  
		Last Modified: Thu, 27 Oct 2022 00:21:22 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f70ada2dbae717de01734e027164f46178c2304a58c702dd5488375e1b2c347`  
		Last Modified: Thu, 27 Oct 2022 00:21:23 GMT  
		Size: 16.5 MB (16460493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f886755e1faef990bf587c830745fc38bde61889959e4ff9a57436b97921e858`  
		Last Modified: Thu, 27 Oct 2022 00:21:22 GMT  
		Size: 5.3 KB (5289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c4c41a32c356534571e15346f0bfeaaa565a5482cfbc17ac4f031a639654f1`  
		Last Modified: Thu, 27 Oct 2022 00:21:55 GMT  
		Size: 269.1 MB (269120450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06e31ef44b16d3b808aa158ec91285ba48fc3ce46be97b7ca03d735a290dbc6`  
		Last Modified: Thu, 27 Oct 2022 00:21:21 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5de441a7b60e60d77a2166ee22dcd97bd6a7af69ca118300ca283083ff8ff1`  
		Last Modified: Thu, 27 Oct 2022 00:21:19 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9501cd64e5ec0558ef787e9591111e154ae854a739d8de870da22b00fe1c56e6`  
		Last Modified: Thu, 27 Oct 2022 00:21:19 GMT  
		Size: 4.5 KB (4506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa2ba840eb00f5fc27bb15cb17656aa0ef143f92d5d7af3f9319ad5f4c50609`  
		Last Modified: Thu, 27 Oct 2022 00:21:19 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b573bb90bed58e0e68bb340d1430d88392e3e595c733fbe91be59909b46350`  
		Last Modified: Thu, 27 Oct 2022 00:21:19 GMT  
		Size: 189.4 KB (189391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60bde26a17c014793459708c56c923a6c3a673d6f0c39bea9f7a05ffaef91e`  
		Last Modified: Thu, 27 Oct 2022 00:21:19 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.17.7` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:84781310f0f3dce3a4892160d64497e3d16aff2bd1fcc4c5832d0b19865a9289
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.4 MB (338353583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c229fd67efd81d3f0b2b2e5ecfc60cb22f6a92d52197ebead46d713d2fbaac64`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Thu, 13 Oct 2022 11:36:55 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 13 Oct 2022 11:36:55 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 13 Oct 2022 11:36:57 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 13 Oct 2022 11:36:58 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 13 Oct 2022 11:37:00 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 13 Oct 2022 11:37:01 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 13 Oct 2022 11:37:02 GMT
RUN fc-cache -v # buildkit
# Thu, 13 Oct 2022 11:37:57 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 13 Oct 2022 11:37:57 GMT
WORKDIR /usr/share/kibana
# Thu, 13 Oct 2022 11:37:57 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 13 Oct 2022 11:37:57 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 13 Oct 2022 11:37:57 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Oct 2022 11:37:57 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 13 Oct 2022 11:37:57 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 13 Oct 2022 11:37:58 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 13 Oct 2022 11:37:59 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 13 Oct 2022 11:38:00 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 13 Oct 2022 11:38:00 GMT
LABEL org.label-schema.build-date=2022-10-13T11:08:08.384Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=d60b53b0f972a3e59c06c2cb1bf5818f92d1cb63 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.7 org.opencontainers.image.created=2022-10-13T11:08:08.384Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=d60b53b0f972a3e59c06c2cb1bf5818f92d1cb63 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.7
# Thu, 13 Oct 2022 11:38:00 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 13 Oct 2022 11:38:00 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 13 Oct 2022 11:38:00 GMT
USER kibana
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3529e72c508ff0c278baa082272c33398313d46c0d9ce9fe40a40b4c5a08da00`  
		Last Modified: Wed, 26 Oct 2022 20:29:50 GMT  
		Size: 10.7 MB (10722256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0585400ab4eb919c7b7b17055696358f9e4af11b6cdd0251d119c9c061722023`  
		Last Modified: Wed, 26 Oct 2022 20:29:48 GMT  
		Size: 9.1 KB (9097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b45335f3c1dd3a8f1dfba84038b846f342d7b1ba1a8871c8ca3c9d0ee50489f`  
		Last Modified: Wed, 26 Oct 2022 20:29:47 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379c494583da78edbdc81aaa481b82306ef148a817430fffe6020c10f361dde`  
		Last Modified: Wed, 26 Oct 2022 20:29:49 GMT  
		Size: 16.5 MB (16460495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8468d973542b3c8616b0e8cbbdcbf23e1ee004fe61e1eed3cc65e2769861a6cc`  
		Last Modified: Wed, 26 Oct 2022 20:29:46 GMT  
		Size: 5.3 KB (5287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b77109bc67edcca176d061e28487d7fb4067172185df235fd7071892f70844`  
		Last Modified: Wed, 26 Oct 2022 20:30:11 GMT  
		Size: 283.8 MB (283773951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775d06ca9fb9ed231701a4f0f43778cae2dd0389bffb23de3d9596029ddfb4cc`  
		Last Modified: Wed, 26 Oct 2022 20:29:45 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528dd9baaf0de5faa6896d397c81ea5e36406ff305f788dfbdbe5192cdae47b`  
		Last Modified: Wed, 26 Oct 2022 20:29:42 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1102316d9fbdf06487275aacff53ad9f16bc43813feaabcbeafc21da91bc4669`  
		Last Modified: Wed, 26 Oct 2022 20:29:42 GMT  
		Size: 4.5 KB (4506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790d774652bfa0418ce89a7f709b6dd2cbcca55262d1be69a323252c86ea5690`  
		Last Modified: Wed, 26 Oct 2022 20:29:42 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906e4ce11fd4ef4bf903429529f67328c7a8130516be2ff143b3dabacd673ac2`  
		Last Modified: Wed, 26 Oct 2022 20:29:43 GMT  
		Size: 183.4 KB (183395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be51d178a5092cb1ad5b51052bf3ccf28f29ccd4c52c5506fbe3d7e335b4b60`  
		Last Modified: Wed, 26 Oct 2022 20:29:46 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.5.1`

```console
$ docker pull kibana@sha256:09d6267c4d0433f5a52d3ade36a518adfaab0ef1b43951a0c064cb0e00b2c914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.5.1` - linux; amd64

```console
$ docker pull kibana@sha256:2a1a2a86bfcaecb6d7917f9981ad96d505bd879a7ea78649d9d8ff540894733c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (282986584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a5dbfe4bf27f49e2717a021e936de38db6c89b7e154aeecc99979fcef2f5aa5`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Wed, 09 Nov 2022 14:39:24 GMT
EXPOSE map[5601/tcp:{}]
# Wed, 09 Nov 2022 14:39:24 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Wed, 09 Nov 2022 14:39:25 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Wed, 09 Nov 2022 14:39:26 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Wed, 09 Nov 2022 14:39:26 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Wed, 09 Nov 2022 14:39:27 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Wed, 09 Nov 2022 14:39:27 GMT
RUN fc-cache -v # buildkit
# Wed, 09 Nov 2022 14:40:30 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Wed, 09 Nov 2022 14:40:30 GMT
WORKDIR /usr/share/kibana
# Wed, 09 Nov 2022 14:40:30 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Wed, 09 Nov 2022 14:40:30 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 09 Nov 2022 14:40:30 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Nov 2022 14:40:30 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Wed, 09 Nov 2022 14:40:30 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Wed, 09 Nov 2022 14:40:31 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Wed, 09 Nov 2022 14:40:31 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Wed, 09 Nov 2022 14:40:32 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Wed, 09 Nov 2022 14:40:32 GMT
LABEL org.label-schema.build-date=2022-11-09T14:16:54.640Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=87149bfd06f4fe41dbfa7e95461294e9dadfb1d8 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.5.1 org.opencontainers.image.created=2022-11-09T14:16:54.640Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=87149bfd06f4fe41dbfa7e95461294e9dadfb1d8 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.5.1
# Wed, 09 Nov 2022 14:40:32 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 09 Nov 2022 14:40:32 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Wed, 09 Nov 2022 14:40:32 GMT
USER kibana
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce1cd9cae9c4bff25e47d50e0c3c03bd71ecc166a3ccf6d31fc488e81e58646`  
		Last Modified: Wed, 16 Nov 2022 08:55:52 GMT  
		Size: 10.5 MB (10514265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf5307afb23de394c9e80e9ac0a3cb408817a581cf0baff624b3985454f0dc1`  
		Last Modified: Wed, 16 Nov 2022 08:55:50 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c0371af101a7f7584d390dafa2288778c1917d28fdf87d18dc7d7f6a546ad2`  
		Last Modified: Wed, 16 Nov 2022 08:55:50 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee76862f97267fadf5a5ece5fbf9251146e5c798d9a8c2b2209149902438e97`  
		Last Modified: Wed, 16 Nov 2022 08:55:51 GMT  
		Size: 16.5 MB (16460474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9c3d75aef9be04823048157f8a2574de0b8b7140fe9f1a95101229773d56c1`  
		Last Modified: Wed, 16 Nov 2022 08:55:48 GMT  
		Size: 5.3 KB (5279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0683f3929ed9bcad849f9c04b5da9ae1945a52eb8e79927979c8893e0c13f4bb`  
		Last Modified: Wed, 16 Nov 2022 08:56:17 GMT  
		Size: 227.2 MB (227222428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b620023814f3765bc9dc32e760bcc22404f40c7e31a01ff25996643b9007a4f4`  
		Last Modified: Wed, 16 Nov 2022 08:55:48 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4edced3e1f061e4323fcf61e79c7a9819705411b1ab287c5713c9c0779a7754`  
		Last Modified: Wed, 16 Nov 2022 08:55:48 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e51f0498a02fca87f9aa748dbec55fd1e835f8401f127d39f8bb3094c9c07d`  
		Last Modified: Wed, 16 Nov 2022 08:55:46 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6bd0d772405268e8ce28fecfc5f7b756feee2165138aa8f820384e55d0d9e2`  
		Last Modified: Wed, 16 Nov 2022 08:55:46 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b6fe4d253c69562a2a75f1d799fdc81a1c21355a09743327819372532303dd`  
		Last Modified: Wed, 16 Nov 2022 08:55:46 GMT  
		Size: 189.4 KB (189391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcdfee0cf97e07d022b301fec2de201f15f6eee1461dfb3a9205db1e73f4e1a`  
		Last Modified: Wed, 16 Nov 2022 08:55:46 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.5.1` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:12af670cba9834e484c17cb1fd8cfcad4d2f9d3b20ef04869febff5028125c50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297870452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9757a5fce14fd7de2fb2087451f11f84e8f48c610a3f1307dba09cb8d912aff`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 09 Nov 2022 14:42:26 GMT
EXPOSE map[5601/tcp:{}]
# Wed, 09 Nov 2022 14:42:26 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Wed, 09 Nov 2022 14:42:28 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Wed, 09 Nov 2022 14:42:28 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Wed, 09 Nov 2022 14:42:31 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Wed, 09 Nov 2022 14:42:32 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Wed, 09 Nov 2022 14:42:32 GMT
RUN fc-cache -v # buildkit
# Wed, 09 Nov 2022 14:43:30 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Wed, 09 Nov 2022 14:43:30 GMT
WORKDIR /usr/share/kibana
# Wed, 09 Nov 2022 14:43:30 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Wed, 09 Nov 2022 14:43:30 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 09 Nov 2022 14:43:30 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Nov 2022 14:43:30 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Wed, 09 Nov 2022 14:43:30 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Wed, 09 Nov 2022 14:43:31 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Wed, 09 Nov 2022 14:43:32 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Wed, 09 Nov 2022 14:43:33 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Wed, 09 Nov 2022 14:43:33 GMT
LABEL org.label-schema.build-date=2022-11-09T14:16:54.640Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=87149bfd06f4fe41dbfa7e95461294e9dadfb1d8 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.5.1 org.opencontainers.image.created=2022-11-09T14:16:54.640Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=87149bfd06f4fe41dbfa7e95461294e9dadfb1d8 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.5.1
# Wed, 09 Nov 2022 14:43:33 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 09 Nov 2022 14:43:33 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Wed, 09 Nov 2022 14:43:33 GMT
USER kibana
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcdffed6688eb0fb9e6b5b71b1b2b2cb5002c334f13a52b83fcb5d8705af441`  
		Last Modified: Wed, 16 Nov 2022 20:05:53 GMT  
		Size: 10.4 MB (10382841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff47e994a0db17adf6c88e1188c2e28889f4a0b9baa1cd589a001f01b8a3903`  
		Last Modified: Wed, 16 Nov 2022 20:05:50 GMT  
		Size: 9.1 KB (9101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ef174be10b2c35e435596e6b54006d48ceae130380c235d379227842104af1`  
		Last Modified: Wed, 16 Nov 2022 20:05:50 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81676bac6d92b44ede75b987e5ef7dad32315b272700d948cd85da9e3732d9c2`  
		Last Modified: Wed, 16 Nov 2022 20:05:49 GMT  
		Size: 16.5 MB (16460471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da60965156d69918124a71247fdec526a66586ae9e62add40a5479dc20cd778`  
		Last Modified: Wed, 16 Nov 2022 20:05:48 GMT  
		Size: 5.3 KB (5290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f62b2a462f2a6d4e8ed997289447dee0017e6c744101b105806a2f8a72d9543`  
		Last Modified: Wed, 16 Nov 2022 20:06:12 GMT  
		Size: 243.6 MB (243625964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ac0e44cf2f8506e741229ee6231a6bf61a76fc9124d6291e6a5417d718ccc4`  
		Last Modified: Wed, 16 Nov 2022 20:05:47 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fe14c89e122dcda2b585dfc5b65a93a74380c43a596130a2f5c48b8a109ada`  
		Last Modified: Wed, 16 Nov 2022 20:05:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd916f37803a1da5f39ddb527d7bd46cc6dc111aec8d525538ba5bf0c62f3e`  
		Last Modified: Wed, 16 Nov 2022 20:05:45 GMT  
		Size: 4.4 KB (4417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b188b9ca49bac72b55bb4246b8d44db9a5d89a602f414c9f56c513c0791d826d`  
		Last Modified: Wed, 16 Nov 2022 20:05:45 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7549169a333ff9544f0f55db0ae7369e4dc23db6a14703f2fdc25205985ca16`  
		Last Modified: Wed, 16 Nov 2022 20:05:46 GMT  
		Size: 183.4 KB (183395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350ea9e4de704f008e8abe75fb7ac3200ad54fe1b7d687d15fc6dfc71941ba3f`  
		Last Modified: Wed, 16 Nov 2022 20:05:51 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
