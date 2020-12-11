<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.13`](#elasticsearch6813)
-	[`elasticsearch:7.10.1`](#elasticsearch7101)

## `elasticsearch:6.8.13`

```console
$ docker pull elasticsearch@sha256:8d4e29332dc159e7c256efa131453bd62a35b6e90f32aa9ab3f76632e29372c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `elasticsearch:6.8.13` - linux; amd64

```console
$ docker pull elasticsearch@sha256:8a1fe3c94950c07fa156aec633b7fc946cd81645b8c48e306535da675a69fc6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.8 MB (440820933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e1d4b5ee814bc6c25cb4c8a2ee7950f25ca0f7621005405484b94b40e0f976`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Fri, 16 Oct 2020 09:18:17 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 16 Oct 2020 09:18:18 GMT
ENV JAVA_HOME=/opt/jdk-15+36
# Fri, 16 Oct 2020 09:18:24 GMT
COPY dir:d78ffb599e9e9b4589ff70ac49aaeab0c8bd3455dac60ff715fb156774755752 in /opt/jdk-15+36 
# Fri, 16 Oct 2020 09:18:34 GMT
RUN for iter in {1..10}; do yum update  --setopt=tsflags=nodocs -y &&     yum install -y  --setopt=tsflags=nodocs nc unzip wget which &&     yum clean all && exit_code=0 && break || exit_code=\$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Fri, 16 Oct 2020 09:18:36 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Fri, 16 Oct 2020 09:18:37 GMT
WORKDIR /usr/share/elasticsearch
# Fri, 16 Oct 2020 09:18:43 GMT
COPY --chown=1000:0dir:787d275540a0eea8d7d841a45f6cec0bfb0a080933199b53aa7a277315198546 in /usr/share/elasticsearch 
# Fri, 16 Oct 2020 09:18:43 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Oct 2020 09:18:44 GMT
COPY --chown=1000:0file:08193f849fc25f29db1438eff6d5c9fe1d63237aeb07a3e0009e8ba554f97c31 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 16 Oct 2020 09:18:45 GMT
RUN chgrp 0 /usr/local/bin/docker-entrypoint.sh &&     chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Fri, 16 Oct 2020 09:18:45 GMT
EXPOSE 9200 9300
# Fri, 16 Oct 2020 09:18:45 GMT
LABEL org.label-schema.build-date=2020-10-16T09:09:46.555371Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=be13c699d0ab4706ec25626375b0965e3cdfa138 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=6.8.13 org.opencontainers.image.created=2020-10-16T09:09:46.555371Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=be13c699d0ab4706ec25626375b0965e3cdfa138 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=6.8.13
# Fri, 16 Oct 2020 09:18:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 16 Oct 2020 09:18:46 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddf21112a95c2b297c9501907ea7830e6e4a56044aa9a64628e5bc4db52e157`  
		Last Modified: Thu, 22 Oct 2020 13:53:03 GMT  
		Size: 207.6 MB (207649973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9eb3eb5dbd4f6e0f58a238f77287efcd8d0493f75a967ee0bb85560786b031f`  
		Last Modified: Thu, 22 Oct 2020 13:52:30 GMT  
		Size: 7.2 MB (7197391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec630f80209e807986f3133930339442edbade997649eb1c85c0edb0d215f1db`  
		Last Modified: Thu, 22 Oct 2020 13:52:28 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c6cedc99d3f0ee71111a79c397e76c8c0e3a5efa5ae0224dab1bdd664a9356`  
		Last Modified: Thu, 22 Oct 2020 13:52:40 GMT  
		Size: 150.1 MB (150103638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a8f20dfc6929720417e888382d2edf8e28e28854d275f00129e7cbe9a1d14`  
		Last Modified: Thu, 22 Oct 2020 13:52:25 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb9e7bea81267646c5a5db3fa9bd4f43cccf91081d1e8def3a4d3c5ec048a4`  
		Last Modified: Thu, 22 Oct 2020 13:52:25 GMT  
		Size: 2.4 KB (2402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:7.10.1`

```console
$ docker pull elasticsearch@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
