<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.23`](#elasticsearch6823)
-	[`elasticsearch:7.17.7`](#elasticsearch7177)
-	[`elasticsearch:8.4.3`](#elasticsearch843)

## `elasticsearch:6.8.23`

```console
$ docker pull elasticsearch@sha256:deda76957c8cacc5dbf0d535fd14fe365f37d839813099bc32f26390a5e232dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `elasticsearch:6.8.23` - linux; amd64

```console
$ docker pull elasticsearch@sha256:71d4f7d890b90d277a1677d53f100139dcb39a34e9aac1138bfbf272c878a9cf
```

-	Docker Version: 20.10.10
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.7 MB (492666994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a2652c5f453b2f21ac32f841a6ed1897097741d69a1a4cc1947f58fae0d04b4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Thu, 06 Jan 2022 21:35:20 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 06 Jan 2022 21:35:21 GMT
ENV JAVA_HOME=/opt/jdk-15.0.1+9
# Thu, 06 Jan 2022 21:35:26 GMT
COPY dir:8d79ae5f21bb18379c0d92b3d252f4730fec22a4509252ec794212b8f72bd7af in /opt/jdk-15.0.1+9 
# Thu, 06 Jan 2022 21:36:34 GMT
RUN for iter in {1..10}; do yum update  --setopt=tsflags=nodocs -y &&     yum install -y  --setopt=tsflags=nodocs nc unzip wget which &&     yum clean all && exit_code=0 && break || exit_code=\$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Thu, 06 Jan 2022 21:36:38 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Thu, 06 Jan 2022 21:36:38 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 06 Jan 2022 21:36:42 GMT
COPY --chown=1000:0dir:b97ce01feda46ea896b080aa40faf3a7efc9341727b688e691ee0eac86058c3a in /usr/share/elasticsearch 
# Thu, 06 Jan 2022 21:36:43 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 21:36:44 GMT
COPY --chown=1000:0file:08193f849fc25f29db1438eff6d5c9fe1d63237aeb07a3e0009e8ba554f97c31 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Jan 2022 21:36:45 GMT
RUN chgrp 0 /usr/local/bin/docker-entrypoint.sh &&     chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Thu, 06 Jan 2022 21:36:46 GMT
EXPOSE 9200 9300
# Thu, 06 Jan 2022 21:36:46 GMT
LABEL org.label-schema.build-date=2022-01-06T21:30:50.087716Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=4f67856884ff580d8b48a858411b8c17cb0f8cdb org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=6.8.23 org.opencontainers.image.created=2022-01-06T21:30:50.087716Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=4f67856884ff580d8b48a858411b8c17cb0f8cdb org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=6.8.23
# Thu, 06 Jan 2022 21:36:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 06 Jan 2022 21:36:46 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d2262411d0f2af035c2e0f0c62814960b3e7d77eecab02eba9f97819d00d2e`  
		Last Modified: Thu, 13 Jan 2022 16:11:26 GMT  
		Size: 207.7 MB (207657716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa3bfe04943870deba40892398c3fc9d08da9825ea7953984632c74e4994bd`  
		Last Modified: Thu, 13 Jan 2022 16:11:18 GMT  
		Size: 58.2 MB (58240591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e780d91c9f56dc0a05ae8916a4e8d6738cf94ed5cf924534d41236da5fb38f`  
		Last Modified: Thu, 13 Jan 2022 16:11:06 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2471af457050139c5057c781433abadb769786df91ecbe6ed2a59b5f85e50369`  
		Last Modified: Thu, 13 Jan 2022 16:11:20 GMT  
		Size: 150.7 MB (150664745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca890dfc68d05cdbdd9a7f528fbe8707c05d71e8c0c985307da6797ad204eb49`  
		Last Modified: Thu, 13 Jan 2022 16:11:05 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd85b0b895822b5794063d98df42deeb3f0110f505b79fff7abc26f54f70a9c5`  
		Last Modified: Thu, 13 Jan 2022 16:11:05 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:7.17.7`

```console
$ docker pull elasticsearch@sha256:46735b5456419da6eeed5439fdb90c4eaf3480609f2c47757020fb7b1ac8fdf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `elasticsearch:7.17.7` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:4e456210ad045e8c2e71fc757f46da9b8b035a589caa57f6b98da92f89547641
```

-	Docker Version: 20.10.19
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.9 MB (349948977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c7d96debc9d30e6f99e98641695c8b44fe2e75d1072aa566b57dc4eed34f09`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 17 Oct 2022 19:33:09 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Mon, 17 Oct 2022 19:33:10 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Mon, 17 Oct 2022 19:33:10 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 17 Oct 2022 19:33:10 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 17 Oct 2022 19:33:15 GMT
COPY --chown=0:0dir:442b2e05fbe59277941d1b1045e3ce4d8bc3d0f01530e6cba28d90f0376b9e99 in /usr/share/elasticsearch 
# Mon, 17 Oct 2022 19:33:19 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Mon, 17 Oct 2022 19:33:19 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Oct 2022 19:33:19 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Mon, 17 Oct 2022 19:33:20 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Mon, 17 Oct 2022 19:33:20 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Mon, 17 Oct 2022 19:33:20 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Mon, 17 Oct 2022 19:33:20 GMT
EXPOSE 9200 9300
# Mon, 17 Oct 2022 19:33:20 GMT
LABEL org.label-schema.build-date=2022-10-17T19:31:01.853349037Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=78dcaaa8cee33438b91eca7f5c7f56a70fec9e80 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.7 org.opencontainers.image.created=2022-10-17T19:31:01.853349037Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=78dcaaa8cee33438b91eca7f5c7f56a70fec9e80 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.7
# Mon, 17 Oct 2022 19:33:21 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 17 Oct 2022 19:33:21 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb772f3aa0b7617c189a791b2626db6ca7a36379e6cd3af495f9e682f516a0`  
		Last Modified: Wed, 26 Oct 2022 20:23:16 GMT  
		Size: 7.7 MB (7654532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958897edaf7ac53f4443dd9fe18860d100d0f8ac7e9958ad2965cb597be92881`  
		Last Modified: Wed, 26 Oct 2022 20:23:15 GMT  
		Size: 4.4 KB (4363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08fedfc6594de363c61df1d412c4533e6ae78de3640bf2c8de9064446f28dcd`  
		Last Modified: Wed, 26 Oct 2022 20:23:35 GMT  
		Size: 314.8 MB (314798397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7564d3ff4f93c09c8c094b098b259b546ed7032074c9ba6ce3636354361b9277`  
		Last Modified: Wed, 26 Oct 2022 20:23:12 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951a2253715ab74b864db039e653e96d381a03f938e1ace36fb6b8a0b089c651`  
		Last Modified: Wed, 26 Oct 2022 20:23:12 GMT  
		Size: 2.0 KB (1981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38386a5ad2f6acf32792485561084b4902d9bdce427d4485edc8bb0c4ecf1547`  
		Last Modified: Wed, 26 Oct 2022 20:23:13 GMT  
		Size: 186.2 KB (186159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176a4f233e2115c55ccb247c52ef765372a0d5372a870a9d6498461f2e634137`  
		Last Modified: Wed, 26 Oct 2022 20:23:13 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457203fd2aa311a6924dd7e9cad32897e48cf13c3be7c47d7ae49cd06dadfdc6`  
		Last Modified: Wed, 26 Oct 2022 20:23:17 GMT  
		Size: 102.4 KB (102418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:8.4.3`

```console
$ docker pull elasticsearch@sha256:bb72a5788e156171b111d2fc21825d007f235c3314295aa86d0ef500678923bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.4.3` - linux; amd64

```console
$ docker pull elasticsearch@sha256:d1fe8c4c2aeeee3014dba964a5c35bc6a0da96ce436e534183645ffdd5692491
```

-	Docker Version: 20.10.18
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.0 MB (609970700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce2b9dc7fe85c774b88db460a07fbf299e45136c41d5e14287b6dec806a851a3`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 10:38:17 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Tue, 04 Oct 2022 10:38:18 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Tue, 04 Oct 2022 10:38:18 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 04 Oct 2022 10:38:18 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 04 Oct 2022 10:38:32 GMT
COPY --chown=0:0dir:2b4c9f6152a06e8da08453d2e93bd3a1ad936c394eecdfd1e501406f5a79ccce in /usr/share/elasticsearch 
# Tue, 04 Oct 2022 10:38:35 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Tue, 04 Oct 2022 10:38:35 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 10:38:35 GMT
COPY file:480ac78aea3a6b2b78f3489c03400c7b30d7129a2955fcf04b47c6666f033929 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 04 Oct 2022 10:38:36 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Tue, 04 Oct 2022 10:38:36 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Tue, 04 Oct 2022 10:38:37 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Tue, 04 Oct 2022 10:38:37 GMT
EXPOSE 9200 9300
# Tue, 04 Oct 2022 10:38:37 GMT
LABEL org.label-schema.build-date=2022-10-04T10:35:41.162162476Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=42f05b9372a9a4a470db3b52817899b99a76ee73 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.4.3 org.opencontainers.image.created=2022-10-04T10:35:41.162162476Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=42f05b9372a9a4a470db3b52817899b99a76ee73 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.4.3
# Tue, 04 Oct 2022 10:38:37 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 04 Oct 2022 10:38:37 GMT
CMD ["eswrapper"]
# Tue, 04 Oct 2022 10:38:38 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad25a8ce517dec967303372b7efd02d2a8a207ef7819a04639ccc95119366d09`  
		Last Modified: Thu, 06 Oct 2022 05:21:52 GMT  
		Size: 8.1 MB (8137604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bc58111791f520ac76c17e3cf7b9adcb2472e6e6b5d2fbbc8479ac654d7b05`  
		Last Modified: Thu, 06 Oct 2022 05:21:50 GMT  
		Size: 4.3 KB (4335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c030cb8b3c40d05d4c2ca43a033023a5d55dcc0dc562012cfb93e997262c86ce`  
		Last Modified: Thu, 06 Oct 2022 05:22:54 GMT  
		Size: 573.0 MB (572950123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4bbb7bdb12d40be146b39be93fcb5a9d1f8fd54c5534905d673bc9f9963921`  
		Last Modified: Thu, 06 Oct 2022 05:21:50 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061d37f045fc44f5819e3b5c6a66f977e714043d0ed0693c95d52c5dbf85639`  
		Last Modified: Thu, 06 Oct 2022 05:21:47 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c204de0d0710bab1339a66619a94d1c36580506134d48b14ef5c62af845a2d4`  
		Last Modified: Thu, 06 Oct 2022 05:21:48 GMT  
		Size: 191.9 KB (191873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43dd3e01e6720260658085b92ba646a915df0c140f5c4b29f9b0b8117e25d5d`  
		Last Modified: Thu, 06 Oct 2022 05:21:48 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828c381bc69ae5cf11d9a63f1f6d300710aee7ba219291e64ee8f84a295b5358`  
		Last Modified: Thu, 06 Oct 2022 05:21:48 GMT  
		Size: 102.4 KB (102421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.4.3` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:78b32e509491cf214c4d654a9e2c81692d858dd90c627621e45b455551ac6180
```

-	Docker Version: 20.10.18
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **405.4 MB (405417512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0856752e5da12fe3f0303eb843b907a053813f30de356013d90b651022465af`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 10:39:06 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Tue, 04 Oct 2022 10:39:06 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Tue, 04 Oct 2022 10:39:07 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 04 Oct 2022 10:39:07 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 04 Oct 2022 10:39:14 GMT
COPY --chown=0:0dir:6aa4c1395af235ddbc69b4343d666ce4bea82776bf74fb7c3addd4df70e12453 in /usr/share/elasticsearch 
# Tue, 04 Oct 2022 10:39:17 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Tue, 04 Oct 2022 10:39:17 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 10:39:17 GMT
COPY file:480ac78aea3a6b2b78f3489c03400c7b30d7129a2955fcf04b47c6666f033929 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 04 Oct 2022 10:39:18 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Tue, 04 Oct 2022 10:39:18 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Tue, 04 Oct 2022 10:39:19 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Tue, 04 Oct 2022 10:39:19 GMT
EXPOSE 9200 9300
# Tue, 04 Oct 2022 10:39:19 GMT
LABEL org.label-schema.build-date=2022-10-04T10:36:54.924853217Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=42f05b9372a9a4a470db3b52817899b99a76ee73 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.4.3 org.opencontainers.image.created=2022-10-04T10:36:54.924853217Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=42f05b9372a9a4a470db3b52817899b99a76ee73 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.4.3
# Tue, 04 Oct 2022 10:39:19 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 04 Oct 2022 10:39:20 GMT
CMD ["eswrapper"]
# Tue, 04 Oct 2022 10:39:20 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c232e33d5a311313b35f383f03b107b0be6bc3d2e3937f41003920e5606fa23d`  
		Last Modified: Thu, 06 Oct 2022 07:48:25 GMT  
		Size: 7.9 MB (7944257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16428e9cbfbb4b2ad0bc98d98f75208ee28f6ffe074acc6b7f7567f4323c67d1`  
		Last Modified: Thu, 06 Oct 2022 07:48:23 GMT  
		Size: 4.4 KB (4372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404fa9e45216104ace7869845517c6768eec549a45eec237de9d32736141c808`  
		Last Modified: Thu, 06 Oct 2022 07:48:53 GMT  
		Size: 370.0 MB (369977524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8d0487473d11bfcec6985532db6025f519d9f38edfc696ffd64cf18d5b615a`  
		Last Modified: Thu, 06 Oct 2022 07:48:21 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5376305778e0a70d16018d28b3c6181adacf06e1d07ee6efee0c55a39ca9a2b9`  
		Last Modified: Thu, 06 Oct 2022 07:48:21 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7703f2f0a73836653a7151caa80a8e8b1a9e79a9405029ea4d42b176894cbd9`  
		Last Modified: Thu, 06 Oct 2022 07:48:21 GMT  
		Size: 185.9 KB (185895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf333966726274e04861c607f12ae8f46f903dbcc0e463a6237c75979f12d3b`  
		Last Modified: Thu, 06 Oct 2022 07:48:21 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32256c1e7ee467f1b011c8d91ab36107f30d3721dc5d8f0ad442758df8e14abd`  
		Last Modified: Thu, 06 Oct 2022 07:48:21 GMT  
		Size: 102.4 KB (102420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
