<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.16`](#elasticsearch71716)
-	[`elasticsearch:8.11.2`](#elasticsearch8112)
-	[`elasticsearch:8.11.3`](#elasticsearch8113)

## `elasticsearch:7.17.16`

```console
$ docker pull elasticsearch@sha256:a77c043ee446165cb78e288a0232e5af767f24911647e59d8c44cec352823894
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `elasticsearch:7.17.16` - linux; amd64

```console
$ docker pull elasticsearch@sha256:2701b3b14cede7427a1b1c431329d116c148b046e0fd51e1692ff4fc7b85609d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.8 MB (359794117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697bd265a575670964f47521902556d61d9c2f7f171415cd9b64ebd9532b7d24`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 12 Dec 2023 12:49:29 GMT
ARG RELEASE
# Tue, 12 Dec 2023 12:49:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 12 Dec 2023 12:49:29 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Tue, 12 Dec 2023 12:49:29 GMT
CMD ["/bin/bash"]
# Tue, 12 Dec 2023 12:49:29 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 12:49:29 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 12 Dec 2023 12:49:29 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
COPY /bin/tini /bin/tini # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 12:49:29 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.label-schema.build-date=2023-12-08T10:06:54.672540567Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=2b23fa076334f8d4651aeebe458a955a2ae23218 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.16 org.opencontainers.image.created=2023-12-08T10:06:54.672540567Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=2b23fa076334f8d4651aeebe458a955a2ae23218 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.16
# Tue, 12 Dec 2023 12:49:29 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 12 Dec 2023 12:49:29 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:527f5363b98e562da03d2e0bbf86fd7c34f487bffd9b27a3cf0a9afea2f0ee1f`  
		Last Modified: Wed, 13 Dec 2023 10:48:59 GMT  
		Size: 27.5 MB (27512774 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e0392900c090e0874026902fcf47570efe46a3ad865442d3405133fd9d5d1f2`  
		Last Modified: Sat, 16 Dec 2023 10:49:40 GMT  
		Size: 7.5 MB (7507967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:048e1fb8f2e7018d4149fa020b7d8a86ebf994b3bfda9c7082ad280bec5bd497`  
		Last Modified: Sat, 16 Dec 2023 10:49:39 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df07542030d0683cfb3c2e788a23ba0f6d3e68a570b52c6c5ca9189f63f60998`  
		Last Modified: Sat, 16 Dec 2023 10:49:45 GMT  
		Size: 324.5 MB (324455734 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d4ccccfb1b809375ba9cee7a276f6f8dbe3fa587c07c724cb95405027b7ff05`  
		Last Modified: Sat, 16 Dec 2023 10:49:40 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e174847d32055c4f97fc38e1daaf8a0bd99bbc714d73a81c37d4f92cc1dd0570`  
		Last Modified: Sat, 16 Dec 2023 10:49:41 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:115f8c3340002597eda9bbe5dde18ac80b13821d4584862dd0a44dbf270ca872`  
		Last Modified: Sat, 16 Dec 2023 10:49:41 GMT  
		Size: 192.1 KB (192139 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74a5da86cfd8a041da96c5ef53efaae037ef64f0c1591386ef3660ae95c17daf`  
		Last Modified: Sat, 16 Dec 2023 10:49:41 GMT  
		Size: 405.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d5f9700eab1ef95eaab31593030f82816b1ce3234f472ae3ac8664da930aa3c`  
		Last Modified: Sat, 16 Dec 2023 10:49:42 GMT  
		Size: 109.2 KB (109248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:7.17.16` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:73c70f673d17ac6df8e8403ef165b737e40d8bcc15b5d5a9bea2c314d95bdd5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2107517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20a956f437c186cf5a8e522464fc3f8da1d78c95870b6a288e89d05d399b25b2`

```dockerfile
```

-	Layers:
	-	`sha256:14b741a0405c8c20b72a53d0ce8a6944da335bf2d76a17c2f9c4d0819b23ef6b`  
		Last Modified: Sat, 16 Dec 2023 10:49:39 GMT  
		Size: 2.1 MB (2069775 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7b83c7b1dc543de472b4aeda9f41214bf0c4d7b104b259272be0a5cd3531ee5d`  
		Last Modified: Sat, 16 Dec 2023 10:49:39 GMT  
		Size: 37.7 KB (37742 bytes)  
		MIME: application/vnd.in-toto+json

### `elasticsearch:7.17.16` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:4c89c8c1bdadcd6e9ebf2c37580a61e37093cd3143e2399b00ff4bdb92c41644
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.8 MB (361784660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a1e8fc8a9e6895c208a233c6adcd9fb468022ca6e66bcc98e39e2a118a1f1b`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

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
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 12:49:29 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 12 Dec 2023 12:49:29 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
COPY /bin/tini /bin/tini # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 12:49:29 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.label-schema.build-date=2023-12-08T10:06:54.672540567Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=2b23fa076334f8d4651aeebe458a955a2ae23218 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.16 org.opencontainers.image.created=2023-12-08T10:06:54.672540567Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=2b23fa076334f8d4651aeebe458a955a2ae23218 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.16
# Tue, 12 Dec 2023 12:49:29 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 12 Dec 2023 12:49:29 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1cd4f99a610be444dfff1ae0c40ce13564f13e34b28c5be770e1d952eed9c6b`  
		Last Modified: Tue, 12 Dec 2023 17:49:40 GMT  
		Size: 13.1 MB (13103533 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbdf3ab269a14f2fe4e3711c51d1ca401e0b0ee05fbdac3182da784b5258f4b2`  
		Last Modified: Tue, 12 Dec 2023 17:49:39 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dba730edf31691b025ed8ba38962f964ff0563211f400a7a67684049f847fa52`  
		Last Modified: Thu, 14 Dec 2023 19:34:33 GMT  
		Size: 322.4 MB (322394350 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ffbdfed47dee0b7d1d7dc2425b987408ba8b659b7915e4370ee54eea228fd267`  
		Last Modified: Thu, 14 Dec 2023 19:34:25 GMT  
		Size: 9.1 KB (9101 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ec83c6ad1e9e66d694c8b4e9dfe08f8073086157a58d01b9575017f2ba2700f`  
		Last Modified: Thu, 14 Dec 2023 19:34:25 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22c098f9a5b6fbf5c278066822c12cf8badb1fe9f726072feae05dd6c877b3a7`  
		Last Modified: Thu, 14 Dec 2023 19:34:26 GMT  
		Size: 186.2 KB (186170 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:589c2b08fdbef037fcdfd3679d0ef2daaa6a279cbc376a7988543fa410f4fd65`  
		Last Modified: Thu, 14 Dec 2023 19:34:26 GMT  
		Size: 407.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f3383cf3663bcf1d013315adb1ad351a4076d2b5b4eee9e43135166285279f82`  
		Last Modified: Thu, 14 Dec 2023 19:34:27 GMT  
		Size: 109.2 KB (109250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:7.17.16` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:90deff51fd0cfdc86d2add7ea9354c5bdab551c3c78c25fe9eca701633e923e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2107692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36432870664415139a3852e880db1283f940bae9ac56c9cc0d8c0f070cc9aa0`

```dockerfile
```

-	Layers:
	-	`sha256:9cd9dad00e234302ab5bf8e9ddcfa0b3d1be7a41df1fa8c07f109e9b0909d154`  
		Last Modified: Thu, 14 Dec 2023 19:34:26 GMT  
		Size: 2.1 MB (2070098 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:73ccdf9ad71f431ce3f2e4c3b68a7e75be8061b14b000acd225779fe69b6ce29`  
		Last Modified: Thu, 14 Dec 2023 19:34:25 GMT  
		Size: 37.6 KB (37594 bytes)  
		MIME: application/vnd.in-toto+json

## `elasticsearch:8.11.2`

```console
$ docker pull elasticsearch@sha256:f18dfcc9ce0c53426fff398e0d1898cadcff9d38eca31df08897deed52a95513
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `elasticsearch:8.11.2` - linux; amd64

```console
$ docker pull elasticsearch@sha256:7ec8e6e6eb32522e42346288ddf87eb7a63ffb2afea47bb3d807b43213bb164c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **673.3 MB (673279297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd23e0d92af843760d60bddce650814844ed657923ddf401b49b8301befd0723`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Thu, 07 Dec 2023 12:34:16 GMT
ARG RELEASE
# Thu, 07 Dec 2023 12:34:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 07 Dec 2023 12:34:16 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Thu, 07 Dec 2023 12:34:16 GMT
CMD ["/bin/bash"]
# Thu, 07 Dec 2023 12:34:16 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 07 Dec 2023 12:34:16 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 07 Dec 2023 12:34:16 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Dec 2023 12:34:16 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.label-schema.build-date=2023-12-05T10:03:47.729926671Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=76013fa76dcbf144c886990c6290715f5dc2ae20 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.11.2 org.opencontainers.image.created=2023-12-05T10:03:47.729926671Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=76013fa76dcbf144c886990c6290715f5dc2ae20 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.2
# Thu, 07 Dec 2023 12:34:16 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 07 Dec 2023 12:34:16 GMT
CMD ["eswrapper"]
# Thu, 07 Dec 2023 12:34:16 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:527f5363b98e562da03d2e0bbf86fd7c34f487bffd9b27a3cf0a9afea2f0ee1f`  
		Last Modified: Wed, 13 Dec 2023 10:48:59 GMT  
		Size: 27.5 MB (27512774 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58c1b2d3060242e81915ea135bc9bcbd11f8a981ee26f1453db7dd8e2e8d1693`  
		Last Modified: Sat, 16 Dec 2023 10:50:29 GMT  
		Size: 7.5 MB (7507938 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:581503f8352f112b3935bd3fe47e04b75d9996fb6f16fd1afb8f4f800665179d`  
		Last Modified: Sat, 16 Dec 2023 10:50:29 GMT  
		Size: 4.3 KB (4309 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d29ac748c000264a4b5cc14719be283c76d670b22c4a84ea972c415f552a5fbc`  
		Last Modified: Sat, 16 Dec 2023 10:50:43 GMT  
		Size: 637.9 MB (637941465 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ccf24b99a884370c20573059ddcd56e4d713f08594189374a8a4f739ae0e5f94`  
		Last Modified: Sat, 16 Dec 2023 10:50:29 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:021f7a48ece6b33dad9927fb9665a38b788bf9742d268de0ca1b9097a66434e1`  
		Last Modified: Sat, 16 Dec 2023 10:50:30 GMT  
		Size: 1.7 KB (1721 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a22b2302c3a0b5a91ee54d72cf186bdc43046defc240efb50086d48d8b8a66ae`  
		Last Modified: Sat, 16 Dec 2023 10:50:30 GMT  
		Size: 191.9 KB (191875 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2e93798e494890a0971c68571672f6eab64313bc352b38d311b2f8d30fbe511f`  
		Last Modified: Sat, 16 Dec 2023 10:50:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bd8cb414bcdb6faf94408bf9af63bede825babb42317d1b0e11849f3ebec2a2c`  
		Last Modified: Sat, 16 Dec 2023 10:50:31 GMT  
		Size: 109.2 KB (109250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:8.11.2` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:790df170b272ecbb8671a9faf48efb7b95cfb7cdc4f8a541db03d3c58bd77b8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2376840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd4f47bb3ff90d649537597f66cad1cab62d75507d06633a02b497f82cce140`

```dockerfile
```

-	Layers:
	-	`sha256:1b2ea3c736caad1cf8d2827789f890bc553a7a93edad37cf8d346bacbb0071ad`  
		Last Modified: Sat, 16 Dec 2023 10:50:29 GMT  
		Size: 2.3 MB (2339082 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bad4463453006c62811eb4121ad73918fbcd3980b183d43ad957634f9314c487`  
		Last Modified: Sat, 16 Dec 2023 10:50:29 GMT  
		Size: 37.8 KB (37758 bytes)  
		MIME: application/vnd.in-toto+json

### `elasticsearch:8.11.2` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:e1fd628a70d52683ee032f2d72948a1d28d16a7772ac533a60422e7a1d28f389
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.5 MB (456537204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4596f0d2accf7be6471f0ca46abbfd31df63317435310d5f0638efa50c11fad`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

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
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 07 Dec 2023 12:34:16 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 07 Dec 2023 12:34:16 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Dec 2023 12:34:16 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.label-schema.build-date=2023-12-05T10:03:47.729926671Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=76013fa76dcbf144c886990c6290715f5dc2ae20 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.11.2 org.opencontainers.image.created=2023-12-05T10:03:47.729926671Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=76013fa76dcbf144c886990c6290715f5dc2ae20 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.2
# Thu, 07 Dec 2023 12:34:16 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 07 Dec 2023 12:34:16 GMT
CMD ["eswrapper"]
# Thu, 07 Dec 2023 12:34:16 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1fad6d5c5cc520ad13dbf6a0fad6c68e44f414404e8f7cce759a1533656103b3`  
		Last Modified: Tue, 12 Dec 2023 17:48:11 GMT  
		Size: 13.1 MB (13103527 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c6c2b9825c789c2462f62696c0513cfc91e1df500b5ea96ee546250047bb6068`  
		Last Modified: Tue, 12 Dec 2023 17:48:10 GMT  
		Size: 4.3 KB (4317 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bb9e590e913bcc5f376cecfb8c678bfd9233dc66897a75087a7354bfdfb90a4b`  
		Last Modified: Thu, 14 Dec 2023 19:32:00 GMT  
		Size: 417.1 MB (417147432 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d75909748fece91d574f65e5a1b43c6c266b0e1f869aef2963fe7ecbe981ba2`  
		Last Modified: Thu, 14 Dec 2023 19:31:49 GMT  
		Size: 9.1 KB (9101 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6141f47b5431387ffe9b52c941538a02db70aad70868f3223e9a1f18732d6334`  
		Last Modified: Thu, 14 Dec 2023 19:31:50 GMT  
		Size: 1.7 KB (1721 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0c33057cf2ae8d7550d1db0d0a489d7755da1e2b5191af7ba01960af73a48a0`  
		Last Modified: Thu, 14 Dec 2023 19:31:50 GMT  
		Size: 185.9 KB (185903 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44aa5f504a8211bcbdcb3eceac3bd3ecfdcb05f2057b91affc82dac5c23745d0`  
		Last Modified: Thu, 14 Dec 2023 19:31:51 GMT  
		Size: 407.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0cc7808036e8e94c79c132dd51e0dedc1b45783e5776f376b0185af9555097e9`  
		Last Modified: Thu, 14 Dec 2023 19:31:51 GMT  
		Size: 109.3 KB (109257 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:8.11.2` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:539b48fafdb8027f2214eee6c3c726f001692ba127001bdde7f0a2aae2bdc637
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2377015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9c803a4109fa9bbff9c0e49406c3a42c641d33ab34231f9d4ef078a9556216`

```dockerfile
```

-	Layers:
	-	`sha256:dbdba262a4b7cd0f1a281d4fdbf0f36062af03fca3f27bc119fdbabe55cae08b`  
		Last Modified: Thu, 14 Dec 2023 19:31:50 GMT  
		Size: 2.3 MB (2339405 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:03d237023e1363c8d5ac5c1540eb9631b2b5149afc5bbb79724e2923851ee1fd`  
		Last Modified: Thu, 14 Dec 2023 19:31:49 GMT  
		Size: 37.6 KB (37610 bytes)  
		MIME: application/vnd.in-toto+json

## `elasticsearch:8.11.3`

```console
$ docker pull elasticsearch@sha256:892ec1ae812d582c232e15e6889ca2f419a5126b3d94e428a0fe788808aa292d
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `elasticsearch:8.11.3` - linux; amd64

```console
$ docker pull elasticsearch@sha256:0e47a784b266b7f30d8071a25f774b10a38f3bb9bb41e23a2767ba464aafcb21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **673.3 MB (673285089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac1eef4151323a027507b73e0536f971b5a2181f3c0e77b37b335c84e37c1340`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 12 Dec 2023 13:07:20 GMT
ARG RELEASE
# Tue, 12 Dec 2023 13:07:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 12 Dec 2023 13:07:20 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Tue, 12 Dec 2023 13:07:20 GMT
CMD ["/bin/bash"]
# Tue, 12 Dec 2023 13:07:20 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 13:07:20 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 12 Dec 2023 13:07:20 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY /bin/tini /bin/tini # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 13:07:20 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.label-schema.build-date=2023-12-08T11:33:53.634979452Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=64cf052f3b56b1fd4449f5454cb88aca7e739d9a org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.11.3 org.opencontainers.image.created=2023-12-08T11:33:53.634979452Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=64cf052f3b56b1fd4449f5454cb88aca7e739d9a org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.3
# Tue, 12 Dec 2023 13:07:20 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 12 Dec 2023 13:07:20 GMT
CMD ["eswrapper"]
# Tue, 12 Dec 2023 13:07:20 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:527f5363b98e562da03d2e0bbf86fd7c34f487bffd9b27a3cf0a9afea2f0ee1f`  
		Last Modified: Wed, 13 Dec 2023 10:48:59 GMT  
		Size: 27.5 MB (27512774 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88b906db9c15d2c19cbad2233f11145f77d05494442b029fbb62d21c7a17ad1`  
		Last Modified: Sat, 16 Dec 2023 10:50:33 GMT  
		Size: 7.5 MB (7507922 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:02840f0dd2d9ceb41fa735b73717dd0f7d312194d56a2f3e99d49f8e666336a7`  
		Last Modified: Sat, 16 Dec 2023 10:50:33 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d36bf0362a7bdf86ca6ac3913102fe7d18545adbdf3396fb36630a83ada3cc1f`  
		Last Modified: Sat, 16 Dec 2023 10:50:44 GMT  
		Size: 637.9 MB (637947273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7cfad007f0aceab44ae4666c1f29057e4236068fb3c1d1ffded6e06943c9e8bf`  
		Last Modified: Sat, 16 Dec 2023 10:50:33 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bcb210dd3ca5dc1d2a3857f12ca89154853b676442284131db2777c7a265cd2`  
		Last Modified: Sat, 16 Dec 2023 10:50:34 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1bae0d7353fa7ad39a03e97c711bee6887fefd83adabbf268eae420eaaff13a`  
		Last Modified: Sat, 16 Dec 2023 10:50:34 GMT  
		Size: 191.9 KB (191877 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2aa937b89ef3ee82ce67b4d85be7fa6ce4fcdb9624ee855add8a84d6c0b1f374`  
		Last Modified: Sat, 16 Dec 2023 10:50:34 GMT  
		Size: 402.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7132da5d7ea559eb1228766a02223dfe2df191fe6a0d4cf70547c2e6a5c76a14`  
		Last Modified: Sat, 16 Dec 2023 10:50:35 GMT  
		Size: 109.2 KB (109244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:8.11.3` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:42dd20e51b3a7472d4ad1ce3b60b1b7430dc28db4ef03f59913a65401f442432
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2376856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97cf2acf6ca8c0bdc1c9740b9975e73217ee98de0014dadbe2b330382a190faf`

```dockerfile
```

-	Layers:
	-	`sha256:157f68bbcfb0e3689702ecea161c39617ea1ad353cbef195dc61d3faf06ae866`  
		Last Modified: Sat, 16 Dec 2023 10:50:33 GMT  
		Size: 2.3 MB (2339098 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d1170dd9f7df6540aefc6c9f0ff475c564ffb9e4154021ae1f6fabb4fdb9d9c`  
		Last Modified: Sat, 16 Dec 2023 10:50:33 GMT  
		Size: 37.8 KB (37758 bytes)  
		MIME: application/vnd.in-toto+json

### `elasticsearch:8.11.3` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:44398545f17b295cb016e0c50dc12efb538eab67e87fdbc2499cc0448200c480
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.5 MB (456542578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92866351f1d21ad06cbcd8cef0251a644efbb68e4eb0c9f56f7a7b40c639628f`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

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
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 13:07:20 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 12 Dec 2023 13:07:20 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY /bin/tini /bin/tini # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 13:07:20 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.label-schema.build-date=2023-12-08T11:33:53.634979452Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=64cf052f3b56b1fd4449f5454cb88aca7e739d9a org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.11.3 org.opencontainers.image.created=2023-12-08T11:33:53.634979452Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=64cf052f3b56b1fd4449f5454cb88aca7e739d9a org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.3
# Tue, 12 Dec 2023 13:07:20 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 12 Dec 2023 13:07:20 GMT
CMD ["eswrapper"]
# Tue, 12 Dec 2023 13:07:20 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1fad6d5c5cc520ad13dbf6a0fad6c68e44f414404e8f7cce759a1533656103b3`  
		Last Modified: Tue, 12 Dec 2023 17:48:11 GMT  
		Size: 13.1 MB (13103527 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c6c2b9825c789c2462f62696c0513cfc91e1df500b5ea96ee546250047bb6068`  
		Last Modified: Tue, 12 Dec 2023 17:48:10 GMT  
		Size: 4.3 KB (4317 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:715eb0de7bac9b6d554a5e26bfafdf2afa5f1449be13bd98cfd8eb8b27e539d5`  
		Last Modified: Thu, 14 Dec 2023 19:23:06 GMT  
		Size: 417.2 MB (417152807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b996c48e81a2bb33206f1ef942d24aa751f2d680ab2f60382ea5093b2af34a3`  
		Last Modified: Thu, 14 Dec 2023 19:22:57 GMT  
		Size: 9.1 KB (9100 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f0edcba450a381bed3774b133f94cd449b405eaf58a3151f01ff1634849a66f`  
		Last Modified: Thu, 14 Dec 2023 19:22:57 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cd5fcee8a7e50961b8a4e4c800e58543768b3bccb7f706636810e638b658b9c`  
		Last Modified: Thu, 14 Dec 2023 19:22:57 GMT  
		Size: 185.9 KB (185904 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97ad3ae845f052b8d52f6c6a61dfc48185e84ea0f5abbe2552e9a10ec8c8af8e`  
		Last Modified: Thu, 14 Dec 2023 19:22:58 GMT  
		Size: 408.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4fd48697c3d9a794bd555ab5f5f263654225c981a8eea063af5ce75c3db85c0b`  
		Last Modified: Thu, 14 Dec 2023 19:22:58 GMT  
		Size: 109.3 KB (109254 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:8.11.3` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:187d5e81002c71e7a9134c6173fed78b42d1744f89202215f0d756199946ac9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2377015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:789a22aaffe1ca9d0f094f4f8378b7b97572b28e198027a1fbf166eb2420fc19`

```dockerfile
```

-	Layers:
	-	`sha256:b1b2a0d17147ac7109d5fbd5fb466311422690ab34daa880fec08fcb12f02718`  
		Last Modified: Thu, 14 Dec 2023 19:22:57 GMT  
		Size: 2.3 MB (2339405 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d33af2d1bdea4795e5c5c7291e68b6e0a340ceb03b6d233d6fd0693965372781`  
		Last Modified: Thu, 14 Dec 2023 19:22:57 GMT  
		Size: 37.6 KB (37610 bytes)  
		MIME: application/vnd.in-toto+json
