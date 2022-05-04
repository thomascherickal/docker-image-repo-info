<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.23`](#elasticsearch6823)
-	[`elasticsearch:7.17.3`](#elasticsearch7173)
-	[`elasticsearch:8.2.0`](#elasticsearch820)

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

## `elasticsearch:7.17.3`

```console
$ docker pull elasticsearch@sha256:5e6ac15bf6a57c42fa702a647c13749b1249c89e59be8f654f61a3feade9dc47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.17.3` - linux; amd64

```console
$ docker pull elasticsearch@sha256:7167ec15528cca7e968736c73290506082305ee72e5ecb54ec0af2700326a34e
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.2 MB (351187495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c91aa69ae062dd312fbe54fa0d3e8e306e506f4e9bfbad702ae8ebc499fe7f2`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Tue, 19 Apr 2022 11:42:37 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Tue, 19 Apr 2022 11:42:38 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Tue, 19 Apr 2022 11:42:38 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 19 Apr 2022 11:42:38 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 19 Apr 2022 11:42:45 GMT
COPY --chown=0:0dir:a31532899c4b8c084e83c255a37e64040476e8e3c59bccd77705e4e169c8d5a2 in /usr/share/elasticsearch 
# Tue, 19 Apr 2022 11:42:49 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Tue, 19 Apr 2022 11:42:49 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Apr 2022 11:42:49 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Apr 2022 11:42:50 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Tue, 19 Apr 2022 11:42:50 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Tue, 19 Apr 2022 11:42:50 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Tue, 19 Apr 2022 11:42:51 GMT
EXPOSE 9200 9300
# Tue, 19 Apr 2022 11:42:51 GMT
LABEL org.label-schema.build-date=2022-04-19T11:40:27.226665974Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=5ad023604c8d7416c9eb6c0eadb62b14e766caff org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.3 org.opencontainers.image.created=2022-04-19T11:40:27.226665974Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=5ad023604c8d7416c9eb6c0eadb62b14e766caff org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.3
# Tue, 19 Apr 2022 11:42:51 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Apr 2022 11:42:51 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed156f90b4db47dbe9a6297ffc441368c59d70258e03dc4e629203d2c2f9925`  
		Last Modified: Thu, 21 Apr 2022 21:45:35 GMT  
		Size: 8.8 MB (8828457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3c161c8ebdbb29cfea5b9f938a7504f364ad66aabd34a3b5c310bb52b94888`  
		Last Modified: Thu, 21 Apr 2022 21:45:34 GMT  
		Size: 4.4 KB (4362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157de9ee3c7a470bff0bf66ece81d394da05bf211b843a73f2cf04e6301e4abb`  
		Last Modified: Thu, 21 Apr 2022 21:45:58 GMT  
		Size: 313.5 MB (313480467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea187b8272b73ab6b6d819f9967de71f2720589fe2cf5ae4ca8183a23bbb4bf`  
		Last Modified: Thu, 21 Apr 2022 21:45:31 GMT  
		Size: 9.5 KB (9530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04594f99bf2efd369ef4b3a73cde25f3d50f638571145fed10a7c8deafc1f84`  
		Last Modified: Thu, 21 Apr 2022 21:45:32 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88cab9df767c378fa6634b7685dce04b1fa10a75797e958843181189a2b7885`  
		Last Modified: Thu, 21 Apr 2022 21:45:32 GMT  
		Size: 192.1 KB (192127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95579404185a842323a0e7ea7d2849e7f911a11959344e5e1a70805059e267e`  
		Last Modified: Thu, 21 Apr 2022 21:45:31 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da4afe05b7ab95d3b853c99d631aae19134116175c157792cc7edc5fa95758c`  
		Last Modified: Thu, 21 Apr 2022 21:45:31 GMT  
		Size: 103.9 KB (103867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.17.3` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:4501ca84e54db6e0a05d16bd32f1511f971185572203ec7d058a86a6d7d87a99
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.1 MB (348084170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5ea769f02490906acad218dd6d87b87a80e45e96d03de339ae2bacbcad30f5`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:59 GMT
ADD file:113ba5e7bc74d50e8d35449f8a62712359e2f00146e03eee822c28c8c6f59368 in / 
# Tue, 05 Apr 2022 22:41:00 GMT
CMD ["bash"]
# Tue, 19 Apr 2022 11:43:28 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Tue, 19 Apr 2022 11:43:29 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Tue, 19 Apr 2022 11:43:29 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 19 Apr 2022 11:43:29 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 19 Apr 2022 11:43:34 GMT
COPY --chown=0:0dir:ed3e65eef94fe7cef85882637a5b8cc2851c40aebfde55bc77037b402eb909b6 in /usr/share/elasticsearch 
# Tue, 19 Apr 2022 11:43:37 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Tue, 19 Apr 2022 11:43:37 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Apr 2022 11:43:37 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Apr 2022 11:43:38 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Tue, 19 Apr 2022 11:43:38 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Tue, 19 Apr 2022 11:43:39 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Tue, 19 Apr 2022 11:43:39 GMT
EXPOSE 9200 9300
# Tue, 19 Apr 2022 11:43:39 GMT
LABEL org.label-schema.build-date=2022-04-19T11:41:28.537638728Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=5ad023604c8d7416c9eb6c0eadb62b14e766caff org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.3 org.opencontainers.image.created=2022-04-19T11:41:28.537638728Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=5ad023604c8d7416c9eb6c0eadb62b14e766caff org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.3
# Tue, 19 Apr 2022 11:43:39 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Apr 2022 11:43:39 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:185e8a4c100571f111d924b5d4399d89f163bf95d71ce2c6a33f656a66c52f0a`  
		Last Modified: Tue, 05 Apr 2022 13:15:01 GMT  
		Size: 27.2 MB (27169393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2b4b72756270ff4b5152443c2370b33f527a8a50479acc0b6e2f77d8bb1b46`  
		Last Modified: Thu, 21 Apr 2022 22:16:44 GMT  
		Size: 8.7 MB (8656815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd30e545fe44910d8e750c6e52b47416d56480b7720d385b5fcc26780bca1fa`  
		Last Modified: Thu, 21 Apr 2022 22:16:42 GMT  
		Size: 4.4 KB (4369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662db77324df30dd42b051de8a2ac543aac1e45a7913f127f35c44d19cae6cdc`  
		Last Modified: Thu, 21 Apr 2022 22:17:09 GMT  
		Size: 312.0 MB (311952081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65480c38f8aac9945e87923640bec53b3fbb0eb5f6bc27ebbfc86a46c47ced89`  
		Last Modified: Thu, 21 Apr 2022 22:16:40 GMT  
		Size: 9.1 KB (9097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5ed093d3567b51ae35365d8f07af4340d592cf7b99204e2f4c57fbfd781c82`  
		Last Modified: Thu, 21 Apr 2022 22:16:40 GMT  
		Size: 2.0 KB (1982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96d789e0fcd72fc25936c78dc8d631708a2c51fe66e9801af73696e20fdddcb`  
		Last Modified: Thu, 21 Apr 2022 22:16:40 GMT  
		Size: 186.2 KB (186159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12beea32d34ef174ccc9cbc3815ed2c2d0c022ee11eef73487857d5e918d85c`  
		Last Modified: Thu, 21 Apr 2022 22:16:40 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7fc0dc2571965ed7372560c050043b061f93c92eb95da1596f6377137b18bf`  
		Last Modified: Thu, 21 Apr 2022 22:16:40 GMT  
		Size: 103.9 KB (103866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:8.2.0`

```console
$ docker pull elasticsearch@sha256:6bd33a35f529d349d8d385856b138d73241555abf2851287c055665494680b8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.2.0` - linux; amd64

```console
$ docker pull elasticsearch@sha256:0746955184ec8e3bffcf4c1bfb1ed6cef349941803ca0e96a55455faef7530d6
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.4 MB (574431974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f75ee9faf7183b931afb70d416647824c9b344e83905bbe7f70062b5eab91e43`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:34:59 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Wed, 20 Apr 2022 13:35:00 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Wed, 20 Apr 2022 13:35:00 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 20 Apr 2022 13:35:01 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 20 Apr 2022 13:35:15 GMT
COPY --chown=0:0dir:733df2f041cb5cacb63ffada2014b5611c3be52ce4d75bd37d82294c959f5436 in /usr/share/elasticsearch 
# Wed, 20 Apr 2022 13:35:19 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Wed, 20 Apr 2022 13:35:19 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 13:35:19 GMT
COPY file:bd241387dbc1b05c0872607dd207d3a5b10dfd812f1441a5b215a7e5436fca23 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Apr 2022 13:35:19 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Wed, 20 Apr 2022 13:35:20 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Wed, 20 Apr 2022 13:35:20 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Wed, 20 Apr 2022 13:35:20 GMT
EXPOSE 9200 9300
# Wed, 20 Apr 2022 13:35:21 GMT
LABEL org.label-schema.build-date=2022-04-20T13:32:27.787910643Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=b174af62e8dd9f4ac4d25875e9381ffe2b9282c5 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.2.0 org.opencontainers.image.created=2022-04-20T13:32:27.787910643Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=b174af62e8dd9f4ac4d25875e9381ffe2b9282c5 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.2.0
# Wed, 20 Apr 2022 13:35:21 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 13:35:21 GMT
CMD ["eswrapper"]
# Wed, 20 Apr 2022 13:35:21 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860caabdf2636b7c290f0a6f6f149e271ccee8e468f25cfb3b65f03251a47aa3`  
		Last Modified: Tue, 03 May 2022 16:27:37 GMT  
		Size: 9.4 MB (9422941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbe6bc43ac5f980e21b554aed748fd2ac7c68259a09797edd12c2f10989fb53`  
		Last Modified: Tue, 03 May 2022 16:27:32 GMT  
		Size: 4.4 KB (4367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4f6737f430d335a5c008db96f5547ddea32fbf3c906419bfebc53d2c1a0422`  
		Last Modified: Tue, 03 May 2022 16:28:29 GMT  
		Size: 536.1 MB (536130966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f01841fd3e9f3d1da68905203679f7f28073a2d467ca5eff045603beb309f3`  
		Last Modified: Tue, 03 May 2022 16:27:32 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae1e3bba0981804affa640695f0172157582323246aa3a72fe8cd078bc2f6d3`  
		Last Modified: Tue, 03 May 2022 16:27:32 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3767e40ef9c1b7365144bdd96950901266834bb63e35787a7c47e0f5817485`  
		Last Modified: Tue, 03 May 2022 16:27:32 GMT  
		Size: 191.9 KB (191867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d786dfd085d12df53d627e7a7a70be503b14e9f2a69d35c1e07a8f9bbf0ec27`  
		Last Modified: Tue, 03 May 2022 16:27:31 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce904f28ed33827923f2ce230a6f86d1ef64412583f165c24bb600d37987012`  
		Last Modified: Tue, 03 May 2022 16:27:31 GMT  
		Size: 103.9 KB (103876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.2.0` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:624e2c28b0cc2d6d6df29db11e99787596db8e8d15037810321f081f5b077e56
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.5 MB (382546257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fb72f73e4be26a7092cd19ffef5bdd30344bd250b60644c30da1a77e2f98488`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:59 GMT
ADD file:113ba5e7bc74d50e8d35449f8a62712359e2f00146e03eee822c28c8c6f59368 in / 
# Tue, 05 Apr 2022 22:41:00 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:36:37 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Wed, 20 Apr 2022 13:36:37 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Wed, 20 Apr 2022 13:36:38 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 20 Apr 2022 13:36:38 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 20 Apr 2022 13:36:43 GMT
COPY --chown=0:0dir:14abb5585e3f0d092437e84317657fce59afcd87ec30d0126e76b1d21e7728b2 in /usr/share/elasticsearch 
# Wed, 20 Apr 2022 13:36:47 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Wed, 20 Apr 2022 13:36:47 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 13:36:47 GMT
COPY file:bd241387dbc1b05c0872607dd207d3a5b10dfd812f1441a5b215a7e5436fca23 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Apr 2022 13:36:48 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Wed, 20 Apr 2022 13:36:48 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Wed, 20 Apr 2022 13:36:48 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Wed, 20 Apr 2022 13:36:48 GMT
EXPOSE 9200 9300
# Wed, 20 Apr 2022 13:36:49 GMT
LABEL org.label-schema.build-date=2022-04-20T13:34:34.842505421Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=b174af62e8dd9f4ac4d25875e9381ffe2b9282c5 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.2.0 org.opencontainers.image.created=2022-04-20T13:34:34.842505421Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=b174af62e8dd9f4ac4d25875e9381ffe2b9282c5 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.2.0
# Wed, 20 Apr 2022 13:36:49 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 13:36:49 GMT
CMD ["eswrapper"]
# Wed, 20 Apr 2022 13:36:49 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:185e8a4c100571f111d924b5d4399d89f163bf95d71ce2c6a33f656a66c52f0a`  
		Last Modified: Tue, 05 Apr 2022 13:15:01 GMT  
		Size: 27.2 MB (27169393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08916e81a2b262e63c5fe4ce31be090bfd93c1bde602463547954dadab8925df`  
		Last Modified: Wed, 04 May 2022 21:40:05 GMT  
		Size: 9.3 MB (9256968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51815c9b04fb87895a1090ec293df3cddd6c4d1aea75f6af68daebf356e91793`  
		Last Modified: Wed, 04 May 2022 21:40:03 GMT  
		Size: 4.4 KB (4376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9f9700741f53591ab73a65c106c61293c2ff428a3b7bfab69b95d91761c85e`  
		Last Modified: Wed, 04 May 2022 21:40:31 GMT  
		Size: 345.8 MB (345814534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bc63233efc7f0ff44ccf7335ce788f66bcd041f5f561edbba3750e08c24fa5`  
		Last Modified: Wed, 04 May 2022 21:40:00 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770e2eabff16c616975ab7b75787c9312f8cb9f689674e3e7aef778a24a68a1d`  
		Last Modified: Wed, 04 May 2022 21:40:00 GMT  
		Size: 1.7 KB (1721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098ebe130ce14278e8eb25328c88d1672246c4e36993d8ea8d815cd961d0d349`  
		Last Modified: Wed, 04 May 2022 21:40:00 GMT  
		Size: 185.9 KB (185890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346d8d86ff9141ed233c96ef0853d1c350d65803cf654cd929ac12e2a3ec41ff`  
		Last Modified: Wed, 04 May 2022 21:40:00 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38ab66ded2da45d547e2b6b6f132e7c2cc645617b7ea517011ed85812359e9c`  
		Last Modified: Wed, 04 May 2022 21:40:00 GMT  
		Size: 103.9 KB (103873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
