<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.22`](#elasticsearch6822)
-	[`elasticsearch:7.16.2`](#elasticsearch7162)

## `elasticsearch:6.8.22`

```console
$ docker pull elasticsearch@sha256:95de2fb1fc05e1c5f19c8e39ab6691c4ec8eb6c78b4469bc582647fc4fbc48bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `elasticsearch:6.8.22` - linux; amd64

```console
$ docker pull elasticsearch@sha256:e20bcda3c57ecc2f901d61fa3811465e2520d33a53d5c70c891d689847ea3cdd
```

-	Docker Version: 20.10.10
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.7 MB (492662101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bf941c09b95156c677e8518111577f21996fbd4fe2d30d3c0d50b94191fc689`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Sun, 19 Dec 2021 01:16:58 GMT
ENV ELASTIC_CONTAINER=true
# Sun, 19 Dec 2021 01:16:58 GMT
ENV JAVA_HOME=/opt/jdk-15.0.1+9
# Sun, 19 Dec 2021 01:17:10 GMT
COPY dir:8d79ae5f21bb18379c0d92b3d252f4730fec22a4509252ec794212b8f72bd7af in /opt/jdk-15.0.1+9 
# Sun, 19 Dec 2021 01:18:11 GMT
RUN for iter in {1..10}; do yum update  --setopt=tsflags=nodocs -y &&     yum install -y  --setopt=tsflags=nodocs nc unzip wget which &&     yum clean all && exit_code=0 && break || exit_code=\$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Sun, 19 Dec 2021 01:18:13 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Sun, 19 Dec 2021 01:18:13 GMT
WORKDIR /usr/share/elasticsearch
# Sun, 19 Dec 2021 01:18:19 GMT
COPY --chown=1000:0dir:b79a54eb984345cc2fbb03db213a63d061749a623c44953da80bf99c9f4ecc73 in /usr/share/elasticsearch 
# Sun, 19 Dec 2021 01:18:20 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 19 Dec 2021 01:18:21 GMT
COPY --chown=1000:0file:08193f849fc25f29db1438eff6d5c9fe1d63237aeb07a3e0009e8ba554f97c31 in /usr/local/bin/docker-entrypoint.sh 
# Sun, 19 Dec 2021 01:18:23 GMT
RUN chgrp 0 /usr/local/bin/docker-entrypoint.sh &&     chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Sun, 19 Dec 2021 01:18:23 GMT
EXPOSE 9200 9300
# Sun, 19 Dec 2021 01:18:24 GMT
LABEL org.label-schema.build-date=2021-12-19T01:10:56.497443Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=71fcb50e179e8ff6f36ccc96fefc1d9fb484c734 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=6.8.22 org.opencontainers.image.created=2021-12-19T01:10:56.497443Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=71fcb50e179e8ff6f36ccc96fefc1d9fb484c734 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=6.8.22
# Sun, 19 Dec 2021 01:18:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sun, 19 Dec 2021 01:18:24 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd93047f409b0f1f2c8ddfe61d0e394c53f3abcc944d130d5c29b3f74dd27c7`  
		Last Modified: Sun, 19 Dec 2021 20:54:20 GMT  
		Size: 207.7 MB (207657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221803e6108b62f9f1750f3240599371663f841ff364c6b6663ae54a53808846`  
		Last Modified: Sun, 19 Dec 2021 20:54:13 GMT  
		Size: 58.2 MB (58238759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475ee6ce7d6b7d239eaa07de097d32e17438e0eee6618de08d511664ea1d90fb`  
		Last Modified: Sun, 19 Dec 2021 20:54:06 GMT  
		Size: 2.3 KB (2317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f5b8058898177e3877c1da76ed7673a82305d4aeab0ae1bb16d460283e72d7`  
		Last Modified: Sun, 19 Dec 2021 20:54:17 GMT  
		Size: 150.7 MB (150661747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671234d166d6e08048a062e3048c72eb909a3b9d40eb3685836e5463c9ed1f15`  
		Last Modified: Sun, 19 Dec 2021 20:54:03 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f28e098f061afce8acacef7f53f0a609efbdad8a03e02197ef8329a09c0ae0`  
		Last Modified: Sun, 19 Dec 2021 20:54:03 GMT  
		Size: 2.4 KB (2401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:7.16.2`

```console
$ docker pull elasticsearch@sha256:fe7ae76ec33e1222ece5216e3a9c6346999a73d3fb65256abb01638758db4b5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.16.2` - linux; amd64

```console
$ docker pull elasticsearch@sha256:3e82c0aefb87f2b716d0d09ffc252076b200a05eb1692c795dcb5c3057952477
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.5 MB (382549502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c29cde15cefd5a697365a004cc4e887cf9b40cdea32d961fc805381d2b623d`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sun, 19 Dec 2021 00:19:08 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Sun, 19 Dec 2021 00:19:09 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Sun, 19 Dec 2021 00:19:09 GMT
ENV ELASTIC_CONTAINER=true
# Sun, 19 Dec 2021 00:19:10 GMT
WORKDIR /usr/share/elasticsearch
# Sun, 19 Dec 2021 00:19:17 GMT
COPY --chown=0:0dir:a84e5e9b2d41756dd522fa3f09be04d6bd4a7755262e376e557495c9be14d0f6 in /usr/share/elasticsearch 
# Sun, 19 Dec 2021 00:19:20 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Sun, 19 Dec 2021 00:19:20 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 19 Dec 2021 00:19:20 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Sun, 19 Dec 2021 00:19:21 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Sun, 19 Dec 2021 00:19:21 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Sun, 19 Dec 2021 00:19:22 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Sun, 19 Dec 2021 00:19:22 GMT
EXPOSE 9200 9300
# Sun, 19 Dec 2021 00:19:22 GMT
LABEL org.label-schema.build-date=2021-12-19T00:16:42.756969090Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=2b937c44140b6559905130a8650c64dbd0879cfb org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.16.2 org.opencontainers.image.created=2021-12-19T00:16:42.756969090Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=2b937c44140b6559905130a8650c64dbd0879cfb org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.16.2
# Sun, 19 Dec 2021 00:19:22 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Sun, 19 Dec 2021 00:19:22 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f9908af642bc5bb87a5580bd911de3c7082a279296727070067fd5165e482f`  
		Last Modified: Sun, 19 Dec 2021 13:21:21 GMT  
		Size: 8.3 MB (8306413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04928834f6a2e383dca0d57d342477a9e28143f4e45c4ee08397d5e144d0b952`  
		Last Modified: Sun, 19 Dec 2021 13:21:19 GMT  
		Size: 4.4 KB (4373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f647d55d420f23af45fa03073d89d739d5bd43c31eb8a1b553896006f4c2fe8`  
		Last Modified: Sun, 19 Dec 2021 13:21:37 GMT  
		Size: 345.4 MB (345363707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7afec4a2d7a582fd241c45fa316035aed10d6dca281851f9482c9bfe60f04f`  
		Last Modified: Sun, 19 Dec 2021 13:21:17 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146b4a7018b9f710ab33158af1f16aa117051132a7cf3b4c8c176a0ba9d0ff39`  
		Last Modified: Sun, 19 Dec 2021 13:21:15 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc193d8d7c71d806276274ccb811ffcfc09ef891b563cb5aec6070a4b4ed569d`  
		Last Modified: Sun, 19 Dec 2021 13:21:16 GMT  
		Size: 192.1 KB (192127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb19b2c38ae118ebccc3ba98ebae836af472bed1e4804be135e6fd5f036a7`  
		Last Modified: Sun, 19 Dec 2021 13:21:14 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b79893ce5a3ebbb11abf7879e6fce3845dd2b57ffc2f9670018fefa9cfedd5e`  
		Last Modified: Sun, 19 Dec 2021 13:21:14 GMT  
		Size: 103.9 KB (103867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.16.2` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:5837d1482e31630c7c8f0b309743361c260c50749dd2ca14d96b8950f727993b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.5 MB (377483701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e082d8ac7e5eae3c4ce3015db758c02a5a1b9632ee236f87d68b36888f27b6c4`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sun, 19 Dec 2021 00:21:03 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Sun, 19 Dec 2021 00:21:04 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Sun, 19 Dec 2021 00:21:04 GMT
ENV ELASTIC_CONTAINER=true
# Sun, 19 Dec 2021 00:21:04 GMT
WORKDIR /usr/share/elasticsearch
# Sun, 19 Dec 2021 00:21:09 GMT
COPY --chown=0:0dir:19a1de97b8859a3faa3f0ccabd812ca69eb4c98f175be6a35fdb7052cff647e7 in /usr/share/elasticsearch 
# Sun, 19 Dec 2021 00:21:12 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Sun, 19 Dec 2021 00:21:12 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 19 Dec 2021 00:21:13 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Sun, 19 Dec 2021 00:21:13 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Sun, 19 Dec 2021 00:21:13 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Sun, 19 Dec 2021 00:21:14 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Sun, 19 Dec 2021 00:21:14 GMT
EXPOSE 9200 9300
# Sun, 19 Dec 2021 00:21:14 GMT
LABEL org.label-schema.build-date=2021-12-19T00:19:05.483528077Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=2b937c44140b6559905130a8650c64dbd0879cfb org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.16.2 org.opencontainers.image.created=2021-12-19T00:19:05.483528077Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=2b937c44140b6559905130a8650c64dbd0879cfb org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.16.2
# Sun, 19 Dec 2021 00:21:14 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Sun, 19 Dec 2021 00:21:14 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f04d38758f714d622b694e50f75aeeabda6b0266d766dc590d2b0ed0777af1`  
		Last Modified: Tue, 21 Dec 2021 00:40:01 GMT  
		Size: 8.1 MB (8135172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff284304c6e213ea7ee4bdb674bfc18b2fb951c9c8a0899c2eb1d2671b304b72`  
		Last Modified: Tue, 21 Dec 2021 00:40:00 GMT  
		Size: 4.4 KB (4376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0977aa7b61a2e92a20fef14b13c2726fef6beeb2431302078e5dc31c8f4c6d94`  
		Last Modified: Tue, 21 Dec 2021 00:40:32 GMT  
		Size: 341.9 MB (341871754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183dccc90e7138905cc3769aa935558f79d3e401cf7e80c8f833dd8e5e0dbcff`  
		Last Modified: Tue, 21 Dec 2021 00:39:57 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e28a3fcbc334550351cd3eb59700da8019ae8774863faedb00362f9c3b84a2e`  
		Last Modified: Tue, 21 Dec 2021 00:39:57 GMT  
		Size: 2.0 KB (1981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d89da09830a43e9628d99b22a4ebca7a2d60edb5b9058f0fd82f956517d267f`  
		Last Modified: Tue, 21 Dec 2021 00:39:58 GMT  
		Size: 186.1 KB (186149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18ca4ae6e3a1bfd31f2c12c8d4e6dc53de2e009d7abf9b824ca03e557259653`  
		Last Modified: Tue, 21 Dec 2021 00:39:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f7daaf7d736f5de791839017f359052124be1df120b1f44b9790d130c3d0f9`  
		Last Modified: Tue, 21 Dec 2021 00:39:57 GMT  
		Size: 103.9 KB (103868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
