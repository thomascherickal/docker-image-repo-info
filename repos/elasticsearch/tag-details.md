<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.9`](#elasticsearch7179)
-	[`elasticsearch:8.6.2`](#elasticsearch862)

## `elasticsearch:7.17.9`

```console
$ docker pull elasticsearch@sha256:e04ffd9739aa018693acb752f13c5791d15185a8c48e18a0ebd7055d1a203291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.17.9` - linux; amd64

```console
$ docker pull elasticsearch@sha256:56789f44fd8c451fdeb40a095c5089367e588c7a24e0a03cdbd6ba53ebd84649
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.8 MB (353752503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e1effda4391287fa2f751348ac771b6396e0107c2be7578f1fc5b93941eb514`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 05:40:05 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Tue, 31 Jan 2023 05:40:06 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Tue, 31 Jan 2023 05:40:06 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 31 Jan 2023 05:40:06 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 31 Jan 2023 05:40:12 GMT
COPY --chown=0:0dir:51f5868a5b50dadd2025adb7ada88ae1ef20dee4c79576d156fda50265dc2163 in /usr/share/elasticsearch 
# Tue, 31 Jan 2023 05:40:16 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Tue, 31 Jan 2023 05:40:16 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 05:40:16 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 05:40:17 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Tue, 31 Jan 2023 05:40:17 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Tue, 31 Jan 2023 05:40:18 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Tue, 31 Jan 2023 05:40:18 GMT
EXPOSE 9200 9300
# Tue, 31 Jan 2023 05:40:18 GMT
LABEL org.label-schema.build-date=2023-01-31T05:34:43.305517834Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=ef48222227ee6b9e70e502f0f0daa52435ee634d org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.9 org.opencontainers.image.created=2023-01-31T05:34:43.305517834Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=ef48222227ee6b9e70e502f0f0daa52435ee634d org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.9
# Tue, 31 Jan 2023 05:40:18 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 05:40:18 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bafa17d6585fee8b52c5aa7301d3996b83d08be2a66f352115a1bc9b5c0791c`  
		Last Modified: Fri, 03 Feb 2023 04:44:05 GMT  
		Size: 7.9 MB (7884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353eee74d0cb50e3e3b70d8bb4fd5f01b0fb4a4d60df551ea3164a758829be1b`  
		Last Modified: Fri, 03 Feb 2023 04:44:04 GMT  
		Size: 4.3 KB (4333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27b9d1798a418a0ed58a5fd8c8cacebd1ff316c8079306bb1a35dec6b257f15`  
		Last Modified: Fri, 03 Feb 2023 04:44:26 GMT  
		Size: 317.0 MB (316982903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08294d2254657a06d806ea955d6bd17fb16551624bb05add94ff9df08cca50cb`  
		Last Modified: Fri, 03 Feb 2023 04:44:04 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f207e8486f79fdd06aa643a52bf4b3a892eda0b2477d3275b0512757e437b1`  
		Last Modified: Fri, 03 Feb 2023 04:44:03 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c53a9497b4b5c5a1d17b47ba7deba33dc67a2d0e292b8467fa388b107608426`  
		Last Modified: Fri, 03 Feb 2023 04:44:03 GMT  
		Size: 192.1 KB (192137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e428e99f03989ad1fd4c38783abb84a9cd541a644dc39aad0c0f16b939dd2dee`  
		Last Modified: Fri, 03 Feb 2023 04:44:03 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353e2b73d0d51f1ebdf34ff2cfecb7dff013d121a1e3e4b86937dd3f304d5ac1`  
		Last Modified: Fri, 03 Feb 2023 04:44:03 GMT  
		Size: 100.0 KB (99981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.17.9` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:b0aaf5ceb461b1bef50225fa462aecab4eab12d1951d05f389c98116f5f5e6a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.6 MB (350632920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b82614cac80061c8ad1bfc5e693d999ee0f9cb59b02e29c535d6eba3a91ec6`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 05:40:29 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Tue, 31 Jan 2023 05:40:31 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Tue, 31 Jan 2023 05:40:31 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 31 Jan 2023 05:40:31 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 31 Jan 2023 05:40:33 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Tue, 31 Jan 2023 05:40:33 GMT
COPY /bin/tini /bin/tini # buildkit
# Tue, 31 Jan 2023 05:40:33 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 05:40:33 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Tue, 31 Jan 2023 05:40:34 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Tue, 31 Jan 2023 05:40:34 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 31 Jan 2023 05:40:35 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 31 Jan 2023 05:40:35 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Tue, 31 Jan 2023 05:40:35 GMT
LABEL org.label-schema.build-date=2023-01-31T05:34:43.305517834Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=ef48222227ee6b9e70e502f0f0daa52435ee634d org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.9 org.opencontainers.image.created=2023-01-31T05:34:43.305517834Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=ef48222227ee6b9e70e502f0f0daa52435ee634d org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.9
# Tue, 31 Jan 2023 05:40:35 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 05:40:35 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59229ceb84d042c77a4fddb180245a085a14ccd32c0ce68b0c76f7f1cfd3a50`  
		Last Modified: Tue, 07 Feb 2023 22:42:17 GMT  
		Size: 7.7 MB (7695965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e42b7f20bae103e319256e37a3023b29f6d0b5cf7a1a6f821f402228b09f4e7`  
		Last Modified: Tue, 07 Feb 2023 22:42:16 GMT  
		Size: 4.4 KB (4353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcad1c3b09c5bf862567dcf31e31f588330e0d1d99c94f57038d582b77cf537`  
		Last Modified: Tue, 07 Feb 2023 22:42:35 GMT  
		Size: 315.4 MB (315441762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ef16838dfcd51faf8c68a2f0d21b49766cfd509f8efe1714571ea64c58fa1e`  
		Last Modified: Tue, 07 Feb 2023 22:42:13 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3434ada9d99f11f53404da1d528b43e92c30072b0fe19776b0f8f15ad7230a0`  
		Last Modified: Tue, 07 Feb 2023 22:42:13 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1d2a10757cfffa944c419f7f70745c0ff447afdf06e1bb73b9055376854923`  
		Last Modified: Tue, 07 Feb 2023 22:42:13 GMT  
		Size: 186.2 KB (186161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce466df2ea588c374d130e45282047be140317c83f125b8db7599439acfd6676`  
		Last Modified: Tue, 07 Feb 2023 22:42:13 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481f37cf01bb85452377aa3c35ddae28c1e25b1a7b882cc51329e153261e600a`  
		Last Modified: Tue, 07 Feb 2023 22:42:17 GMT  
		Size: 100.0 KB (99991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:8.6.2`

```console
$ docker pull elasticsearch@sha256:93bc71907ca0e6e3b4f181e0dc850b90bb6cb2686c2778def0b8542398983c28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.6.2` - linux; amd64

```console
$ docker pull elasticsearch@sha256:58e27a304bdf15810e965acecbfb0bd455c33d86c85fe46d288495d095fb2cb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **625.3 MB (625263117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04485c81cc2d3ae1ae68e8be87f8a5043d71496332680a5b2e58664be95461c5`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Mon, 13 Feb 2023 09:42:06 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Mon, 13 Feb 2023 09:42:08 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Mon, 13 Feb 2023 09:42:08 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 13 Feb 2023 09:42:08 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 13 Feb 2023 09:42:33 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Mon, 13 Feb 2023 09:42:33 GMT
COPY /bin/tini /bin/tini # buildkit
# Mon, 13 Feb 2023 09:42:33 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Feb 2023 09:42:34 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Mon, 13 Feb 2023 09:42:35 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Mon, 13 Feb 2023 09:42:35 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Feb 2023 09:42:36 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Feb 2023 09:42:36 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Mon, 13 Feb 2023 09:42:36 GMT
LABEL org.label-schema.build-date=2023-02-13T09:35:20.314882762Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=2d58d0f136141f03239816a4e360a8d17b6d8f29 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.6.2 org.opencontainers.image.created=2023-02-13T09:35:20.314882762Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=2d58d0f136141f03239816a4e360a8d17b6d8f29 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.6.2
# Mon, 13 Feb 2023 09:42:36 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 13 Feb 2023 09:42:36 GMT
CMD ["eswrapper"]
# Mon, 13 Feb 2023 09:42:36 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f482acd67790286816234784186ff93e786103bd4fedb5f354cc4ca0610ce2a`  
		Last Modified: Fri, 17 Feb 2023 04:44:46 GMT  
		Size: 7.9 MB (7885601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c511159dc30adea69052e7cf9e72ef7b028470f073f3f652b108a30aa80193`  
		Last Modified: Fri, 17 Feb 2023 04:44:44 GMT  
		Size: 4.3 KB (4338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1119bf533ec8c791f5fc6e2c2aa0f8169d86984079b3cf295bfea04b1f1f62e3`  
		Last Modified: Fri, 17 Feb 2023 04:45:46 GMT  
		Size: 588.5 MB (588491732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a304f3d9b402474288ebe7cf8fdeeb466f4951291b95a9fda58f1207875262e7`  
		Last Modified: Fri, 17 Feb 2023 04:44:44 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759db6b51754caf426d9e6769e7700fcec49f26011d623a7a53e48cda0168e81`  
		Last Modified: Fri, 17 Feb 2023 04:44:43 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d240ef7d164ea2dd69bcd75743836ece632c6bec3c7657e0bbfb3ad3bbca77e`  
		Last Modified: Fri, 17 Feb 2023 04:44:43 GMT  
		Size: 191.9 KB (191873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff79e85e349e3cac7ed00772505f0bf95f5a9da3793be5fdce35529086466de`  
		Last Modified: Fri, 17 Feb 2023 04:44:43 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8817d57d05de7204f22d30db664dba21aa08102e666dd6d1e10e7e8567576c`  
		Last Modified: Fri, 17 Feb 2023 04:44:43 GMT  
		Size: 100.0 KB (99994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.6.2` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:d84d2364916c2a7fc901a489ba82bf9072b9557b1886b7ae5fd80d3fe2d1ca93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.6 MB (420639002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feeebb78e9cfb3c2d6db45b4ac7ae855b9c183588610755d7ab3eb4035e85f40`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Mon, 13 Feb 2023 09:42:33 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Mon, 13 Feb 2023 09:42:36 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Mon, 13 Feb 2023 09:42:36 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 13 Feb 2023 09:42:36 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 13 Feb 2023 09:42:38 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Mon, 13 Feb 2023 09:42:38 GMT
COPY /bin/tini /bin/tini # buildkit
# Mon, 13 Feb 2023 09:42:38 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Feb 2023 09:42:38 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Mon, 13 Feb 2023 09:42:40 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Mon, 13 Feb 2023 09:42:40 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Feb 2023 09:42:43 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 13 Feb 2023 09:42:43 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Mon, 13 Feb 2023 09:42:43 GMT
LABEL org.label-schema.build-date=2023-02-13T09:35:20.314882762Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=2d58d0f136141f03239816a4e360a8d17b6d8f29 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.6.2 org.opencontainers.image.created=2023-02-13T09:35:20.314882762Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=2d58d0f136141f03239816a4e360a8d17b6d8f29 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.6.2
# Mon, 13 Feb 2023 09:42:43 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 13 Feb 2023 09:42:43 GMT
CMD ["eswrapper"]
# Mon, 13 Feb 2023 09:42:43 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffd832ec8e91aebdecb8005d42477cf48761a7e670657e8e47487aebf987a46`  
		Last Modified: Wed, 22 Feb 2023 01:42:19 GMT  
		Size: 7.7 MB (7699297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff463bb80eb4ac5b4be481bde0ada72bd39368c877abb06ed92b97cccdb7734f`  
		Last Modified: Wed, 22 Feb 2023 01:42:18 GMT  
		Size: 4.4 KB (4357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628a62899f31621a9042729334933c45daba7cbe23ffbced57f3ac49cc86a553`  
		Last Modified: Wed, 22 Feb 2023 01:42:38 GMT  
		Size: 385.4 MB (385444457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980c10a354b3ab2b9231fc2fdc854735d60c0e7cd66def8f7c701d67d28dfdb`  
		Last Modified: Wed, 22 Feb 2023 01:42:15 GMT  
		Size: 9.1 KB (9098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798f80095917cd09693127f2deef8162e70c91abfc116f1a94207d6161b3980a`  
		Last Modified: Wed, 22 Feb 2023 01:42:15 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c923a39a68a0afd7d3895db99186947a78c0a69438d436870b339214399486`  
		Last Modified: Wed, 22 Feb 2023 01:42:16 GMT  
		Size: 185.9 KB (185898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6844500f55912849687ec52a9a96b07b2c94c54ac5cf78fc60134a7de9d1261c`  
		Last Modified: Wed, 22 Feb 2023 01:42:15 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925488f5d95c11087c85edfaafd12683dd180a7ace3eeb8f72efa4f09674718a`  
		Last Modified: Wed, 22 Feb 2023 01:42:17 GMT  
		Size: 100.0 KB (99990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
