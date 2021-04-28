<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.15`](#elasticsearch6815)
-	[`elasticsearch:7.12.1`](#elasticsearch7121)

## `elasticsearch:6.8.15`

```console
$ docker pull elasticsearch@sha256:fa7433fcb125b5c89e2db80918f460e4097cdcfcf1694e268a114270d70ec23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `elasticsearch:6.8.15` - linux; amd64

```console
$ docker pull elasticsearch@sha256:a4a020e64f64a12262aced394a20153b21b307ae7985f73c6b869e6cdcbe6131
```

-	Docker Version: 20.10.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **479.8 MB (479849192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71dbc55f668dad4f27786066060ffde16f347dc7c8345ab90b09e1157bf7b6e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 06:38:46 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 18 Mar 2021 06:38:48 GMT
ENV JAVA_HOME=/opt/jdk-15.0.1+9
# Thu, 18 Mar 2021 06:38:56 GMT
COPY dir:8d79ae5f21bb18379c0d92b3d252f4730fec22a4509252ec794212b8f72bd7af in /opt/jdk-15.0.1+9 
# Thu, 18 Mar 2021 06:39:58 GMT
RUN for iter in {1..10}; do yum update  --setopt=tsflags=nodocs -y &&     yum install -y  --setopt=tsflags=nodocs nc unzip wget which &&     yum clean all && exit_code=0 && break || exit_code=\$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Thu, 18 Mar 2021 06:40:00 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Thu, 18 Mar 2021 06:40:01 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 18 Mar 2021 06:40:06 GMT
COPY --chown=1000:0dir:bb53662b52f576e56386260cb35c528866996ddd5f87ba1d0573eff4bd6ad3c1 in /usr/share/elasticsearch 
# Thu, 18 Mar 2021 06:40:06 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Mar 2021 06:40:07 GMT
COPY --chown=1000:0file:08193f849fc25f29db1438eff6d5c9fe1d63237aeb07a3e0009e8ba554f97c31 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Mar 2021 06:40:09 GMT
RUN chgrp 0 /usr/local/bin/docker-entrypoint.sh &&     chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Thu, 18 Mar 2021 06:40:09 GMT
EXPOSE 9200 9300
# Thu, 18 Mar 2021 06:40:10 GMT
LABEL org.label-schema.build-date=2021-03-18T06:33:32.588487Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=c9a8c60f59a902dfa018abda97b195f7ba9f29aa org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=6.8.15 org.opencontainers.image.created=2021-03-18T06:33:32.588487Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=c9a8c60f59a902dfa018abda97b195f7ba9f29aa org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=6.8.15
# Thu, 18 Mar 2021 06:40:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 18 Mar 2021 06:40:11 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d2a6bc4529ec41290eade86ead2e35adfe70d2fc4d9e7daa0705c289268094`  
		Last Modified: Tue, 23 Mar 2021 13:50:07 GMT  
		Size: 207.7 MB (207657697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e7ca20d705bc564bbc887c37719377ca2e97b30463f55a4555c88636eda2f`  
		Last Modified: Tue, 23 Mar 2021 13:50:02 GMT  
		Size: 46.0 MB (45959281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e358dab17355c3301934ef365a5c8e709e8802c91387858a26d7c8b15858e996`  
		Last Modified: Tue, 23 Mar 2021 13:49:47 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f67e30bb9fdd10fc4c310217f041d893d7f28adf748f28bda4880b93b12f21`  
		Last Modified: Tue, 23 Mar 2021 13:50:01 GMT  
		Size: 150.1 MB (150128276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29090ccafdcace322e29724fb1d373a3a0bc0a0e5d0bd64406b0db09bc194d63`  
		Last Modified: Tue, 23 Mar 2021 13:49:46 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6764b4f35508eb86b0b503e3c8526ce38e2fbd8990beaf14c2bc249bc57c20c7`  
		Last Modified: Tue, 23 Mar 2021 13:49:46 GMT  
		Size: 2.4 KB (2402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:7.12.1`

**does not exist** (yet?)
