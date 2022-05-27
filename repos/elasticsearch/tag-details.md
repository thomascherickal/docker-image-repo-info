<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.23`](#elasticsearch6823)
-	[`elasticsearch:7.17.4`](#elasticsearch7174)
-	[`elasticsearch:8.2.2`](#elasticsearch822)

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

## `elasticsearch:7.17.4`

```console
$ docker pull elasticsearch@sha256:529b3cfec4354beda158c6c7f2f8015cbdc9432a48c1d63e824d6fd728f30db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.17.4` - linux; amd64

```console
$ docker pull elasticsearch@sha256:9396036d141a2bc50bfb74cba320483ade8c1d62f850faa4d41b4461e0a8fe48
```

-	Docker Version: 20.10.16
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.8 MB (356782272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d64cccab426e007ea19962deb2910114c25bb4e945ceb09c27926ff1c34a6dca`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Wed, 18 May 2022 20:14:01 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Wed, 18 May 2022 20:14:02 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Wed, 18 May 2022 20:14:02 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 18 May 2022 20:14:02 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 18 May 2022 20:14:09 GMT
COPY --chown=0:0dir:549be6b9d73a27c351f455baa31dc1ee6178243ba7007fa8dee8e3f73969de9b in /usr/share/elasticsearch 
# Wed, 18 May 2022 20:14:13 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Wed, 18 May 2022 20:14:13 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 May 2022 20:14:13 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Wed, 18 May 2022 20:14:14 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Wed, 18 May 2022 20:14:14 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Wed, 18 May 2022 20:14:15 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Wed, 18 May 2022 20:14:15 GMT
EXPOSE 9200 9300
# Wed, 18 May 2022 20:14:15 GMT
LABEL org.label-schema.build-date=2022-05-18T20:11:36.585918371Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=79878662c54c886ae89206c685d9f1051a9d6411 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.4 org.opencontainers.image.created=2022-05-18T20:11:36.585918371Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=79878662c54c886ae89206c685d9f1051a9d6411 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.4
# Wed, 18 May 2022 20:14:15 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 18 May 2022 20:14:15 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aceae0816c1b49cb7f63d9aa49e1f53fd5ccedf70454dfd9d9217e0ddf01829`  
		Last Modified: Wed, 25 May 2022 05:41:42 GMT  
		Size: 18.1 MB (18081009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f282e391d7d7f1c42a92085425c737a0b4ab56d57633b0257f6ec9fecb5c218`  
		Last Modified: Wed, 25 May 2022 05:41:39 GMT  
		Size: 4.4 KB (4360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d1c86ab271c86978c55c9a189af4eb3bd0088ff0a80d95381689fcc7eff6a8`  
		Last Modified: Wed, 25 May 2022 05:42:03 GMT  
		Size: 309.8 MB (309822759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2d02571b2b6619cfc5e3ffd5afa77e69a5b6c7e086a9a4700e89aa5a34a966`  
		Last Modified: Wed, 25 May 2022 05:41:39 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25fb4b01f643c5b7787c878b813f5e912417d715cd41b201ab28ebbd2734965e`  
		Last Modified: Wed, 25 May 2022 05:41:37 GMT  
		Size: 2.0 KB (1982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606786004049189a662f6c51433fe32773329f2fb4ba176d748cd175be0a2c0e`  
		Last Modified: Wed, 25 May 2022 05:41:37 GMT  
		Size: 192.1 KB (192132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ec7712324b21e55297cba4c0624cc6535e11b5309dae6212dab6b36505249f`  
		Last Modified: Wed, 25 May 2022 05:41:37 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5976c5411619b618cc8e6b0a1d46d2f3b5845535ecbcf9443770f6c51e8614`  
		Last Modified: Wed, 25 May 2022 05:41:37 GMT  
		Size: 103.9 KB (103864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.17.4` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:310afb0b900b01b1b09f2bca48f0b7eb7f7e62ef6ed1d9b08f25a7a868158bc4
```

-	Docker Version: 20.10.16
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.6 MB (352575853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ac99164e4b7ab458a8d3543382b5385747531ccf32848617b2b26684ac2b58`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Wed, 18 May 2022 20:16:15 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Wed, 18 May 2022 20:16:16 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Wed, 18 May 2022 20:16:16 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 18 May 2022 20:16:16 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 18 May 2022 20:16:20 GMT
COPY --chown=0:0dir:73295c4ff64e88fda921ca45a9ec688267643b9c6d62f3af207bcabbcc95a809 in /usr/share/elasticsearch 
# Wed, 18 May 2022 20:16:24 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Wed, 18 May 2022 20:16:24 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 May 2022 20:16:24 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Wed, 18 May 2022 20:16:25 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Wed, 18 May 2022 20:16:25 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Wed, 18 May 2022 20:16:26 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Wed, 18 May 2022 20:16:26 GMT
EXPOSE 9200 9300
# Wed, 18 May 2022 20:16:26 GMT
LABEL org.label-schema.build-date=2022-05-18T20:13:54.577348181Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=79878662c54c886ae89206c685d9f1051a9d6411 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.4 org.opencontainers.image.created=2022-05-18T20:13:54.577348181Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=79878662c54c886ae89206c685d9f1051a9d6411 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.4
# Wed, 18 May 2022 20:16:26 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 18 May 2022 20:16:26 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfeca47b2583f728bc6074e8af984467a9e890d8ff2e2cc54569fe53745f7a1`  
		Last Modified: Wed, 25 May 2022 17:40:56 GMT  
		Size: 16.7 MB (16731258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc138a45fc96942a2eee3aa460ed184765fa1ae9471e1ba6b4b50538d33c12e`  
		Last Modified: Wed, 25 May 2022 17:40:54 GMT  
		Size: 4.4 KB (4371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0770aba879c1a2d17504e1bac9d5fe38d86c294a0bab0920d44da83bbaff72cb`  
		Last Modified: Wed, 25 May 2022 17:41:20 GMT  
		Size: 308.4 MB (308369316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec2d6215148c5ecc813ab122741c8daaae09fdcd2f5b6446ed622ca9c961657`  
		Last Modified: Wed, 25 May 2022 17:40:51 GMT  
		Size: 9.1 KB (9097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a9b212c684ffe79573e749dac7569a7b951b8fcb7ab956dac815cb69ebf937`  
		Last Modified: Wed, 25 May 2022 17:40:51 GMT  
		Size: 2.0 KB (1981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0077c1fe93adcd113fb488696828dc20331f82bb452c5cd88d8c6ff705a2ecd`  
		Last Modified: Wed, 25 May 2022 17:40:51 GMT  
		Size: 186.2 KB (186162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57a9cfa22bef167240fc89d77533d745561cfc6d7e8d461793e6fc1f6a79220`  
		Last Modified: Wed, 25 May 2022 17:40:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddc033588d2c34315404a643898ad686b4f22f11d7f44b4720a810a5b639f89`  
		Last Modified: Wed, 25 May 2022 17:40:51 GMT  
		Size: 103.9 KB (103872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:8.2.2`

```console
$ docker pull elasticsearch@sha256:8c666cb1e76650306655b67644a01663f9c7a5422b2c51dd570524267f11ce3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.2.2` - linux; amd64

```console
$ docker pull elasticsearch@sha256:ba529600e5d761231f803feba56bb482bff047822c3e2097950db76ae67f7d60
```

-	Docker Version: 20.10.16
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.4 MB (579434599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6476fa627dfa17b1fc40d68fb1bdcbd3e785a0f9f2252ec79495c3cca6df77`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Wed, 25 May 2022 19:06:24 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Wed, 25 May 2022 19:06:25 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Wed, 25 May 2022 19:06:25 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 25 May 2022 19:06:25 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 25 May 2022 19:06:40 GMT
COPY --chown=0:0dir:d47f2eba6255b7cf98d4c18217d9db8ff67955f4ad68f0b7ac7569d39c256040 in /usr/share/elasticsearch 
# Wed, 25 May 2022 19:06:44 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Wed, 25 May 2022 19:06:44 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 19:06:44 GMT
COPY file:bd241387dbc1b05c0872607dd207d3a5b10dfd812f1441a5b215a7e5436fca23 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 May 2022 19:06:45 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Wed, 25 May 2022 19:06:45 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Wed, 25 May 2022 19:06:45 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Wed, 25 May 2022 19:06:46 GMT
EXPOSE 9200 9300
# Wed, 25 May 2022 19:06:46 GMT
LABEL org.label-schema.build-date=2022-05-25T19:03:42.257423355Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=9876968ef3c745186b94fdabd4483e01499224ef org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.2.2 org.opencontainers.image.created=2022-05-25T19:03:42.257423355Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=9876968ef3c745186b94fdabd4483e01499224ef org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.2.2
# Wed, 25 May 2022 19:06:46 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 25 May 2022 19:06:46 GMT
CMD ["eswrapper"]
# Wed, 25 May 2022 19:06:46 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960bdea6755738324fb5dacb769fb5e479106171ea812bb90f90f649f3e39bad`  
		Last Modified: Fri, 27 May 2022 00:25:11 GMT  
		Size: 18.1 MB (18080915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e8a9ab5eb5f1520ae727af5f6332c97ebfc6c1371214fa06e955679a583be3`  
		Last Modified: Fri, 27 May 2022 00:25:08 GMT  
		Size: 4.4 KB (4362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a41a1f614859fb18ee793986a044e10f6eca49438d501f98442e102db99240`  
		Last Modified: Fri, 27 May 2022 00:25:58 GMT  
		Size: 532.5 MB (532475695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f30a84c2b73b892e9ee5195d128aaca318d0be605e7649986b9e14c09d26e0d`  
		Last Modified: Fri, 27 May 2022 00:25:06 GMT  
		Size: 9.5 KB (9530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c111419937d6fef200ede4f1ef85d13f01dadcca6377c21c91704da9de14a3a`  
		Last Modified: Fri, 27 May 2022 00:25:06 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a098105ec5167a01d0a932e5bf6b7a7b0281e4afa6093f959572ffc95809faba`  
		Last Modified: Fri, 27 May 2022 00:25:06 GMT  
		Size: 191.9 KB (191867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c72f905045381fb04c5d1c63f7a05a261128a9464930bcec32f70c38d9e42f1`  
		Last Modified: Fri, 27 May 2022 00:25:06 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3d5560f6a5a7f9f104546fb1f24810d593fe677f720a65988e5b125f00918`  
		Last Modified: Fri, 27 May 2022 00:25:09 GMT  
		Size: 103.9 KB (103866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.2.2` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:349d1287270023b786b9307bb7068c7b8811496420448d288471cc28c65f796f
```

-	Docker Version: 20.10.16
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386434270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:488374d708a32b5992e5072d7dfc6a4d588288b9e5355d700bed351bf08cfd0b`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Wed, 25 May 2022 19:08:14 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Wed, 25 May 2022 19:08:15 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Wed, 25 May 2022 19:08:15 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 25 May 2022 19:08:15 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 25 May 2022 19:08:20 GMT
COPY --chown=0:0dir:0ad4010dfd564a2c6323753b79046fcd90e75b8680b40248015777452aebe525 in /usr/share/elasticsearch 
# Wed, 25 May 2022 19:08:24 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Wed, 25 May 2022 19:08:24 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 19:08:24 GMT
COPY file:bd241387dbc1b05c0872607dd207d3a5b10dfd812f1441a5b215a7e5436fca23 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 May 2022 19:08:25 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Wed, 25 May 2022 19:08:25 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Wed, 25 May 2022 19:08:26 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Wed, 25 May 2022 19:08:26 GMT
EXPOSE 9200 9300
# Wed, 25 May 2022 19:08:26 GMT
LABEL org.label-schema.build-date=2022-05-25T19:05:55.709385419Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=9876968ef3c745186b94fdabd4483e01499224ef org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.2.2 org.opencontainers.image.created=2022-05-25T19:05:55.709385419Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=9876968ef3c745186b94fdabd4483e01499224ef org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.2.2
# Wed, 25 May 2022 19:08:26 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 25 May 2022 19:08:26 GMT
CMD ["eswrapper"]
# Wed, 25 May 2022 19:08:26 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4881599dbc2acc6fe66db6664d7c865fb856d02bb0f1c89147c55a6c28c3a7f5`  
		Last Modified: Fri, 27 May 2022 00:46:18 GMT  
		Size: 16.7 MB (16731321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b28add695a637444b8b8d6b70d6b8f0f1d30934dec1bd5cfcc2d67af194d6`  
		Last Modified: Fri, 27 May 2022 00:46:16 GMT  
		Size: 4.4 KB (4372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9f772d9ba624b5410bfea50d1b67417f8a7f5bf29510ba94a91bcc4064b524`  
		Last Modified: Fri, 27 May 2022 00:46:43 GMT  
		Size: 342.2 MB (342228212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa976743c36a4abcf7ffa94ef8ed2c74613ab4f1e955b1475adf793b4b4bd6a8`  
		Last Modified: Fri, 27 May 2022 00:46:13 GMT  
		Size: 9.1 KB (9092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e10f56d497ff0d48316ec16581177a494cb14fa3294a4607ea3c0396d07f201`  
		Last Modified: Fri, 27 May 2022 00:46:13 GMT  
		Size: 1.7 KB (1720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae35a4514f1c18b1abbfd86736ea1c670f9105731681cbb6f6801d75c38a4f9`  
		Last Modified: Fri, 27 May 2022 00:46:13 GMT  
		Size: 185.9 KB (185891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29fe4c0acfc3df0817983da894a0ff4ca3513376e1e06386e5b3d2cb59a04e4`  
		Last Modified: Fri, 27 May 2022 00:46:13 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9a673932f3298ea9a5fd87fd997a308e5d6be3f2dccd240d997907f4fed432`  
		Last Modified: Fri, 27 May 2022 00:46:14 GMT  
		Size: 103.9 KB (103867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
