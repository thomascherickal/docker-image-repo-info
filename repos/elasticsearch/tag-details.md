<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.23`](#elasticsearch6823)
-	[`elasticsearch:7.17.4`](#elasticsearch7174)
-	[`elasticsearch:8.2.1`](#elasticsearch821)

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

## `elasticsearch:8.2.1`

```console
$ docker pull elasticsearch@sha256:c443ad47448972938a477ec16fb2e5f44d3110165dd5914c3cbbc00d48621b92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.2.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:0322c53c50680cd5dbef29408c73b7ac9a4391db836832f6941119001e9abae3
```

-	Docker Version: 20.10.16
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.4 MB (579438802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d952ffb2b9f6c390645240c86f0eaf3bc11be3558fb8b213a20c28af70addfc`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Thu, 19 May 2022 19:54:14 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Thu, 19 May 2022 19:54:15 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Thu, 19 May 2022 19:54:15 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 19 May 2022 19:54:15 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 19 May 2022 19:54:29 GMT
COPY --chown=0:0dir:db8b66d7217396818b0a365d4782b7e0142963e4e6f0ccbba0e323fe7b4cb5ee in /usr/share/elasticsearch 
# Thu, 19 May 2022 19:54:33 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Thu, 19 May 2022 19:54:33 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 May 2022 19:54:33 GMT
COPY file:bd241387dbc1b05c0872607dd207d3a5b10dfd812f1441a5b215a7e5436fca23 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 May 2022 19:54:34 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Thu, 19 May 2022 19:54:34 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Thu, 19 May 2022 19:54:34 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Thu, 19 May 2022 19:54:35 GMT
EXPOSE 9200 9300
# Thu, 19 May 2022 19:54:35 GMT
LABEL org.label-schema.build-date=2022-05-19T19:51:29.681020456Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=db223507a0bd08f8e84a93e329764cc39b0043b9 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.2.1 org.opencontainers.image.created=2022-05-19T19:51:29.681020456Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=db223507a0bd08f8e84a93e329764cc39b0043b9 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.2.1
# Thu, 19 May 2022 19:54:35 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 19 May 2022 19:54:35 GMT
CMD ["eswrapper"]
# Thu, 19 May 2022 19:54:35 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7751a14d008fa4c21891201bcd262e276c27c377ad0629d3a579c2aaccb2079f`  
		Last Modified: Wed, 25 May 2022 01:57:33 GMT  
		Size: 18.1 MB (18080339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377d55dadb77fcce9929bd2cc2573cfd0983fc9f817c77cb479757336c92078d`  
		Last Modified: Wed, 25 May 2022 01:57:22 GMT  
		Size: 4.4 KB (4366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d2ac085d798273ac81cc41097f9c4b9c65a3c2245019c18ab9f9330b09026`  
		Last Modified: Wed, 25 May 2022 02:30:58 GMT  
		Size: 532.5 MB (532480480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adef96dbaa34db3d0dd41e94bb2468f2b5c501748d484374b9600580340cee0a`  
		Last Modified: Wed, 25 May 2022 01:57:22 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e3eb366f414f75d0bca5b7257206481be82f26ca662392b5c9a32cd6add1aa`  
		Last Modified: Wed, 25 May 2022 01:57:15 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401c3dc99fe2321ae4a62fb49b8cf6be30c95413aa793c4d6c4237b06c8416e7`  
		Last Modified: Wed, 25 May 2022 01:57:16 GMT  
		Size: 191.9 KB (191862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d623bcb146d4bac38beb1e1d8d2aad2ed39cd2879747500ee921c2ac50e5ecd3`  
		Last Modified: Wed, 25 May 2022 01:57:15 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86087d5cda1b0ca386b94b1b0f89ea132c3d3bcde037f80ea861ff4d83690a9f`  
		Last Modified: Wed, 25 May 2022 01:57:16 GMT  
		Size: 103.9 KB (103868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.2.1` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:e1204a1fc6e659d6ec744cd1deb42b6e777bab995a8026bdb54e9f2465c37026
```

-	Docker Version: 20.10.16
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386432149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f97ff6856bf7dc31ce1b13f7a0558623e38b3637f8aa576180d235dc14fad59`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Thu, 19 May 2022 19:24:37 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip vim-tiny zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Thu, 19 May 2022 19:24:38 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Thu, 19 May 2022 19:24:38 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 19 May 2022 19:24:38 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 19 May 2022 19:24:43 GMT
COPY --chown=0:0dir:0f579b9ad1e3a936613478241637c1528361f50352d00c060bddf7613daf5227 in /usr/share/elasticsearch 
# Thu, 19 May 2022 19:24:47 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Thu, 19 May 2022 19:24:47 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 May 2022 19:24:47 GMT
COPY file:bd241387dbc1b05c0872607dd207d3a5b10dfd812f1441a5b215a7e5436fca23 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 May 2022 19:24:48 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Thu, 19 May 2022 19:24:48 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Thu, 19 May 2022 19:24:49 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Thu, 19 May 2022 19:24:49 GMT
EXPOSE 9200 9300
# Thu, 19 May 2022 19:24:49 GMT
LABEL org.label-schema.build-date=2022-05-19T19:22:20.456009274Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=db223507a0bd08f8e84a93e329764cc39b0043b9 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.2.1 org.opencontainers.image.created=2022-05-19T19:22:20.456009274Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=db223507a0bd08f8e84a93e329764cc39b0043b9 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.2.1
# Thu, 19 May 2022 19:24:49 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 19 May 2022 19:24:49 GMT
CMD ["eswrapper"]
# Thu, 19 May 2022 19:24:49 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ef8ea9c491948517a1926f536171b968d97ddd3e3c0e32429726a5b4e79b18`  
		Last Modified: Wed, 25 May 2022 11:56:29 GMT  
		Size: 16.7 MB (16731254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d463bd3b2fc3a2bd88fc3c7f0f838d3b6d3c68ad053107f500c3f4c82f91cad6`  
		Last Modified: Wed, 25 May 2022 11:56:07 GMT  
		Size: 4.4 KB (4365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7861cdac2cb4384ff9cbfdba52f69ee21a605278d6db4882e3ac8de01b968c2`  
		Last Modified: Wed, 25 May 2022 11:59:16 GMT  
		Size: 342.2 MB (342226166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbf437bf19f4f979f007d87aed7c5f72128d61b24a4cdf65e388dadd61d51f0`  
		Last Modified: Wed, 25 May 2022 11:56:05 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d0c9a222bc67612338c2054cf950974fad37556d7867bbcc72d6e101abbf2b`  
		Last Modified: Wed, 25 May 2022 11:56:02 GMT  
		Size: 1.7 KB (1721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0370d640909e7467e649bcd9bd45198788c248d561a6a0c732ba507c2999afb`  
		Last Modified: Wed, 25 May 2022 11:56:02 GMT  
		Size: 185.9 KB (185885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03dcad015cff2438bba92dc33e7e83d8c643b0a2a7e40c09dd181bccdcf6110`  
		Last Modified: Wed, 25 May 2022 11:56:02 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2206136ef560987231c8716cd21524028c1c38f73b9f0912d6851f0927ede38`  
		Last Modified: Wed, 25 May 2022 11:56:03 GMT  
		Size: 103.9 KB (103867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
