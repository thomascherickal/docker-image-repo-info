<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.15`](#elasticsearch71715)
-	[`elasticsearch:8.11.1`](#elasticsearch8111)

## `elasticsearch:7.17.15`

```console
$ docker pull elasticsearch@sha256:88c2ec10c7f2e5e424961d5b0bbfbcf1c2642e55bfd8118e7fb745e8b952c479
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `elasticsearch:7.17.15` - linux; amd64

```console
$ docker pull elasticsearch@sha256:6796c8b715952bf10bf70511c39f2b83bd40a60f3503bedb5bb71b2bf53eedcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.6 MB (366619610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b7216db00ae4415d861df1e01888823c624ae9b1cb5571719106c855c527a7f`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 13 Nov 2023 18:15:06 GMT
ARG RELEASE
# Mon, 13 Nov 2023 18:15:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 13 Nov 2023 18:15:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 13 Nov 2023 18:15:06 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 13 Nov 2023 18:15:06 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Mon, 13 Nov 2023 18:15:06 GMT
CMD ["/bin/bash"]
# Mon, 13 Nov 2023 18:15:06 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 13 Nov 2023 18:15:06 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 13 Nov 2023 18:15:06 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
COPY /bin/tini /bin/tini # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Nov 2023 18:15:06 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Mon, 13 Nov 2023 18:15:06 GMT
LABEL org.label-schema.build-date=2023-11-10T22:03:46.987399016Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=0b8ecfb4378335f4689c4223d1f1115f16bef3ba org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.15 org.opencontainers.image.created=2023-11-10T22:03:46.987399016Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=0b8ecfb4378335f4689c4223d1f1115f16bef3ba org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.15
# Mon, 13 Nov 2023 18:15:06 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 13 Nov 2023 18:15:06 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ffed5cb6c25b8a10866c1c2be758fdcae381a37a164664ad2536d807fb620810`  
		Last Modified: Tue, 12 Dec 2023 17:17:10 GMT  
		Size: 14.3 MB (14340675 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:202a9c37447b09b12e090f8e3574c6a442e040bec6ef3db10d0d0bec21c98229`  
		Last Modified: Tue, 12 Dec 2023 17:17:09 GMT  
		Size: 4.3 KB (4320 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0a62dc45853017daf07d9e1ee745ac439b741d8582369155dde5c6e66c57300`  
		Last Modified: Tue, 12 Dec 2023 17:17:16 GMT  
		Size: 324.4 MB (324448709 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b0ba43353171dd80731540a098ec0493a820f68ecec450817f2410dacbf862d`  
		Last Modified: Tue, 12 Dec 2023 17:17:09 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03681169912a060df231c218f18f2324a9eea708055b0f6be322c3f143062f6c`  
		Last Modified: Tue, 12 Dec 2023 17:17:10 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2eb8d6d3918f1fbfa9a9b0afa5717af10b4b0ebee4f688de7e3548e2069192a3`  
		Last Modified: Tue, 12 Dec 2023 17:17:10 GMT  
		Size: 192.1 KB (192148 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d1dac24be607d1d5928928030281653cce0b8b409e949cec67f3a19c9d5a1a1`  
		Last Modified: Tue, 12 Dec 2023 17:17:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f159f913a363f7492b59c7247ade655e8c326e1a1771c59a0325f3fec24dc8b`  
		Last Modified: Tue, 12 Dec 2023 17:17:11 GMT  
		Size: 109.3 KB (109252 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:7.17.15` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:0e39589699ce7d647e28177e1d5f6a98349002ca92edd75f1d2785011f7f6bb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2107526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928c566eef0397a2e0ae650b963ff6fc43d0795207b24652cbadd86899269bcc`

```dockerfile
```

-	Layers:
	-	`sha256:90de16405ceb8fd39c076b8b56d3246ebf1d59f6cc617b25e4bc57b479f76b38`  
		Last Modified: Tue, 12 Dec 2023 17:17:09 GMT  
		Size: 2.1 MB (2069775 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7985a79e493a045c67e25d5e8709d5126864530d6a92bbd33cbc8abccf6ff6df`  
		Last Modified: Tue, 12 Dec 2023 17:17:09 GMT  
		Size: 37.8 KB (37751 bytes)  
		MIME: application/vnd.in-toto+json

### `elasticsearch:7.17.15` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:852dfc498d281430e1f072c12e2f42aab302d0707170bc430693cd3329f03f98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.8 MB (361780725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6990ab92ba71e6ca82912d0446e0194df38b7f16874a3e7d44ba4f919a5156c9`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 13 Nov 2023 18:15:06 GMT
ARG RELEASE
# Mon, 13 Nov 2023 18:15:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 13 Nov 2023 18:15:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 13 Nov 2023 18:15:06 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 13 Nov 2023 18:15:06 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Mon, 13 Nov 2023 18:15:06 GMT
CMD ["/bin/bash"]
# Mon, 13 Nov 2023 18:15:06 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 13 Nov 2023 18:15:06 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 13 Nov 2023 18:15:06 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
COPY /bin/tini /bin/tini # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Nov 2023 18:15:06 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Nov 2023 18:15:06 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Mon, 13 Nov 2023 18:15:06 GMT
LABEL org.label-schema.build-date=2023-11-10T22:03:46.987399016Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=0b8ecfb4378335f4689c4223d1f1115f16bef3ba org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.15 org.opencontainers.image.created=2023-11-10T22:03:46.987399016Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=0b8ecfb4378335f4689c4223d1f1115f16bef3ba org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.15
# Mon, 13 Nov 2023 18:15:06 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 13 Nov 2023 18:15:06 GMT
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
	-	`sha256:37f2ebdac805f4a73bf3b675d364d74ea8eb9fad5588d88e5bfd9565d402dc78`  
		Last Modified: Tue, 12 Dec 2023 17:49:50 GMT  
		Size: 322.4 MB (322390431 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8fa84f0ec0c4ff0f1efba4eb5a64b5c6d911190516ddca4979189c0c1a0fda0`  
		Last Modified: Tue, 12 Dec 2023 17:49:40 GMT  
		Size: 9.1 KB (9097 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b609a097f87bc734454b4d2d49e9b14861469f8fb7cb9c9c3975347f0f296338`  
		Last Modified: Tue, 12 Dec 2023 17:49:40 GMT  
		Size: 2.0 KB (1980 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d599759046f7ee4e5c43f167593379919761a99358a80b106eb875d05773febf`  
		Last Modified: Tue, 12 Dec 2023 17:49:41 GMT  
		Size: 186.2 KB (186165 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:240b9709cf8ebff1799a9e9ef393f5d00593d4540f9b200a8c278ccc70a05962`  
		Last Modified: Tue, 12 Dec 2023 17:49:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:278ded290f465119a2aaf7718e5ce23bddadee387cb0a47a9fe651fc076a4f50`  
		Last Modified: Tue, 12 Dec 2023 17:49:42 GMT  
		Size: 109.2 KB (109249 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:7.17.15` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:410a2cab1ea9974aa1506bc3f9b69f376a3ff3a9f549e399832d67cfff986f51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2107853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20715b75dde257e9be3dc8b3f0f86cd38baa45565212021a6fe62eca843f2eec`

```dockerfile
```

-	Layers:
	-	`sha256:535784cb863566799c55f6d9d7c6d286eed6fa20b3ed9b479661241654c50c10`  
		Last Modified: Tue, 12 Dec 2023 17:49:40 GMT  
		Size: 2.1 MB (2070098 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:26c4cbc931efc9f153c4ccb10f256a9084ac0d4d84854143bb96f22a74c66f68`  
		Last Modified: Tue, 12 Dec 2023 17:49:39 GMT  
		Size: 37.8 KB (37755 bytes)  
		MIME: application/vnd.in-toto+json

## `elasticsearch:8.11.1`

```console
$ docker pull elasticsearch@sha256:e9b31098201dc40200d7c445f328845d77e9cbb4fe0b38219d989462a9a4280a
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `elasticsearch:8.11.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:adf8680ac410dabaa684bcad22000f0b1dcc85d12cecb7e5bbdd60a496265f77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **680.0 MB (680044102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be606e19dd0f3d8aa0d2adbac6945673f900c31de8dfbbd023a23e54e6a63027`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 13 Nov 2023 14:50:42 GMT
ARG RELEASE
# Mon, 13 Nov 2023 14:50:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 13 Nov 2023 14:50:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 13 Nov 2023 14:50:42 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 13 Nov 2023 14:50:42 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Mon, 13 Nov 2023 14:50:42 GMT
CMD ["/bin/bash"]
# Mon, 13 Nov 2023 14:50:42 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 13 Nov 2023 14:50:42 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 13 Nov 2023 14:50:42 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
COPY /bin/tini /bin/tini # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Nov 2023 14:50:42 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Mon, 13 Nov 2023 14:50:42 GMT
LABEL org.label-schema.build-date=2023-11-11T10:05:59.421038163Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=6f9ff581fbcde658e6f69d6ce03050f060d1fd0c org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.11.1 org.opencontainers.image.created=2023-11-11T10:05:59.421038163Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=6f9ff581fbcde658e6f69d6ce03050f060d1fd0c org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.1
# Mon, 13 Nov 2023 14:50:42 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 13 Nov 2023 14:50:42 GMT
CMD ["eswrapper"]
# Mon, 13 Nov 2023 14:50:42 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:461781d10ee371ad08bdb1eaacc28f982a5611834bae0e6347ee056d0f177b3d`  
		Last Modified: Tue, 12 Dec 2023 17:17:59 GMT  
		Size: 14.3 MB (14340651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e2d8f55faded51bab77b4b9d35b947c186895ad41519c7c8746012cc6298856`  
		Last Modified: Tue, 12 Dec 2023 17:17:58 GMT  
		Size: 4.3 KB (4313 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16e03ab6800c0ff22482bb7639d4d41d98d090841929cd972a4561beeb3ef952`  
		Last Modified: Tue, 12 Dec 2023 17:18:15 GMT  
		Size: 637.9 MB (637873752 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29310f9f80597a7a32df27157facc76cfb379caed0ce7fc6d70be8922f5b3444`  
		Last Modified: Tue, 12 Dec 2023 17:17:58 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:642b4bb113473131349d4132d271d274ed6925edcb99d8dcbcabc27500a8e0cb`  
		Last Modified: Tue, 12 Dec 2023 17:17:59 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:24fec4b7d388c3fdbf50707cb65b8e08c7171ea04885ec697e23d02c1f70ce08`  
		Last Modified: Tue, 12 Dec 2023 17:17:59 GMT  
		Size: 191.9 KB (191882 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d59f72ec50c2a878e00263ad13c9ed7545e81b66367703403dbb7236f61e88e4`  
		Last Modified: Tue, 12 Dec 2023 17:18:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:891545c1073423f974f9f8c1a8e6ec54334fa0e01089ae5168c3ff616bc9bcb8`  
		Last Modified: Tue, 12 Dec 2023 17:18:00 GMT  
		Size: 109.3 KB (109253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:8.11.1` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:a7a915f8e9aeb2ca91555459fd24d9aa2b47df902c6ac5d9455ccaa40c2a6cf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2376857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5adec7037929e1df778b9b66ec86c2f15d904ea25e3cadfb65c2b210a6f0b62`

```dockerfile
```

-	Layers:
	-	`sha256:59b60eed989a1b02258cc9b95f37a698a4a2cb356952e80bff7f72321b39a1f0`  
		Last Modified: Tue, 12 Dec 2023 17:17:58 GMT  
		Size: 2.3 MB (2339090 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:26430b7da58358c96a95933010f62f350700265bd4d8317215de64d06a732a61`  
		Last Modified: Tue, 12 Dec 2023 17:17:57 GMT  
		Size: 37.8 KB (37767 bytes)  
		MIME: application/vnd.in-toto+json

### `elasticsearch:8.11.1` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:fda9a134237a3046b86175d174957a8507df8aafd4c2fb8f13a79dedc590e391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.5 MB (456470318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8567b8c5461b69c3de2eef37ab3415d11b647c10852d85690eedb2326a2102f6`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 13 Nov 2023 14:50:42 GMT
ARG RELEASE
# Mon, 13 Nov 2023 14:50:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 13 Nov 2023 14:50:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 13 Nov 2023 14:50:42 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 13 Nov 2023 14:50:42 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Mon, 13 Nov 2023 14:50:42 GMT
CMD ["/bin/bash"]
# Mon, 13 Nov 2023 14:50:42 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 13 Nov 2023 14:50:42 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 13 Nov 2023 14:50:42 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
COPY /bin/tini /bin/tini # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Nov 2023 14:50:42 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Nov 2023 14:50:42 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Mon, 13 Nov 2023 14:50:42 GMT
LABEL org.label-schema.build-date=2023-11-11T10:05:59.421038163Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=6f9ff581fbcde658e6f69d6ce03050f060d1fd0c org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.11.1 org.opencontainers.image.created=2023-11-11T10:05:59.421038163Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=6f9ff581fbcde658e6f69d6ce03050f060d1fd0c org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.1
# Mon, 13 Nov 2023 14:50:42 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 13 Nov 2023 14:50:42 GMT
CMD ["eswrapper"]
# Mon, 13 Nov 2023 14:50:42 GMT
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
	-	`sha256:e85f5c721eecec59207508a68d3ebd2c00165f18f6557dbfa688c9d36f6783c3`  
		Last Modified: Tue, 12 Dec 2023 17:48:20 GMT  
		Size: 417.1 MB (417080564 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:971bb68f0cb780bf0d27b29a3e17bc277497958a1d92c8eecc79fc5d74c4bcad`  
		Last Modified: Tue, 12 Dec 2023 17:48:11 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ced0226ec7912743afc4adb9ebab502cbd4e4af19f33a94fb38f25d68caa544`  
		Last Modified: Tue, 12 Dec 2023 17:48:12 GMT  
		Size: 1.7 KB (1720 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfd59b7fe418ca242c3b3263a54f2562de1b9090b6ed7c14e1742418a5be78a8`  
		Last Modified: Tue, 12 Dec 2023 17:48:12 GMT  
		Size: 185.9 KB (185899 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d274764d37e25ab436d885f748800bd07e649ed7ec5b8957738c82af3ff984dd`  
		Last Modified: Tue, 12 Dec 2023 17:48:13 GMT  
		Size: 404.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ec5856c55eb13f3d1332cc316cc4d9b4a24b351a8ce07f9a7fd07d919123f26`  
		Last Modified: Tue, 12 Dec 2023 17:48:14 GMT  
		Size: 109.3 KB (109252 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:8.11.1` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:72f267cc5ee1c111d72062e06e99620425736276e6627b9c36b7ddd4c88fa27d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2377031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:478cb0c231969b6d9ca807d6b1d6cc845d0f32f8f97a4a71c6d3ba1cfcd76bdb`

```dockerfile
```

-	Layers:
	-	`sha256:8d168c9b8881a934c3d411de0eca43a42ef8c2bfc2d4af12345c1b4eb8adb5e2`  
		Last Modified: Tue, 12 Dec 2023 17:48:11 GMT  
		Size: 2.3 MB (2339421 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:992da7735e05885ed394d871800a3da119d1cc48fc6442af5fd8d0fc0e3fbe9a`  
		Last Modified: Tue, 12 Dec 2023 17:48:10 GMT  
		Size: 37.6 KB (37610 bytes)  
		MIME: application/vnd.in-toto+json
