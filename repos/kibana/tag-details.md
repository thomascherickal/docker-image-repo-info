<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:7.17.16`](#kibana71716)
-	[`kibana:8.11.2`](#kibana8112)
-	[`kibana:8.11.3`](#kibana8113)

## `kibana:7.17.16`

```console
$ docker pull kibana@sha256:60674b95c97e0964a2a5eed7526378807a5aac4520e860a2bd15c5e9095f3327
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `kibana:7.17.16` - linux; amd64

```console
$ docker pull kibana@sha256:f8502de7578108d37ad4ae3f74029e14ee7bd29ab27df0b839d5a4e2e32a6ec9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.2 MB (363216223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:714310cc818cb5dd9cc98ed18e635c0426e3a473d26a08261f4a04fb8aecfe0d`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Tue, 12 Dec 2023 12:49:29 GMT
EXPOSE map[5601/tcp:{}]
# Tue, 12 Dec 2023 12:49:29 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN fc-cache -v # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
WORKDIR /usr/share/kibana
# Tue, 12 Dec 2023 12:49:29 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 12:49:29 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 12:49:29 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.label-schema.build-date=2023-12-08T12:07:39.833Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=5838d16e60eb684b785702c80ff41e59d344fe1f org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.16 org.opencontainers.image.created=2023-12-08T12:07:39.833Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=5838d16e60eb684b785702c80ff41e59d344fe1f org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.16
# Tue, 12 Dec 2023 12:49:29 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Tue, 12 Dec 2023 12:49:29 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Tue, 12 Dec 2023 12:49:29 GMT
USER kibana
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1816d1c2cd504d823315846b372348e6a7d42a281f1a57f075a6e57871e969ec`  
		Last Modified: Thu, 14 Dec 2023 18:52:30 GMT  
		Size: 17.4 MB (17362832 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6175ec2ba3b2fff80624557bcd8e3face847d535a6d256159b80caaa93924f21`  
		Last Modified: Thu, 14 Dec 2023 18:52:30 GMT  
		Size: 9.5 KB (9525 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbe841c581e2b115f898de7063aaa2a30b951f3dd5f2766ca0b076352793daa4`  
		Last Modified: Thu, 14 Dec 2023 18:52:30 GMT  
		Size: 158.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13eeb291182da62a01b278d7e5c77a67edb11ffef02edf3e5962005c4eb1ad10`  
		Last Modified: Thu, 14 Dec 2023 18:52:30 GMT  
		Size: 16.5 MB (16460476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da987fae49ee010d644562b35a79f6d9de6f5d8ed3ce2ec9a0bb0b299a800639`  
		Last Modified: Thu, 14 Dec 2023 18:52:31 GMT  
		Size: 5.3 KB (5299 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f48cc57395e195e9a0e056dc97163906f6e55df5d36a9b6e0520ebb6f4c9eb8b`  
		Last Modified: Thu, 14 Dec 2023 18:52:35 GMT  
		Size: 301.7 MB (301668681 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2840da6b187d059b6c0d03bcb7cbcfd5863a5458041a559a58a768833a751380`  
		Last Modified: Thu, 14 Dec 2023 18:52:31 GMT  
		Size: 133.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d452835fffd0e3be4c86a2a8c79d5eb77ace37121c61db5c081029ad0f53b0fd`  
		Last Modified: Thu, 14 Dec 2023 18:52:31 GMT  
		Size: 396.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b0365c7fae604106912e3ce68236d36c50315ce59f293df93bf6cdccdeed367`  
		Last Modified: Thu, 14 Dec 2023 18:52:31 GMT  
		Size: 4.5 KB (4503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05bb75c4e234fa8ea8d9b2ddd24c45b53b8615792a69928cee4b20fd7469110b`  
		Last Modified: Thu, 14 Dec 2023 18:52:32 GMT  
		Size: 399.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:873c5439aae097d13eacd32e0a83da2d7a49ec79b5fb4cdf1a084633c0246293`  
		Last Modified: Thu, 14 Dec 2023 18:52:33 GMT  
		Size: 189.4 KB (189403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a8c625146cc61b6082afa47fde3e074000dd6e40160bb44f7215f085e23a35f`  
		Last Modified: Thu, 14 Dec 2023 18:52:32 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `kibana:7.17.16` - unknown; unknown

```console
$ docker pull kibana@sha256:0decec02ba88c248518d7e3eb59e1d2366744123978326df75136914b39b4f42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d155aa359f407b55d991ff06fac5c33688085a4e524a561f8f8c8fe84db0bec`

```dockerfile
```

-	Layers:
	-	`sha256:32a493ba81b3cb1a1eb56bb0844b06724b2f49f2622fdfc372b801ef5a6c352c`  
		Last Modified: Thu, 14 Dec 2023 18:52:30 GMT  
		Size: 3.0 MB (3033311 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b26f21003c74aea83fad7df94a28a114282a141937f792ccd66efc560d95d59c`  
		Last Modified: Thu, 14 Dec 2023 18:52:30 GMT  
		Size: 44.4 KB (44362 bytes)  
		MIME: application/vnd.in-toto+json

### `kibana:7.17.16` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:6078d57e115d77dfbbf9452c000e7ce8a558173a21eab46c3d55990dfcb62080
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.8 MB (372797121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3546836353b717e17907e0c4e9f571974f1e9f2ed8c91c1b1bd72991dc8df44`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Tue, 12 Dec 2023 12:49:29 GMT
EXPOSE map[5601/tcp:{}]
# Tue, 12 Dec 2023 12:49:29 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN fc-cache -v # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
WORKDIR /usr/share/kibana
# Tue, 12 Dec 2023 12:49:29 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 12:49:29 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 12:49:29 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.label-schema.build-date=2023-12-08T12:07:39.833Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=5838d16e60eb684b785702c80ff41e59d344fe1f org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.16 org.opencontainers.image.created=2023-12-08T12:07:39.833Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=5838d16e60eb684b785702c80ff41e59d344fe1f org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.16
# Tue, 12 Dec 2023 12:49:29 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Tue, 12 Dec 2023 12:49:29 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Tue, 12 Dec 2023 12:49:29 GMT
USER kibana
```

-	Layers:
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec7b9b673d1f38d790ba00a6b0a2b21e6ea18dd9f4537c083eddc6bbdfdc3cff`  
		Last Modified: Tue, 12 Dec 2023 17:41:49 GMT  
		Size: 16.2 MB (16165862 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c073b1761863e0d1beeb60203630174ed135cfeffb9033dfac9b84aa6b697e5d`  
		Last Modified: Tue, 12 Dec 2023 17:41:48 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024793d7ef48c7554626bb0ccbe18d80cf9279447bca7a3cb49f4406f071f147`  
		Last Modified: Tue, 12 Dec 2023 17:41:48 GMT  
		Size: 159.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:573567f098043382fde2a7e3904b509735390fc037c5d6cac70129ea669c92f3`  
		Last Modified: Tue, 12 Dec 2023 17:41:50 GMT  
		Size: 16.5 MB (16460474 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8df14c4bedca0ed95701450a2e5c08b6b7d7a185432735fd90785f720711e8f`  
		Last Modified: Tue, 12 Dec 2023 17:41:49 GMT  
		Size: 5.3 KB (5296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18dd0eeaf8f6fb432c1c3a2570df8b715443ada7aeca0833db4f8381caa34027`  
		Last Modified: Thu, 14 Dec 2023 19:47:10 GMT  
		Size: 314.0 MB (313990022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9cc493b77fac0b4252b3fd1c7b4358b349eaf326b8a60920d45a96f1a7a88253`  
		Last Modified: Thu, 14 Dec 2023 19:47:03 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a368d95d53303e354a8ad5157247a6d19067f6621bd413e16dfe66e119ec7d3`  
		Last Modified: Thu, 14 Dec 2023 19:47:03 GMT  
		Size: 396.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d163ea4cdb5efd985e695f43939246d308fb3be32e3943de40c795f6bae23660`  
		Last Modified: Thu, 14 Dec 2023 19:47:03 GMT  
		Size: 4.5 KB (4505 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5328160d73ddc1bc870bb4a5e6ae229f064326d995bd516bc75417ebb9d78023`  
		Last Modified: Thu, 14 Dec 2023 19:47:04 GMT  
		Size: 399.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c1db5460dd0ebad393a76423350903831058ffd1d4ff153776e5b91d8041619`  
		Last Modified: Tue, 12 Dec 2023 17:41:52 GMT  
		Size: 183.4 KB (183409 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69a9264b770446de536f9e6a6daabed62ce9908ba928f100901a0d8904210df3`  
		Last Modified: Thu, 14 Dec 2023 19:47:05 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `kibana:7.17.16` - unknown; unknown

```console
$ docker pull kibana@sha256:541493bed202b955549a8d8ff303e275557129edeb0ab0778c706eae1eea2565
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17753bd5ddc66b2e915010ee24b14369db347f11495f5ef8bec3e05de4c8497a`

```dockerfile
```

-	Layers:
	-	`sha256:dc227d0c2b5d898252de8fbd7baa0604ea48325399655bfb175656d5609936bc`  
		Last Modified: Thu, 14 Dec 2023 19:47:03 GMT  
		Size: 3.0 MB (3033652 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:57363a75a6f1b3355bcaa20c9caf8ae3753bd3ff625d65d8ffc5d98da5757847`  
		Last Modified: Thu, 14 Dec 2023 19:47:02 GMT  
		Size: 44.2 KB (44206 bytes)  
		MIME: application/vnd.in-toto+json

## `kibana:8.11.2`

```console
$ docker pull kibana@sha256:98cbf9f0eb81a9e3182c9bfbc7e7869c3e654122c6bf2cf2d54ec00b1e800bd9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `kibana:8.11.2` - linux; amd64

```console
$ docker pull kibana@sha256:47afeae7c49cf2b842265a841eea9e5ec00654a430b436abcf466dfa74000c8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.7 MB (375697403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b787e0da3c9ae61d6d606654766beaea10239acf2d5538b1e4b62cbc9835b010`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Thu, 07 Dec 2023 12:34:16 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 07 Dec 2023 12:34:16 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN fc-cache -v # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
WORKDIR /usr/share/kibana
# Thu, 07 Dec 2023 12:34:16 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 07 Dec 2023 12:34:16 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Dec 2023 12:34:16 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.label-schema.build-date=2023-12-05T12:05:54.257Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=92746356b61c3e3ac62b6d7045727f8d737fa4b5 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.11.2 org.opencontainers.image.created=2023-12-05T12:05:54.257Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=92746356b61c3e3ac62b6d7045727f8d737fa4b5 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.2
# Thu, 07 Dec 2023 12:34:16 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 07 Dec 2023 12:34:16 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 07 Dec 2023 12:34:16 GMT
USER kibana
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5fd2342533ef3867e45bb0343ae11cb6ee25c6edad60cf59792eadc985db08a`  
		Last Modified: Thu, 14 Dec 2023 18:53:19 GMT  
		Size: 17.4 MB (17362873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87bd4d7599f1856813a46f6746b61608a47b66f7277fc3259a7acd4280167024`  
		Last Modified: Thu, 14 Dec 2023 18:53:19 GMT  
		Size: 9.5 KB (9525 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b1e19d40d7e66fe9e935b27b139e9914ab0cf165106a64d049f8f3b5db3b1fc`  
		Last Modified: Thu, 14 Dec 2023 18:53:18 GMT  
		Size: 158.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:629bbbf2d619383c329380984b777cee91f7d00bbf68a2e25aa9064d00699982`  
		Last Modified: Thu, 14 Dec 2023 18:53:20 GMT  
		Size: 16.5 MB (16460488 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8bc55c13617bb63f53e937515e1994376e3acd6f9273e336ed5521992f635177`  
		Last Modified: Thu, 14 Dec 2023 18:53:20 GMT  
		Size: 5.3 KB (5286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47232ac250f2cc84dc0b2226ef835fab15ef0ac896fe351999cdbf7a5a8df220`  
		Last Modified: Thu, 14 Dec 2023 18:53:27 GMT  
		Size: 314.1 MB (314149761 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eeb55d4c81e3f1c7da2feaf7d677c83fb530c03c1fa2b5f36e6bee632ae109d2`  
		Last Modified: Thu, 14 Dec 2023 18:53:21 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23c859d63fa1185f91d3612ca9f79262fff6beee516949f9bf8c09c4d44ca50c`  
		Last Modified: Thu, 14 Dec 2023 18:53:21 GMT  
		Size: 396.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d156dc2f30e4fc29499827d005a7526214d3968b592697ac14aa335858c441e`  
		Last Modified: Thu, 14 Dec 2023 18:53:21 GMT  
		Size: 4.6 KB (4555 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7fa98f8f28a98372806fb43ac6a93fd341b8191a7f77fe1e325e8cb8904689ca`  
		Last Modified: Thu, 14 Dec 2023 18:53:22 GMT  
		Size: 400.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0382bbe265a9a19fd3a6d5fb1396f2f53ff4478ffc7aebed0d88fdf9d80a6290`  
		Last Modified: Thu, 14 Dec 2023 18:53:22 GMT  
		Size: 189.4 KB (189404 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65f124100a9c32471f7259463b2a8ab360e7270231e2704945c3438c6d4e16c1`  
		Last Modified: Thu, 14 Dec 2023 18:53:23 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `kibana:8.11.2` - unknown; unknown

```console
$ docker pull kibana@sha256:b670e4b663fe11493b9de3d9169d50e3c6e6ffa2a713fcafa826b86d558562e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3481554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b628eec603f4fb9b77626e6b73ec8beb1fad7441472f1050faf35a901bc4afe8`

```dockerfile
```

-	Layers:
	-	`sha256:ba768fab692e9a88ec56da80580f182352142f31c63078b83815f810e6cf34d3`  
		Last Modified: Thu, 14 Dec 2023 18:53:19 GMT  
		Size: 3.4 MB (3437198 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9082a573ff4bd22e37cb85c67f1674f318f7bd4aa5615cb1b0be08d5445e89f4`  
		Last Modified: Thu, 14 Dec 2023 18:53:19 GMT  
		Size: 44.4 KB (44356 bytes)  
		MIME: application/vnd.in-toto+json

### `kibana:8.11.2` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:82ea470abb05bc1ec2905d74270662b1ffa3f2216b6a2c79a860072ed4830172
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.5 MB (385455045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6120b6f0b93a94825d05068f973f1d8aaff615ac2fd27a9667ea65350ebba8f2`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Thu, 07 Dec 2023 12:34:16 GMT
EXPOSE map[5601/tcp:{}]
# Thu, 07 Dec 2023 12:34:16 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN fc-cache -v # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
WORKDIR /usr/share/kibana
# Thu, 07 Dec 2023 12:34:16 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 07 Dec 2023 12:34:16 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Dec 2023 12:34:16 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.label-schema.build-date=2023-12-05T12:05:54.257Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=92746356b61c3e3ac62b6d7045727f8d737fa4b5 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.11.2 org.opencontainers.image.created=2023-12-05T12:05:54.257Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=92746356b61c3e3ac62b6d7045727f8d737fa4b5 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.2
# Thu, 07 Dec 2023 12:34:16 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Thu, 07 Dec 2023 12:34:16 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Thu, 07 Dec 2023 12:34:16 GMT
USER kibana
```

-	Layers:
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec7b9b673d1f38d790ba00a6b0a2b21e6ea18dd9f4537c083eddc6bbdfdc3cff`  
		Last Modified: Tue, 12 Dec 2023 17:41:49 GMT  
		Size: 16.2 MB (16165862 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c073b1761863e0d1beeb60203630174ed135cfeffb9033dfac9b84aa6b697e5d`  
		Last Modified: Tue, 12 Dec 2023 17:41:48 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024793d7ef48c7554626bb0ccbe18d80cf9279447bca7a3cb49f4406f071f147`  
		Last Modified: Tue, 12 Dec 2023 17:41:48 GMT  
		Size: 159.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:573567f098043382fde2a7e3904b509735390fc037c5d6cac70129ea669c92f3`  
		Last Modified: Tue, 12 Dec 2023 17:41:50 GMT  
		Size: 16.5 MB (16460474 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8df14c4bedca0ed95701450a2e5c08b6b7d7a185432735fd90785f720711e8f`  
		Last Modified: Tue, 12 Dec 2023 17:41:49 GMT  
		Size: 5.3 KB (5296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59b59806b11a9ffe3a3c26543ef7672ef96cf77c0ead7da03b70104b2edc95ad`  
		Last Modified: Thu, 14 Dec 2023 19:43:51 GMT  
		Size: 326.6 MB (326647897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df5a775da8742dac72a8ae8c8882d9cd5b517a2a046bf735adbe0d34ced7ca32`  
		Last Modified: Thu, 14 Dec 2023 19:43:43 GMT  
		Size: 131.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c19072b78b7e5488b49440708e740b39375661d2b4a3fca041d34fbb8a8e591e`  
		Last Modified: Thu, 14 Dec 2023 19:43:43 GMT  
		Size: 397.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0121cb675b6edc489bbe6dca9cbdcf9da680adfaf16067a27b992f8dcb1ed7a1`  
		Last Modified: Thu, 14 Dec 2023 19:43:43 GMT  
		Size: 4.6 KB (4554 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1702634fde8d03114c9ce1186b5bf1e3a5b4815c39b3b9375220952fcd435e1`  
		Last Modified: Thu, 14 Dec 2023 19:43:44 GMT  
		Size: 401.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c1db5460dd0ebad393a76423350903831058ffd1d4ff153776e5b91d8041619`  
		Last Modified: Tue, 12 Dec 2023 17:41:52 GMT  
		Size: 183.4 KB (183409 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e385d24b09c2d8222a56427db8ae00d1a0024db02c9f298a1b780fa8986f87aa`  
		Last Modified: Thu, 14 Dec 2023 19:43:44 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `kibana:8.11.2` - unknown; unknown

```console
$ docker pull kibana@sha256:2ba285b4f05a32e7e42bdc51a4aae3e55d9f843de1464156f1f870ec889bf700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3481738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:314f6026ddde392f8dc9f7ac058f0cb4979b66c3e49d5d98db55a8f76e333982`

```dockerfile
```

-	Layers:
	-	`sha256:d46ca866dcdd846c5d8d86cdecf8da60ca76ddd72800ad78a152c3847029db51`  
		Last Modified: Thu, 14 Dec 2023 19:43:43 GMT  
		Size: 3.4 MB (3437539 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d5ea55504936f02a81cb05476f83f55c82ad7dbb8ebd39e2f6dda62f7e5bf59`  
		Last Modified: Thu, 14 Dec 2023 19:43:43 GMT  
		Size: 44.2 KB (44199 bytes)  
		MIME: application/vnd.in-toto+json

## `kibana:8.11.3`

```console
$ docker pull kibana@sha256:cd2006c19023837fae89392547e462957f9b87bfa781eec4fdfd9007ce3db9db
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `kibana:8.11.3` - linux; amd64

```console
$ docker pull kibana@sha256:b47ce47b9746cec56e185bf9b7d2951cbc8679b3b10b9b0a441f08b5f3144f17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.7 MB (375698330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228964c3bf6f248c4986b7619863ebcbf7c33e29e84ded64beaeef713d99bacd`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Tue, 12 Dec 2023 13:07:20 GMT
EXPOSE map[5601/tcp:{}]
# Tue, 12 Dec 2023 13:07:20 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN fc-cache -v # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
WORKDIR /usr/share/kibana
# Tue, 12 Dec 2023 13:07:20 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 13:07:20 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 13:07:20 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.label-schema.build-date=2023-12-08T16:30:01.542Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=cc11667953f4734af414e8d8977b8d9dda5698ef org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.11.3 org.opencontainers.image.created=2023-12-08T16:30:01.542Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=cc11667953f4734af414e8d8977b8d9dda5698ef org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.3
# Tue, 12 Dec 2023 13:07:20 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Tue, 12 Dec 2023 13:07:20 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Tue, 12 Dec 2023 13:07:20 GMT
USER kibana
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e794b3eaffd1698b2ce4d7f9ba74b8812237d31a60d593b335ba84b10ae113e7`  
		Last Modified: Thu, 14 Dec 2023 18:53:21 GMT  
		Size: 17.4 MB (17362961 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:83504a32f59ec7363c8c95e99161a27650b35babd5f1ff5c4fe297381e7123f5`  
		Last Modified: Thu, 14 Dec 2023 18:53:20 GMT  
		Size: 9.5 KB (9525 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df699dc3f050db3472ac2cd2f4d81d0e6f38d40682c306196f8cfc8266b4ba1e`  
		Last Modified: Thu, 14 Dec 2023 18:53:20 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab14a5c4f1db757f58c42ddecad85abaa8771976f9053b7cc27fe3ffc9edc972`  
		Last Modified: Thu, 14 Dec 2023 18:53:21 GMT  
		Size: 16.5 MB (16460489 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12463f0670e3468aaa13f0c7526ca5522e4466155da3e9b47937a4aa8de6047f`  
		Last Modified: Thu, 14 Dec 2023 18:53:21 GMT  
		Size: 5.3 KB (5302 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26718126203d5d5c1fff85986f480267a3575c3cfc4eac71821dc1197dbb61aa`  
		Last Modified: Thu, 14 Dec 2023 18:53:28 GMT  
		Size: 314.2 MB (314150581 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:93820a9bc1628eb5173320b4a910886ad0ac0776e5830e5b02e5dcab149b5f92`  
		Last Modified: Thu, 14 Dec 2023 18:53:22 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:654bdb608b4ff7b83d0243eb0fed9af028657b584f9b605a545bb039f0f22d46`  
		Last Modified: Thu, 14 Dec 2023 18:53:22 GMT  
		Size: 397.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:88c68bf14a26effceb3a41666e49fa238af84a72602a6fafacf0bb035e78269e`  
		Last Modified: Thu, 14 Dec 2023 18:53:22 GMT  
		Size: 4.6 KB (4554 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f145f03c873fd3961b5ba433c3e40292866ad68be9b16826232939c5d4bbf2a`  
		Last Modified: Thu, 14 Dec 2023 18:53:23 GMT  
		Size: 401.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f87624960a7fa990053b7fd1d89005b237bc37b09d6f9ad627f26c34ba726b8`  
		Last Modified: Thu, 14 Dec 2023 18:53:23 GMT  
		Size: 189.4 KB (189404 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27c75980b896d17e9e22bdac31f42dde5f96968a70bc2f2c388cfcea359addf6`  
		Last Modified: Thu, 14 Dec 2023 18:53:23 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `kibana:8.11.3` - unknown; unknown

```console
$ docker pull kibana@sha256:e6e8a799e055befe4a591de2641cbd4d4274b834a7cee5877d2f90d72a075783
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3480479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feb9f3f88b0cf9c511c233d01f5c28056d9c0f629e640de72a30f70d0d3f4704`

```dockerfile
```

-	Layers:
	-	`sha256:8c527f89611098850d88acf39bc8e557ce275f3c85bc571709b87d965db23fb0`  
		Last Modified: Thu, 14 Dec 2023 18:53:20 GMT  
		Size: 3.4 MB (3436123 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ceb4f5a683d27c2e5bb4bd1e2799b1bd0e43495241ec78c0a3622f7b1466f76a`  
		Last Modified: Thu, 14 Dec 2023 18:53:20 GMT  
		Size: 44.4 KB (44356 bytes)  
		MIME: application/vnd.in-toto+json

### `kibana:8.11.3` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:3251dbb0dcfc8cf5c48959b7532a4625b75acdcd2e59c19a9648dedab426411f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.5 MB (385453216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b211f93eacc6025cf8f7a17b5213be81bac6776d08990f2eccc22a437a00e56`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Tue, 12 Dec 2023 13:07:20 GMT
EXPOSE map[5601/tcp:{}]
# Tue, 12 Dec 2023 13:07:20 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN mkdir /usr/share/fonts/local # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN fc-cache -v # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY /usr/share/kibana /usr/share/kibana # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
WORKDIR /usr/share/kibana
# Tue, 12 Dec 2023 13:07:20 GMT
RUN ln -s /usr/share/kibana /opt/kibana # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 13:07:20 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 13:07:20 GMT
COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.label-schema.build-date=2023-12-08T16:30:01.542Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=cc11667953f4734af414e8d8977b8d9dda5698ef org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.11.3 org.opencontainers.image.created=2023-12-08T16:30:01.542Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=cc11667953f4734af414e8d8977b8d9dda5698ef org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.3
# Tue, 12 Dec 2023 13:07:20 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Tue, 12 Dec 2023 13:07:20 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Tue, 12 Dec 2023 13:07:20 GMT
USER kibana
```

-	Layers:
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec7b9b673d1f38d790ba00a6b0a2b21e6ea18dd9f4537c083eddc6bbdfdc3cff`  
		Last Modified: Tue, 12 Dec 2023 17:41:49 GMT  
		Size: 16.2 MB (16165862 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c073b1761863e0d1beeb60203630174ed135cfeffb9033dfac9b84aa6b697e5d`  
		Last Modified: Tue, 12 Dec 2023 17:41:48 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024793d7ef48c7554626bb0ccbe18d80cf9279447bca7a3cb49f4406f071f147`  
		Last Modified: Tue, 12 Dec 2023 17:41:48 GMT  
		Size: 159.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:573567f098043382fde2a7e3904b509735390fc037c5d6cac70129ea669c92f3`  
		Last Modified: Tue, 12 Dec 2023 17:41:50 GMT  
		Size: 16.5 MB (16460474 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8df14c4bedca0ed95701450a2e5c08b6b7d7a185432735fd90785f720711e8f`  
		Last Modified: Tue, 12 Dec 2023 17:41:49 GMT  
		Size: 5.3 KB (5296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d2748d460361ce850e9fde1233aa670dd9f13acf0b565209b87560fdef37bafa`  
		Last Modified: Thu, 14 Dec 2023 19:39:13 GMT  
		Size: 326.6 MB (326646068 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b41cb23bdf7f6d743966b43b93cc5d3b38feb80872691299f7a43f3ecb2e147`  
		Last Modified: Thu, 14 Dec 2023 19:39:04 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47b2fb1a5ed3bc10d51c3b7839664ca5de65929d2e58580c73003c984f4b39d5`  
		Last Modified: Thu, 14 Dec 2023 19:39:04 GMT  
		Size: 397.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d37a43c56434573d150fee3c82cf8b40135e1afbc49dd633dead36f627cdd912`  
		Last Modified: Thu, 14 Dec 2023 19:39:04 GMT  
		Size: 4.6 KB (4552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:076e46ba55c4cfc00992224aac1c2787293d991e44996ba6f714596069a04d7c`  
		Last Modified: Thu, 14 Dec 2023 19:39:05 GMT  
		Size: 401.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c1db5460dd0ebad393a76423350903831058ffd1d4ff153776e5b91d8041619`  
		Last Modified: Tue, 12 Dec 2023 17:41:52 GMT  
		Size: 183.4 KB (183409 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96b9a49ca4063929cda8decc0d973a50b88e339cfd2ac99a2cf0c715fab99bc6`  
		Last Modified: Thu, 14 Dec 2023 19:39:05 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `kibana:8.11.3` - unknown; unknown

```console
$ docker pull kibana@sha256:667efe78f534dc44f18a80763d202873363efbc61a60bcc65e2bc76fb61d9f36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3480663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc415d91f08ef95cac059093dc9d046a8228f83e1317215d1cdb3d5ca5cf9830`

```dockerfile
```

-	Layers:
	-	`sha256:fe157d00ce62c201578213548ff71cc9beb579f63d5965a0fbb714546600a885`  
		Last Modified: Thu, 14 Dec 2023 19:39:04 GMT  
		Size: 3.4 MB (3436464 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d6d526d4a8306a8dae53fa41338f7f0438c0997a18ebed560b4c044e7bcfe82`  
		Last Modified: Thu, 14 Dec 2023 19:39:04 GMT  
		Size: 44.2 KB (44199 bytes)  
		MIME: application/vnd.in-toto+json
