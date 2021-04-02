<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.15`](#elasticsearch6815)
-	[`elasticsearch:7.12.0`](#elasticsearch7120)

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

## `elasticsearch:7.12.0`

```console
$ docker pull elasticsearch@sha256:383e9fb572f3ca2fdef5ba2edb0dae2c467736af96aba2c193722aa0c08ca7ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.12.0` - linux; amd64

```console
$ docker pull elasticsearch@sha256:337003ae571eedd3272cfa935386fa4ea52f74f5a4531f70790a74f092437122
```

-	Docker Version: 20.10.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.8 MB (428750860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9337ed510a0c8f147628631000504ef85e2c808b75cade2d86a09b71ff2bbbf0`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 06:25:09 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y       nc shadow-utils zip unzip  &&       yum clean all &&       exit_code=0 && break ||         exit_code=$? && echo "yum error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Thu, 18 Mar 2021 06:25:13 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chown -R 1000:0 /usr/share/elasticsearch
# Thu, 18 Mar 2021 06:25:13 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 18 Mar 2021 06:25:14 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 18 Mar 2021 06:25:38 GMT
COPY --chown=1000:0dir:93ca6108378768c73bc78d3f798e78e23126cf6bae7be978c6b861e28e7482d7 in /usr/share/elasticsearch 
# Thu, 18 Mar 2021 06:25:40 GMT
COPY --chown=0:0file:cbfbfe828617d3c65a10427a333f66d6d0b1b1aaea532739bba4696579b6cb19 in /bin/tini 
# Thu, 18 Mar 2021 06:25:42 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Mar 2021 06:25:42 GMT
COPY file:b60644ac0fe4cb4e2bab5fb75a5f9b33fa1cb8276d88703c138a52af6bd8ea5b in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Mar 2021 06:25:49 GMT
RUN chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     ln -sf /etc/pki/ca-trust/extracted/java/cacerts /usr/share/elasticsearch/jdk/lib/security/cacerts
# Thu, 18 Mar 2021 06:25:50 GMT
EXPOSE 9200 9300
# Thu, 18 Mar 2021 06:25:52 GMT
LABEL org.label-schema.build-date=2021-03-18T06:17:15.410153305Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=78722783c38caa25a70982b5b042074cde5d3b3a org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.12.0 org.opencontainers.image.created=2021-03-18T06:17:15.410153305Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=78722783c38caa25a70982b5b042074cde5d3b3a org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.12.0
# Thu, 18 Mar 2021 06:25:53 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 18 Mar 2021 06:25:55 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b674c951ca3fadb8221ca6bd14094c02bfea2267aa71ba770efbe822c0946e5`  
		Last Modified: Tue, 23 Mar 2021 15:57:39 GMT  
		Size: 24.2 MB (24160645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06baeb69f25f248eceb6170d6fcb8cc2d061c8da97d92aa16b075a3a87a6136f`  
		Last Modified: Tue, 23 Mar 2021 15:57:19 GMT  
		Size: 2.4 KB (2372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff01d19ce5bcfa5c5320384fd3ead0d5607b874068904d12167ccef9bf6a40`  
		Last Modified: Tue, 23 Mar 2021 15:58:14 GMT  
		Size: 329.2 MB (329198546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a994306398cabaa6aa80989dbda3119f1b6a659060c737f4cfba37aaf3655cc3`  
		Last Modified: Tue, 23 Mar 2021 15:57:18 GMT  
		Size: 9.5 KB (9537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c002d76c1f67f6fed27b4cc0ece7472a2b5ab726e956f8e5650142817e02ba5`  
		Last Modified: Tue, 23 Mar 2021 15:57:19 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6286f2196f9bf47ed60a719189e0803738f40780bcfe2180ec6d817d732294d6`  
		Last Modified: Tue, 23 Mar 2021 15:57:18 GMT  
		Size: 195.8 KB (195817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.12.0` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:6ecd0d2d606f55bf43e810b5c8a1ac8fa719fa48343fe104757699912d4c2b19
```

-	Docker Version: 20.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **425.9 MB (425940118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49283431aef6fe2938e9f502918b9ef40421082252f3b3cacbdddc0cefddaacd`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Mon, 07 Dec 2020 23:42:06 GMT
ADD file:edd6e1253ec7bbb67b5a28d40c7d28b34a443c2cfa327bebf55c8b0b19484bf9 in / 
# Mon, 07 Dec 2020 23:42:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Mon, 07 Dec 2020 23:42:10 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 07:08:00 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y       nc shadow-utils zip unzip  &&       yum clean all &&       exit_code=0 && break ||         exit_code=$? && echo "yum error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Thu, 18 Mar 2021 07:08:01 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chown -R 1000:0 /usr/share/elasticsearch
# Thu, 18 Mar 2021 07:08:01 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 18 Mar 2021 07:08:01 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 18 Mar 2021 07:08:05 GMT
COPY --chown=1000:0dir:02ebc5a92b1cd31a6bd8ec800e56287b49eb75b57071e3097f12c4a021fc64e9 in /usr/share/elasticsearch 
# Thu, 18 Mar 2021 07:08:09 GMT
COPY --chown=0:0file:1d48586bd42e8cf29bed9d4feee798b5c536660cc7b115750f0cd4f7bd33c311 in /bin/tini 
# Thu, 18 Mar 2021 07:08:09 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Mar 2021 07:08:10 GMT
COPY file:b60644ac0fe4cb4e2bab5fb75a5f9b33fa1cb8276d88703c138a52af6bd8ea5b in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Mar 2021 07:08:10 GMT
RUN chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     ln -sf /etc/pki/ca-trust/extracted/java/cacerts /usr/share/elasticsearch/jdk/lib/security/cacerts
# Thu, 18 Mar 2021 07:08:10 GMT
EXPOSE 9200 9300
# Thu, 18 Mar 2021 07:08:11 GMT
LABEL org.label-schema.build-date=2021-03-18T07:06:31.670489143Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=78722783c38caa25a70982b5b042074cde5d3b3a org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.12.0 org.opencontainers.image.created=2021-03-18T07:06:31.670489143Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=78722783c38caa25a70982b5b042074cde5d3b3a org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.12.0
# Thu, 18 Mar 2021 07:08:11 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 18 Mar 2021 07:08:11 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:333cbcae3fb80b9a46084ae4caea81a84aafda9700fb646ab89206d0cfe213fd`  
		Last Modified: Mon, 07 Dec 2020 23:42:49 GMT  
		Size: 75.6 MB (75613064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad1ce7569a047e1fb17bc9918b5d7b74d03a181296ad3e40d00cd986cda3460`  
		Last Modified: Thu, 01 Apr 2021 21:14:45 GMT  
		Size: 23.7 MB (23719165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82135e026bf0875593e502d15b364500d60e21bfad8b1f91c61a19a2b5bd195e`  
		Last Modified: Thu, 01 Apr 2021 21:14:36 GMT  
		Size: 2.4 KB (2373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf318b78920ac85fe87ac2e0295fab2a311465c0355637611d3e59c13f5658e`  
		Last Modified: Thu, 01 Apr 2021 21:15:27 GMT  
		Size: 326.4 MB (326399344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661831a6fae5b3d356d23c3cd0599ea7c587512bc9572ee24e98ecf7f9a8792b`  
		Last Modified: Thu, 01 Apr 2021 21:14:36 GMT  
		Size: 9.1 KB (9107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91e1632de105d5fbad59c2e1da7885fbdc05eaaab852c979d05cb7ae747ce9d`  
		Last Modified: Thu, 01 Apr 2021 21:14:36 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa437c7674d9eb2f31af79c7ef74a452bce745e9a14b77a0b337a5ba3ef4236`  
		Last Modified: Thu, 01 Apr 2021 21:14:38 GMT  
		Size: 195.1 KB (195124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
