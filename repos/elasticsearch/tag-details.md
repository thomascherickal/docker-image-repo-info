<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.12`](#elasticsearch6812)
-	[`elasticsearch:7.9.1`](#elasticsearch791)

## `elasticsearch:6.8.12`

```console
$ docker pull elasticsearch@sha256:318c18bb5b233e79a7f4819ab1de013215d4eb570749d7622c24afdfee84c041
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `elasticsearch:6.8.12` - linux; amd64

```console
$ docker pull elasticsearch@sha256:35c171d04fc54990e61f94ba0bf64655661c4fc9be0db3fa5512d3bac5173626
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **445.1 MB (445104327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd8e25fc357c8b372d3b6f57cc6c82ba13e1d0718a9c2932204c73405d2ddd31`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Wed, 12 Aug 2020 07:33:49 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 12 Aug 2020 07:33:50 GMT
ENV JAVA_HOME=/opt/jdk-14.0.1+7
# Wed, 12 Aug 2020 07:33:57 GMT
COPY dir:1f33bb8a41e8c55f30a27315a6c01178c489337e8e8baee8147ab3a9d9662fcb in /opt/jdk-14.0.1+7 
# Wed, 12 Aug 2020 07:34:20 GMT
RUN for iter in {1..10}; do yum update  --setopt=tsflags=nodocs -y &&     yum install -y  --setopt=tsflags=nodocs nc unzip wget which &&     yum clean all && exit_code=0 && break || exit_code=\$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Wed, 12 Aug 2020 07:34:22 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Wed, 12 Aug 2020 07:34:22 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 12 Aug 2020 07:34:26 GMT
COPY --chown=1000:0dir:43503c83ccfb3cd853ef136c63c26a601b26a8f5de5239d5c47c24eca36c9467 in /usr/share/elasticsearch 
# Wed, 12 Aug 2020 07:34:27 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 07:34:27 GMT
COPY --chown=1000:0file:08193f849fc25f29db1438eff6d5c9fe1d63237aeb07a3e0009e8ba554f97c31 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 12 Aug 2020 07:34:29 GMT
RUN chgrp 0 /usr/local/bin/docker-entrypoint.sh &&     chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Wed, 12 Aug 2020 07:34:29 GMT
EXPOSE 9200 9300
# Wed, 12 Aug 2020 07:34:29 GMT
LABEL org.label-schema.build-date=2020-08-12T07:27:20.804867Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=7a15d2a169913a2d6116dcc081bc592fbf8d9b1c org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=6.8.12 org.opencontainers.image.created=2020-08-12T07:27:20.804867Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=7a15d2a169913a2d6116dcc081bc592fbf8d9b1c org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=6.8.12
# Wed, 12 Aug 2020 07:34:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 12 Aug 2020 07:34:29 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d80c7326d2a5fed590b129882bc569ed5915afce119a5c42e9d9f4f82a918`  
		Last Modified: Tue, 18 Aug 2020 20:41:23 GMT  
		Size: 211.9 MB (211934763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b061ab1ef7fde0c29b329a7a9ae3ddae1ffee16e73643b5fa775a23162d9c54`  
		Last Modified: Tue, 18 Aug 2020 20:41:06 GMT  
		Size: 7.2 MB (7197543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feea456553d8854c6a98dd602c53289d59c2b5e4fe92025c68909aac3704d0b9`  
		Last Modified: Tue, 18 Aug 2020 20:41:02 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79eafa2f0b0b9792f217d33e92fe5dde6c0006d0fb61c83cdfb85572736e55b9`  
		Last Modified: Tue, 18 Aug 2020 20:41:21 GMT  
		Size: 150.1 MB (150102099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b66cf42d5c18c3d3ba3641febef562a44fcf5ff0da69b0096aba16dc31f3f5`  
		Last Modified: Tue, 18 Aug 2020 20:41:02 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f76a960056a5c3fcbf34a7adca2dfbbcd3bcfd63ee139d24749f99c3f745ab`  
		Last Modified: Tue, 18 Aug 2020 20:41:02 GMT  
		Size: 2.4 KB (2400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:7.9.1`

```console
$ docker pull elasticsearch@sha256:a208e0ba7646155d1581bb979f3b300c02cf3a4e871e92ce22a30dd5215c73c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.9.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:1fdbaa46df0e39c4a29412092e7c4ea0754b3c18071e2d30fd866b975d8124ab
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.5 MB (404533759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22008d6d4b2d2aa2d3c79da05a9e6bf98494c505e40919a913278a9e58deebd2`
-	Entrypoint: `["\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Tue, 01 Sep 2020 21:26:30 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 01 Sep 2020 21:26:30 GMT
COPY file:df9158ae8b9b283e8ea5bd72d1e344c08dea733e283f9f0941833f467466323c in /tini 
# Tue, 01 Sep 2020 21:26:48 GMT
RUN for iter in {1..10}; do yum update --setopt=tsflags=nodocs -y &&     yum install --setopt=tsflags=nodocs -y nc shadow-utils zip unzip &&     yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Tue, 01 Sep 2020 21:26:51 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Tue, 01 Sep 2020 21:26:51 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 01 Sep 2020 21:27:13 GMT
COPY --chown=1000:0dir:8031ea9e5da42c4f0d33bf9c91dc33bd5bf17f2836821516848268e0bd971c54 in /usr/share/elasticsearch 
# Tue, 01 Sep 2020 21:27:19 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /usr/share/elasticsearch/jdk/lib/security/cacerts
# Tue, 01 Sep 2020 21:27:19 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Sep 2020 21:27:19 GMT
COPY file:d964df1452418918baf1d29ee20df18c9648ca6c9d51764640fca470bd9a9366 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Sep 2020 21:27:21 GMT
RUN chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Tue, 01 Sep 2020 21:27:23 GMT
RUN find / -xdev -perm -4000 -exec chmod ug-s {} +
# Tue, 01 Sep 2020 21:27:23 GMT
EXPOSE 9200 9300
# Tue, 01 Sep 2020 21:27:23 GMT
LABEL org.label-schema.build-date=2020-09-01T21:22:21.964974Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=083627f112ba94dffc1232e8b42b73492789ef91 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.9.1 org.opencontainers.image.created=2020-09-01T21:22:21.964974Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=083627f112ba94dffc1232e8b42b73492789ef91 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.9.1
# Tue, 01 Sep 2020 21:27:24 GMT
ENTRYPOINT ["/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 01 Sep 2020 21:27:24 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbb6a67f8b37241666e9f3b5de5f1972f070bbd7df637fc84401c52489fd9cb`  
		Last Modified: Thu, 03 Sep 2020 16:34:33 GMT  
		Size: 9.5 KB (9461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6bdc20ad4f68ed4e2c9fe83678ef374d9fe0be205bb7bb8f85f128d8d93945`  
		Last Modified: Thu, 03 Sep 2020 16:34:33 GMT  
		Size: 7.2 MB (7239414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94336c7d5fd543fbc393ecaf8e4d45d03a1ef2afb133503185a1448a6f19d7e`  
		Last Modified: Thu, 03 Sep 2020 16:34:31 GMT  
		Size: 2.3 KB (2283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdbe26fe92d22ad5604fafd44d3272fdeaaa0236aa9e80318db4265465572c6`  
		Last Modified: Thu, 03 Sep 2020 16:34:59 GMT  
		Size: 321.2 MB (321214733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e2d4a5b7b3b5a460cea3f46c4caf09e9400a21179c9cb54619e2b919d50c31`  
		Last Modified: Thu, 03 Sep 2020 16:34:31 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14dbd0b22f9ea5d326d2f2fab45ab9a1bb6e1f256efbdd7c038962fdc23149`  
		Last Modified: Thu, 03 Sep 2020 16:34:30 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24602d8548c0619d813b2c2731013a667446bb1bfbbf058920a1ada31b73fe2`  
		Last Modified: Thu, 03 Sep 2020 16:34:30 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797b5c9616a7e76b8012830206a318c739e4a521a9ad6185df8a6926ef8225ac`  
		Last Modified: Thu, 03 Sep 2020 16:34:29 GMT  
		Size: 200.6 KB (200611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.9.1` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:91fd5a8aad934ab2e3737435c7ca9ef8648896e94d8fad071c44a4672a8316e3
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.8 MB (432807279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:081b36016585b268036519278b3663e7a8da9bdf6e94be2b30aeaf72bd7b9171`
-	Entrypoint: `["\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Wed, 02 Sep 2020 00:53:14 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 02 Sep 2020 00:53:15 GMT
COPY file:71bfd2daffa1277e243209a08921f2609e22adbf82217ed08c071eb3a2ddca8a in /tini 
# Wed, 02 Sep 2020 00:53:20 GMT
RUN for iter in {1..10}; do yum update --setopt=tsflags=nodocs -y &&     yum install --setopt=tsflags=nodocs -y nc shadow-utils zip unzip &&     yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Wed, 02 Sep 2020 00:53:20 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Wed, 02 Sep 2020 00:53:20 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 02 Sep 2020 00:53:23 GMT
COPY --chown=1000:0dir:c1fa01879a80a3c89cbbec1166f928a625aaa8d64d99e51b8e7e4fcdd3faf172 in /usr/share/elasticsearch 
# Wed, 02 Sep 2020 00:53:27 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /usr/share/elasticsearch/jdk/lib/security/cacerts
# Wed, 02 Sep 2020 00:53:27 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Sep 2020 00:53:27 GMT
COPY file:d964df1452418918baf1d29ee20df18c9648ca6c9d51764640fca470bd9a9366 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 02 Sep 2020 00:53:27 GMT
RUN chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Wed, 02 Sep 2020 00:53:28 GMT
RUN find / -xdev -perm -4000 -exec chmod ug-s {} +
# Wed, 02 Sep 2020 00:53:28 GMT
EXPOSE 9200 9300
# Wed, 02 Sep 2020 00:53:28 GMT
LABEL org.label-schema.build-date=2020-09-02T00:51:06.079882Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=083627f112ba94dffc1232e8b42b73492789ef91 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.9.1 org.opencontainers.image.created=2020-09-02T00:51:06.079882Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=083627f112ba94dffc1232e8b42b73492789ef91 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.9.1
# Wed, 02 Sep 2020 00:53:28 GMT
ENTRYPOINT ["/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 02 Sep 2020 00:53:28 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78db0c7b4f3de39bf09ec7ae267343731d5c6caa93c0439682123e7be188d0d`  
		Last Modified: Fri, 04 Sep 2020 20:48:40 GMT  
		Size: 9.0 KB (9037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1c1ab098a17331aa3a81095368fa364b786d76b8333af0034df9e0dbff4c11`  
		Last Modified: Fri, 04 Sep 2020 20:48:43 GMT  
		Size: 7.0 MB (6977538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe014ebeb0c28f7c37c2c6ab817dcef2eecf0b20c6467fa1310c3bea796ffd0`  
		Last Modified: Fri, 04 Sep 2020 20:48:40 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812e724e5b37032aeba929c01ddecae553127b53b01c34a060b576990833bd5d`  
		Last Modified: Fri, 04 Sep 2020 20:49:25 GMT  
		Size: 318.3 MB (318271973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f68b74a338eb1d209cb9ed4a927ee210537696804607807321d14d32846acd5`  
		Last Modified: Fri, 04 Sep 2020 20:48:38 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8ee1a50dcb243f1872f5cf629f482ec516106c971983a936381eb5abebb6c9`  
		Last Modified: Fri, 04 Sep 2020 20:48:38 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28dfc08224d72961629842c0e5e1728eb31aa421a8b27696d917440fc8bebee`  
		Last Modified: Fri, 04 Sep 2020 20:48:38 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f684a7d0b84e6e1f8cc33da2657c68c0455f1b5cdedad480178ae2bd0e63629`  
		Last Modified: Fri, 04 Sep 2020 20:48:38 GMT  
		Size: 211.0 KB (211029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
