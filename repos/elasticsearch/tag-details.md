<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.21`](#elasticsearch6821)
-	[`elasticsearch:7.16.1`](#elasticsearch7161)

## `elasticsearch:6.8.21`

```console
$ docker pull elasticsearch@sha256:b85538ff815dd10b9486d17e81a4c9e55cc0d912657802ea0526feb993a9cdb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `elasticsearch:6.8.21` - linux; amd64

```console
$ docker pull elasticsearch@sha256:2f76a052cff7f04cdf8845d381b3d33c08382bfeceba0bcf0e22670097b48d6c
```

-	Docker Version: 20.10.10
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.1 MB (492122471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61444bb777f03e0d7dcbfd8ce6e529294228b3961a6ec3dde228817a5527ab70`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Sat, 11 Dec 2021 02:49:56 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 11 Dec 2021 02:49:57 GMT
ENV JAVA_HOME=/opt/jdk-15.0.1+9
# Sat, 11 Dec 2021 02:50:05 GMT
COPY dir:8d79ae5f21bb18379c0d92b3d252f4730fec22a4509252ec794212b8f72bd7af in /opt/jdk-15.0.1+9 
# Sat, 11 Dec 2021 02:51:05 GMT
RUN for iter in {1..10}; do yum update  --setopt=tsflags=nodocs -y &&     yum install -y  --setopt=tsflags=nodocs nc unzip wget which &&     yum clean all && exit_code=0 && break || exit_code=\$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Sat, 11 Dec 2021 02:51:08 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Sat, 11 Dec 2021 02:51:09 GMT
WORKDIR /usr/share/elasticsearch
# Sat, 11 Dec 2021 02:51:15 GMT
COPY --chown=1000:0dir:a881e866146471dafe787afb3b2604ddc140b863321790475279e32c6288d9fa in /usr/share/elasticsearch 
# Sat, 11 Dec 2021 02:51:17 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Dec 2021 02:51:17 GMT
COPY --chown=1000:0file:08193f849fc25f29db1438eff6d5c9fe1d63237aeb07a3e0009e8ba554f97c31 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Dec 2021 02:51:18 GMT
RUN chgrp 0 /usr/local/bin/docker-entrypoint.sh &&     chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Sat, 11 Dec 2021 02:51:18 GMT
EXPOSE 9200 9300
# Sat, 11 Dec 2021 02:51:19 GMT
LABEL org.label-schema.build-date=2021-12-11T02:44:56.385871Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=403e8db4f04f2330c29fa9a26b199e6efed15dc0 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=6.8.21 org.opencontainers.image.created=2021-12-11T02:44:56.385871Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=403e8db4f04f2330c29fa9a26b199e6efed15dc0 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=6.8.21
# Sat, 11 Dec 2021 02:51:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 11 Dec 2021 02:51:19 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02221e4ae11f7c1cf06d42036a7114bc0d8678bdc255f512e9b8be0fdfbeb1bb`  
		Last Modified: Mon, 13 Dec 2021 11:44:35 GMT  
		Size: 207.7 MB (207657657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b38a4aa0d5b362884825bfb686b2e4aa808cdd7650f9d2ac2e9d9091004b4ee`  
		Last Modified: Mon, 13 Dec 2021 11:44:30 GMT  
		Size: 58.2 MB (58238554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c16a18a37151a0041b2631a424c95a644b7bab50fed3b567ddd39199f2ec479`  
		Last Modified: Mon, 13 Dec 2021 11:44:20 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff32eb950b63a2f58db187c14fb62496f51821187616018b7d6b394713080cb`  
		Last Modified: Mon, 13 Dec 2021 11:44:30 GMT  
		Size: 150.1 MB (150122321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0b29bc478e4dcda7a30b123dabd60732bc80b7c8167ddfe5c065592b500497`  
		Last Modified: Mon, 13 Dec 2021 11:44:20 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff42a53d9255787e29bb1d387c306ee1a011023b90d9c5151c5a16b91ff8c22`  
		Last Modified: Mon, 13 Dec 2021 11:44:20 GMT  
		Size: 2.4 KB (2403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:7.16.1`

```console
$ docker pull elasticsearch@sha256:8d5fd89230d7985b106bc0586080647a6650ca0f6dfe6c22541ef149045ad52e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.16.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:4000fb7daa3ca86b3dc2ab2d492ddadd79f46367e5875d9871c34f97b1c94b5e
```

-	Docker Version: 20.10.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.5 MB (380515986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:405db9d10ee033c11d79243ac25702ba770f3f8560240a4ca6a03e9bace7894c`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 11 Dec 2021 05:12:20 GMT
RUN for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive && apt-get update && apt-get upgrade -y && apt-get install -y --no-install-recommends curl netcat zip unzip vim-tiny  && apt-get clean && rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Sat, 11 Dec 2021 05:12:20 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Sat, 11 Dec 2021 05:12:21 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 11 Dec 2021 05:12:21 GMT
WORKDIR /usr/share/elasticsearch
# Sat, 11 Dec 2021 05:12:28 GMT
COPY --chown=0:0dir:aa449cf97856b2728742a5679673a570e659211cb06225a60096ba151ea6228e in /usr/share/elasticsearch 
# Sat, 11 Dec 2021 05:12:32 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Sat, 11 Dec 2021 05:12:32 GMT
COPY --chown=0:0file:ab500cfbc0ffd86deed35f80ebd2f3bc60ec9b8063912c4a328e652ad438d04f in /etc/ssl/certs/java/cacerts 
# Sat, 11 Dec 2021 05:12:32 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Dec 2021 05:12:33 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Dec 2021 05:12:33 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     ln -sf /etc/ssl/certs/java/cacerts       /usr/share/elasticsearch/jdk/lib/security/cacerts &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Sat, 11 Dec 2021 05:12:33 GMT
EXPOSE 9200 9300
# Sat, 11 Dec 2021 05:12:33 GMT
LABEL org.label-schema.build-date=2021-12-11T05:09:38.080326932Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=5b38441b16b1ebb16a27c107a4c3865776e20c53 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.16.1 org.opencontainers.image.created=2021-12-11T05:09:38.080326932Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=5b38441b16b1ebb16a27c107a4c3865776e20c53 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.16.1
# Sat, 11 Dec 2021 05:12:34 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Sat, 11 Dec 2021 05:12:34 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85c3fdbf085cc499e666ffe0c06eff28045c9f0173aeef0fc759f6ea2b467f0`  
		Last Modified: Mon, 13 Dec 2021 10:23:43 GMT  
		Size: 7.1 MB (7123988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee9ef16ef16c27feb8f89413f3671f4597a25bdea3502bd752217c5e48ac89f`  
		Last Modified: Mon, 13 Dec 2021 10:23:39 GMT  
		Size: 4.4 KB (4371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b555fc21eda90058f57053e593ee9643b42e01c14a6cae05634c2aafc458f6a`  
		Last Modified: Mon, 13 Dec 2021 10:24:35 GMT  
		Size: 344.5 MB (344510564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5195df1d2493f089c1a03d85a83aecfec8e18c73581d90539680147f49ca6208`  
		Last Modified: Mon, 13 Dec 2021 10:23:37 GMT  
		Size: 9.5 KB (9530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22dfd95268faca25f94abbf01ca8a17df24becbf254f121dc7ea9b42e223fb4`  
		Last Modified: Mon, 13 Dec 2021 10:23:35 GMT  
		Size: 106.2 KB (106199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762293acfd23b4ef9034dde30bad74bc67a64f78a7241e167356ddd9f04cfcc2`  
		Last Modified: Mon, 13 Dec 2021 10:23:34 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d18a44f390beeb2f4407075c14f04c0b8cc0d2ee3847e3b97cb74b540a98e7`  
		Last Modified: Mon, 13 Dec 2021 10:23:31 GMT  
		Size: 192.3 KB (192255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.16.1` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:a6d6b405028e5fc2195bcad27a639bb9a6c19edeb91650f8d2114a9927ac9d07
```

-	Docker Version: 20.10.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.5 MB (375494360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a3f69ec8f54e0904343991c1fde2ab4c156d3c40732051a0eb1250740624643`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 11 Dec 2021 05:13:26 GMT
RUN for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive && apt-get update && apt-get upgrade -y && apt-get install -y --no-install-recommends curl netcat zip unzip vim-tiny  && apt-get clean && rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Sat, 11 Dec 2021 05:13:26 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Sat, 11 Dec 2021 05:13:27 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 11 Dec 2021 05:13:27 GMT
WORKDIR /usr/share/elasticsearch
# Sat, 11 Dec 2021 05:13:32 GMT
COPY --chown=0:0dir:436a00b9cff6472418e764365609df4ed97f3a5d4892364d546fc3a87edee21a in /usr/share/elasticsearch 
# Sat, 11 Dec 2021 05:13:35 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Sat, 11 Dec 2021 05:13:35 GMT
COPY --chown=0:0file:f1656904cdc70949960f8f3f59cda356bbee692f465b73ab51fb316e520d9110 in /etc/ssl/certs/java/cacerts 
# Sat, 11 Dec 2021 05:13:36 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Dec 2021 05:13:36 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Dec 2021 05:13:37 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     ln -sf /etc/ssl/certs/java/cacerts       /usr/share/elasticsearch/jdk/lib/security/cacerts &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Sat, 11 Dec 2021 05:13:37 GMT
EXPOSE 9200 9300
# Sat, 11 Dec 2021 05:13:37 GMT
LABEL org.label-schema.build-date=2021-12-11T05:11:08.265099940Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=5b38441b16b1ebb16a27c107a4c3865776e20c53 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.16.1 org.opencontainers.image.created=2021-12-11T05:11:08.265099940Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=5b38441b16b1ebb16a27c107a4c3865776e20c53 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.16.1
# Sat, 11 Dec 2021 05:13:37 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Sat, 11 Dec 2021 05:13:37 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1974b55a9a83da4cb18b28982f9a45b5e1e9edaa0505297e34a22331b45c269c`  
		Last Modified: Mon, 13 Dec 2021 23:34:36 GMT  
		Size: 7.0 MB (6981973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18470a1704778ba927ecb9c23154f2636273fbe05ae4ddc7ae329345f230551`  
		Last Modified: Mon, 13 Dec 2021 23:33:49 GMT  
		Size: 4.4 KB (4374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b31e84c21ea68e5f99da76801d8e257134258842d76abd9f6b4b50dfb35ef2`  
		Last Modified: Mon, 13 Dec 2021 23:41:13 GMT  
		Size: 341.0 MB (341033578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e1ca52d82ca3ebcaedb685885d74354ccaf68f9c23a72149466ab6cd2bf139`  
		Last Modified: Mon, 13 Dec 2021 23:33:41 GMT  
		Size: 9.1 KB (9103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c5093b45f02317ed5ff866ed97b2086fd70f4549720746dceb28108334c4a1`  
		Last Modified: Mon, 13 Dec 2021 23:33:38 GMT  
		Size: 106.2 KB (106175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd51454d9ccb4b2c45d67f47ef434c1111d07f10a4502ddb25b41d21a703bf6e`  
		Last Modified: Mon, 13 Dec 2021 23:33:31 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5695bf6599536a4097d1ad27fd3485e5f7d961b8284d08f26d44f4b6bd22f1e`  
		Last Modified: Mon, 13 Dec 2021 23:33:23 GMT  
		Size: 186.3 KB (186279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
