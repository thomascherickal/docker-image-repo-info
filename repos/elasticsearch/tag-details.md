<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.18`](#elasticsearch6818)
-	[`elasticsearch:7.14.1`](#elasticsearch7141)

## `elasticsearch:6.8.18`

```console
$ docker pull elasticsearch@sha256:a676c5eadeaff21fb0ed9b7f6be7dcb559dc25dcc017940197dd5ced0f90dbfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `elasticsearch:6.8.18` - linux; amd64

```console
$ docker pull elasticsearch@sha256:0f16a358b58c4d233258c87fe2dd9762d02eb0561ff9e72aa9814e03f2e2dd15
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **482.2 MB (482221730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b226f5ba29f397cac809b642d7f9f9bc7e865c4e248ccb65e6b9cee09bea2d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Wed, 28 Jul 2021 16:10:35 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 28 Jul 2021 16:10:36 GMT
ENV JAVA_HOME=/opt/jdk-15.0.1+9
# Wed, 28 Jul 2021 16:10:41 GMT
COPY dir:8d79ae5f21bb18379c0d92b3d252f4730fec22a4509252ec794212b8f72bd7af in /opt/jdk-15.0.1+9 
# Wed, 28 Jul 2021 16:11:23 GMT
RUN for iter in {1..10}; do yum update  --setopt=tsflags=nodocs -y &&     yum install -y  --setopt=tsflags=nodocs nc unzip wget which &&     yum clean all && exit_code=0 && break || exit_code=\$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Wed, 28 Jul 2021 16:11:25 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Wed, 28 Jul 2021 16:11:25 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 28 Jul 2021 16:11:28 GMT
COPY --chown=1000:0dir:2b0d1a24665560d0012df6c5f68f16ea5e598782bfc6749adbf0f56f745fdcf3 in /usr/share/elasticsearch 
# Wed, 28 Jul 2021 16:11:29 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Jul 2021 16:11:29 GMT
COPY --chown=1000:0file:08193f849fc25f29db1438eff6d5c9fe1d63237aeb07a3e0009e8ba554f97c31 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 28 Jul 2021 16:11:30 GMT
RUN chgrp 0 /usr/local/bin/docker-entrypoint.sh &&     chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Wed, 28 Jul 2021 16:11:30 GMT
EXPOSE 9200 9300
# Wed, 28 Jul 2021 16:11:31 GMT
LABEL org.label-schema.build-date=2021-07-28T16:06:05.232873Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=aca23296a2422a5abea96a1b6b590f6566e9c02f org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=6.8.18 org.opencontainers.image.created=2021-07-28T16:06:05.232873Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=aca23296a2422a5abea96a1b6b590f6566e9c02f org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=6.8.18
# Wed, 28 Jul 2021 16:11:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 16:11:31 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0128b25cc806662d7fe5ee6828f183c810828baa43cf452ddb469980ae5c4ff3`  
		Last Modified: Tue, 03 Aug 2021 12:57:47 GMT  
		Size: 207.7 MB (207657662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e926b4f11fd8c1a1adffe67a9c0803a29698dba31660155078e0b337de05753`  
		Last Modified: Tue, 03 Aug 2021 12:57:27 GMT  
		Size: 48.3 MB (48319743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01aa6e6c3b0500fe4d3d1bc5e21b20db804d517a6f48bc911b001e0577b3544`  
		Last Modified: Tue, 03 Aug 2021 12:57:16 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f53e5ee82cadd34edd16d8d5f9354aa1615988ba5c57670bb2b7dce330df0f3`  
		Last Modified: Tue, 03 Aug 2021 12:57:34 GMT  
		Size: 150.1 MB (150140389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045fa98c98d76b32e4a3f9ea1ab9f8e56b0efb02a13451db236b413feec67e7`  
		Last Modified: Tue, 03 Aug 2021 12:57:16 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec43e9f984f6fc2ffe54f846e2ca96c37af763371f2333fb82c3e54bb3468b1`  
		Last Modified: Tue, 03 Aug 2021 12:57:16 GMT  
		Size: 2.4 KB (2402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:7.14.1`

```console
$ docker pull elasticsearch@sha256:80bc3fe9d3ab2da410abadc2245eb5833c7ef7bb58ce2d89b24dabfb8c3d5233
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.14.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:3719432f511d2e348676e56e111c0e6b9b8f831062e429b78c1b0d2fe96a3bbb
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **512.9 MB (512928157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f287f2cfc393dfd1753034320bed67bc3205f0c3c8a0cbf473f37c3ec8330b72`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Thu, 26 Aug 2021 09:09:35 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y       nc shadow-utils zip unzip  &&       yum clean all &&       exit_code=0 && break ||         exit_code=$? && echo "yum error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Thu, 26 Aug 2021 09:09:37 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chown -R 1000:0 /usr/share/elasticsearch
# Thu, 26 Aug 2021 09:09:37 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 26 Aug 2021 09:09:38 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 26 Aug 2021 09:09:52 GMT
COPY --chown=1000:0dir:ae21f60382363d90b9226998ed46987a0f9f3e904aeece7e876c765dbdab81e7 in /usr/share/elasticsearch 
# Thu, 26 Aug 2021 09:09:53 GMT
COPY --chown=0:0file:cbfbfe828617d3c65a10427a333f66d6d0b1b1aaea532739bba4696579b6cb19 in /bin/tini 
# Thu, 26 Aug 2021 09:09:53 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Aug 2021 09:09:53 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Thu, 26 Aug 2021 09:09:56 GMT
RUN chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     ln -sf /etc/pki/ca-trust/extracted/java/cacerts /usr/share/elasticsearch/jdk/lib/security/cacerts
# Thu, 26 Aug 2021 09:09:57 GMT
EXPOSE 9200 9300
# Thu, 26 Aug 2021 09:09:57 GMT
LABEL org.label-schema.build-date=2021-08-26T09:01:05.390870785Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=66b55ebfa59c92c15db3f69a335d500018b3331e org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.14.1 org.opencontainers.image.created=2021-08-26T09:01:05.390870785Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=66b55ebfa59c92c15db3f69a335d500018b3331e org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.14.1
# Thu, 26 Aug 2021 09:09:57 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 26 Aug 2021 09:09:58 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676f9b0455ba4d508e035773a7eab61d6ee975a3abd0e25ea553806f4983a0da`  
		Last Modified: Wed, 01 Sep 2021 18:41:26 GMT  
		Size: 91.8 MB (91793108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2883bec0e7105d01c4822922438d600b07e3fe41a7939d5c60b3aef5cf7a0d0`  
		Last Modified: Wed, 01 Sep 2021 18:41:03 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da0c921bd93bda616f9008e6e9bb74dd1eb33d7605384c1bae4c9a1877bff3f`  
		Last Modified: Wed, 01 Sep 2021 18:41:49 GMT  
		Size: 345.7 MB (345739450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006b83acd4d9eff0b3cf7dffddfd658fa0ac07147887ed79f65eb3e54ceeeb5c`  
		Last Modified: Wed, 01 Sep 2021 18:41:03 GMT  
		Size: 9.5 KB (9536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7d661103bfc1c38dc1c51f87ba250ae98861cb77deda5e22cf615fbe2d6cdb`  
		Last Modified: Wed, 01 Sep 2021 18:40:59 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351a057c286e93bdae4426939a92f3273a815a995e02a18714693dc7bd3f583c`  
		Last Modified: Wed, 01 Sep 2021 18:40:59 GMT  
		Size: 199.7 KB (199690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.14.1` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:75718885ae60ed8aad6ac8ba6c6522ea41c7fac0c1a0bdb9e719f585baaf3e49
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **510.6 MB (510602327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7467d725d0259e8db758c355b920dd4778ee8988fd347b91bb47e560cde0e5d7`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 07 Dec 2020 23:42:06 GMT
ADD file:edd6e1253ec7bbb67b5a28d40c7d28b34a443c2cfa327bebf55c8b0b19484bf9 in / 
# Mon, 07 Dec 2020 23:42:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Mon, 07 Dec 2020 23:42:10 GMT
CMD ["/bin/bash"]
# Thu, 26 Aug 2021 10:08:57 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y       nc shadow-utils zip unzip  &&       yum clean all &&       exit_code=0 && break ||         exit_code=$? && echo "yum error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Thu, 26 Aug 2021 10:08:58 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chown -R 1000:0 /usr/share/elasticsearch
# Thu, 26 Aug 2021 10:08:58 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 26 Aug 2021 10:08:59 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 26 Aug 2021 10:09:09 GMT
COPY --chown=1000:0dir:0ec9ec6c591086987eb7c75b0239b1db101f178288f85ace6e350577a01d8bbe in /usr/share/elasticsearch 
# Thu, 26 Aug 2021 10:09:11 GMT
COPY --chown=0:0file:1d48586bd42e8cf29bed9d4feee798b5c536660cc7b115750f0cd4f7bd33c311 in /bin/tini 
# Thu, 26 Aug 2021 10:09:11 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Aug 2021 10:09:11 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Thu, 26 Aug 2021 10:09:13 GMT
RUN chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     ln -sf /etc/pki/ca-trust/extracted/java/cacerts /usr/share/elasticsearch/jdk/lib/security/cacerts
# Thu, 26 Aug 2021 10:09:13 GMT
EXPOSE 9200 9300
# Thu, 26 Aug 2021 10:09:13 GMT
LABEL org.label-schema.build-date=2021-08-26T10:04:00.602808229Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=66b55ebfa59c92c15db3f69a335d500018b3331e org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.14.1 org.opencontainers.image.created=2021-08-26T10:04:00.602808229Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=66b55ebfa59c92c15db3f69a335d500018b3331e org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.14.1
# Thu, 26 Aug 2021 10:09:14 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 26 Aug 2021 10:09:14 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:333cbcae3fb80b9a46084ae4caea81a84aafda9700fb646ab89206d0cfe213fd`  
		Last Modified: Mon, 07 Dec 2020 23:42:49 GMT  
		Size: 75.6 MB (75613064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bf28013b64ea8b5ab5d119d4c3e38391c70ca47b720a34328f263449a3cc65`  
		Last Modified: Wed, 01 Sep 2021 23:40:14 GMT  
		Size: 91.7 MB (91745883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf5c6e2fdd7686d10104131a5073d2b1e904da83bd64203854785d8b3f118f7`  
		Last Modified: Wed, 01 Sep 2021 23:39:55 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57878f080fedc3a9f78e5054e75f6a414f72e44567bd6127f0b03f69c8a3ff56`  
		Last Modified: Wed, 01 Sep 2021 23:40:27 GMT  
		Size: 343.0 MB (343029561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0211ec8f60a06da5bb5354a45610fa3be4e8dd0a2504bc0d779461433330cf`  
		Last Modified: Wed, 01 Sep 2021 23:39:55 GMT  
		Size: 9.1 KB (9110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8f8b9d0783eaa7ed6204b966554aedaaa23df3182a6d595f2b13356d3358a0`  
		Last Modified: Wed, 01 Sep 2021 23:39:55 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84390f1f69e0d33fb72dd81c709dc15628f6f11c06ddadf4a91af3f41320b337`  
		Last Modified: Wed, 01 Sep 2021 23:39:58 GMT  
		Size: 200.3 KB (200336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
