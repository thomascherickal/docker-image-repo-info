<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.12`](#elasticsearch6812)
-	[`elasticsearch:7.9.2`](#elasticsearch792)

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

## `elasticsearch:7.9.2`

```console
$ docker pull elasticsearch@sha256:e3b52403c6fb95eb4dc6092d39c187acfc38e8afd61e4d38801ae323b3eeeff3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.9.2` - linux; amd64

```console
$ docker pull elasticsearch@sha256:337369f2403be78fcad2e69d3f56681cd1b7a4aa8539ed599806da83cf0f10ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.2 MB (402205568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caa7a21ca06ea2376dc2a2b3194795def7bed7cc1a4de18feee0a706518d2c39`
-	Entrypoint: `["\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Wed, 23 Sep 2020 00:50:08 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 23 Sep 2020 00:50:08 GMT
COPY file:df9158ae8b9b283e8ea5bd72d1e344c08dea733e283f9f0941833f467466323c in /tini 
# Wed, 23 Sep 2020 00:50:26 GMT
RUN for iter in {1..10}; do yum update --setopt=tsflags=nodocs -y &&     yum install --setopt=tsflags=nodocs -y nc shadow-utils zip unzip &&     yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Wed, 23 Sep 2020 00:50:28 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Wed, 23 Sep 2020 00:50:28 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 23 Sep 2020 00:50:50 GMT
COPY --chown=1000:0dir:be8b362934ad1a6c30510c9303449bf9f264d37dc5ca665b764dbb2ddc85c7db in /usr/share/elasticsearch 
# Wed, 23 Sep 2020 00:50:51 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /usr/share/elasticsearch/jdk/lib/security/cacerts
# Wed, 23 Sep 2020 00:50:51 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Sep 2020 00:50:52 GMT
COPY file:d964df1452418918baf1d29ee20df18c9648ca6c9d51764640fca470bd9a9366 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 23 Sep 2020 00:50:53 GMT
RUN chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Wed, 23 Sep 2020 00:50:57 GMT
RUN find / -xdev -perm -4000 -exec chmod ug-s {} +
# Wed, 23 Sep 2020 00:50:58 GMT
EXPOSE 9200 9300
# Wed, 23 Sep 2020 00:50:58 GMT
LABEL org.label-schema.build-date=2020-09-23T00:45:33.626720Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=d34da0ea4a966c4e49417f2da2f244e3e97b4e6e org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.9.2 org.opencontainers.image.created=2020-09-23T00:45:33.626720Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=d34da0ea4a966c4e49417f2da2f244e3e97b4e6e org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.9.2
# Wed, 23 Sep 2020 00:50:58 GMT
ENTRYPOINT ["/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 23 Sep 2020 00:50:59 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a20a45aa507cd2fb8f0a66d464263c0903977c0d9f7aee3480109b81c793d2`  
		Last Modified: Thu, 24 Sep 2020 14:49:18 GMT  
		Size: 9.5 KB (9462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d49bb9ac613fa3e40c1d232777f63185211144006c5153d9729e5c869888b5e`  
		Last Modified: Thu, 24 Sep 2020 14:49:21 GMT  
		Size: 7.2 MB (7239455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dcf7a2301a13fc43f08dc1e8eeed2219a6a082ee754c3c0706dc6353d31f85`  
		Last Modified: Thu, 24 Sep 2020 14:49:16 GMT  
		Size: 2.3 KB (2283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d68d841d2ebf1af19650ae4f259d67ea0d0e2e62930060af67231ce8dec9b9`  
		Last Modified: Thu, 24 Sep 2020 14:50:05 GMT  
		Size: 318.9 MB (318886514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db71e2f6acdde831a7a04569204025d4ceda326fbd8cec91cb2fc3ec6fdaa625`  
		Last Modified: Thu, 24 Sep 2020 14:49:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d58f7bd0cd73548cf11262982a8d8fb7fa6f6f26276bd2f6f799cab6e7fbfd5`  
		Last Modified: Thu, 24 Sep 2020 14:49:15 GMT  
		Size: 1.7 KB (1717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161752ba6659c507fdad1bd65dedecbaf951a8e6be54ed864963cd2d63b584de`  
		Last Modified: Thu, 24 Sep 2020 14:49:15 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adf2f929b9edbb04ff27c10ef4e6524ef3da1be908a2a7ed93d04e1bfe7be95`  
		Last Modified: Thu, 24 Sep 2020 14:49:16 GMT  
		Size: 200.6 KB (200610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.9.2` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:a6adc5f3bcd320be968b8b69f26e3d1e20cc6717f7d5e83bc71c9387e2533577
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.6 MB (430636991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:345ad16b5b160d8ac12f68c9e118ae709533991f32861861e1bf592d76a5ff31`
-	Entrypoint: `["\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Wed, 23 Sep 2020 04:31:55 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 23 Sep 2020 04:31:55 GMT
COPY file:71bfd2daffa1277e243209a08921f2609e22adbf82217ed08c071eb3a2ddca8a in /tini 
# Wed, 23 Sep 2020 04:32:08 GMT
RUN for iter in {1..10}; do yum update --setopt=tsflags=nodocs -y &&     yum install --setopt=tsflags=nodocs -y nc shadow-utils zip unzip &&     yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Wed, 23 Sep 2020 04:32:08 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Wed, 23 Sep 2020 04:32:09 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 23 Sep 2020 04:32:23 GMT
COPY --chown=1000:0dir:1d2d27a0278dd55b87444df52b237010cb69337cabd99d9012e6dd3b05ccb41f in /usr/share/elasticsearch 
# Wed, 23 Sep 2020 04:32:25 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /usr/share/elasticsearch/jdk/lib/security/cacerts
# Wed, 23 Sep 2020 04:32:25 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Sep 2020 04:32:25 GMT
COPY file:d964df1452418918baf1d29ee20df18c9648ca6c9d51764640fca470bd9a9366 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 23 Sep 2020 04:32:26 GMT
RUN chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Wed, 23 Sep 2020 04:32:28 GMT
RUN find / -xdev -perm -4000 -exec chmod ug-s {} +
# Wed, 23 Sep 2020 04:32:28 GMT
EXPOSE 9200 9300
# Wed, 23 Sep 2020 04:32:28 GMT
LABEL org.label-schema.build-date=2020-09-23T04:28:49.179747Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=d34da0ea4a966c4e49417f2da2f244e3e97b4e6e org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.9.2 org.opencontainers.image.created=2020-09-23T04:28:49.179747Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=d34da0ea4a966c4e49417f2da2f244e3e97b4e6e org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.9.2
# Wed, 23 Sep 2020 04:32:28 GMT
ENTRYPOINT ["/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 23 Sep 2020 04:32:28 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400a45e237b032793623a75188da9fe53e24eb127336bd2f5c3fff97ff69fea8`  
		Last Modified: Mon, 28 Sep 2020 22:40:44 GMT  
		Size: 9.0 KB (9037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3333bd92b5b0cf3bd4b7b1aadf8370026c3334db85fc166c60a1f69c1669ba`  
		Last Modified: Mon, 28 Sep 2020 22:40:47 GMT  
		Size: 7.0 MB (6977592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcb044e3dce3a919259711918952ecd15535a687e777978cf803c76b56c4ca3`  
		Last Modified: Mon, 28 Sep 2020 22:40:44 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c8ab10a68b1b3fe1eeecaa5f99ed1ee54bce175e8d60e02f0ef5058246f68a`  
		Last Modified: Mon, 28 Sep 2020 22:41:34 GMT  
		Size: 316.1 MB (316101630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a49ad5d0992d7b9a4c2401758de12ebc825bb8b429a64967c02afba256ef53`  
		Last Modified: Mon, 28 Sep 2020 22:40:42 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2c85c995eff78b3f8192d2b7431290f695c64e4a9653162ffed040cbb2e968`  
		Last Modified: Mon, 28 Sep 2020 22:40:42 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfc9a234a2013fae439a532cbaace8f7e7d8a48b2cf4e6e980ebb7fa44f14a0`  
		Last Modified: Mon, 28 Sep 2020 22:40:42 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724bf09a020c4f2a6813909a77e8a3204a5de996038f7c730bcaa87c86aeb288`  
		Last Modified: Mon, 28 Sep 2020 22:40:42 GMT  
		Size: 211.0 KB (211025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
