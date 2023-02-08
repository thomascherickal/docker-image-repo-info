<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.9`](#elasticsearch7179)
-	[`elasticsearch:8.6.1`](#elasticsearch861)

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

## `elasticsearch:8.6.1`

```console
$ docker pull elasticsearch@sha256:6242ee491ce3bbdb60543ae31e095630da00a413fa7d3885966a0642734bb69d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.6.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:c4a01d0a2a76e2d371ba66615d5878e3e676a6a44e940656683896789f40b75e
```

-	Docker Version: 20.10.22
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **624.9 MB (624866245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:704e34a98f9ad33b8407232e648c0b0eb39a3bc96373926db18a71f5aa32298f`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 24 Jan 2023 21:51:01 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Tue, 24 Jan 2023 21:51:03 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Tue, 24 Jan 2023 21:51:03 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 24 Jan 2023 21:51:03 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 24 Jan 2023 21:51:17 GMT
COPY --chown=0:0dir:e28ddfbe4e96637ee1a1acbe45388bf0457b103d83bd0967c8c914a0512f3082 in /usr/share/elasticsearch 
# Tue, 24 Jan 2023 21:51:21 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Tue, 24 Jan 2023 21:51:21 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:51:21 GMT
COPY file:480ac78aea3a6b2b78f3489c03400c7b30d7129a2955fcf04b47c6666f033929 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 24 Jan 2023 21:51:22 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Tue, 24 Jan 2023 21:51:22 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Tue, 24 Jan 2023 21:51:23 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Tue, 24 Jan 2023 21:51:23 GMT
EXPOSE 9200 9300
# Tue, 24 Jan 2023 21:51:23 GMT
LABEL org.label-schema.build-date=2023-01-24T21:35:11.506992272Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=180c9830da956993e59e2cd70eb32b5e383ea42c org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.6.1 org.opencontainers.image.created=2023-01-24T21:35:11.506992272Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=180c9830da956993e59e2cd70eb32b5e383ea42c org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.6.1
# Tue, 24 Jan 2023 21:51:23 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 24 Jan 2023 21:51:23 GMT
CMD ["eswrapper"]
# Tue, 24 Jan 2023 21:51:23 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8808e7b116d86a4da8b904a22bdee12c02f26eb26b0d46023cbd858e669c7679`  
		Last Modified: Fri, 27 Jan 2023 03:03:42 GMT  
		Size: 7.5 MB (7486120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1575487a3b14b2d359cc7100068b44063390c2578726d87ebb461bf667707fc9`  
		Last Modified: Fri, 27 Jan 2023 03:03:40 GMT  
		Size: 4.3 KB (4337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12eebc573f38d46992aaeca582964e7e7eb8874dd720bfe6eb82e07f9671808`  
		Last Modified: Fri, 27 Jan 2023 03:04:30 GMT  
		Size: 588.5 MB (588495392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2336bb55b75a660d39665c44f2d6a424323514d9a4e3ad98846161c7ab67183`  
		Last Modified: Fri, 27 Jan 2023 03:03:40 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2665f0ae7e1eef8e6dbc300412bbbc96ea6e121ab9de5f22e8d322fc44a9c26`  
		Last Modified: Fri, 27 Jan 2023 03:03:40 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765d657a2677188c712474404128cb295c96b8e0bb0ebefc88738031745c7061`  
		Last Modified: Fri, 27 Jan 2023 03:03:40 GMT  
		Size: 191.9 KB (191869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b66c25b220395fb17bfeebcc2e841661bad902d7ef8c88996fc91b9e3dfbe9`  
		Last Modified: Fri, 27 Jan 2023 03:03:38 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d1b00a7353e98fa74e2cc0b9ca059a9767f0d576a883946eba4aabdbe071a`  
		Last Modified: Fri, 27 Jan 2023 03:03:38 GMT  
		Size: 100.0 KB (99985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.6.1` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:7616ae747f6139d498b6b2fdd7ce8eea2721be9f0911443be5a47c323d9193b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.2 MB (420247646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4209fba45d31ec23ff4089a63e0c61d44138377b9d4e0407595f8578f9aacf`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Tue, 24 Jan 2023 21:49:41 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Tue, 24 Jan 2023 21:49:48 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Tue, 24 Jan 2023 21:49:49 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 24 Jan 2023 21:49:49 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 24 Jan 2023 21:50:11 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Tue, 24 Jan 2023 21:50:11 GMT
COPY /bin/tini /bin/tini # buildkit
# Tue, 24 Jan 2023 21:50:11 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:50:11 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Tue, 24 Jan 2023 21:50:12 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Tue, 24 Jan 2023 21:50:12 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 24 Jan 2023 21:50:13 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 24 Jan 2023 21:50:13 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Tue, 24 Jan 2023 21:50:13 GMT
LABEL org.label-schema.build-date=2023-01-24T21:35:11.506992272Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=180c9830da956993e59e2cd70eb32b5e383ea42c org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.6.1 org.opencontainers.image.created=2023-01-24T21:35:11.506992272Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=180c9830da956993e59e2cd70eb32b5e383ea42c org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.6.1
# Tue, 24 Jan 2023 21:50:13 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 24 Jan 2023 21:50:13 GMT
CMD ["eswrapper"]
# Tue, 24 Jan 2023 21:50:13 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f825be296d963da2d39bcf9a9d1a0ff6634ba1e14e7fc2aa7eb211dc53413fe`  
		Last Modified: Wed, 01 Feb 2023 22:05:39 GMT  
		Size: 7.3 MB (7305871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a451ffab41d6df7995adac6fe7a8f7f05f392b1ecddb1bfcf10bfaa6f66838e`  
		Last Modified: Wed, 01 Feb 2023 22:05:37 GMT  
		Size: 4.4 KB (4361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2d7b82311048c3fb0fe92d1f0a9d6bcdf04ca06a710752c84a0c854d19f1bf`  
		Last Modified: Wed, 01 Feb 2023 22:05:58 GMT  
		Size: 385.4 MB (385447098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f636ddc069b8c468096c90966d0db1d27df7256a044d80ccc534b9d7ec0278fc`  
		Last Modified: Wed, 01 Feb 2023 22:05:35 GMT  
		Size: 9.1 KB (9094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e634d2b0d5c2300d7897b316a83d786b4000e6717691a800cf94a2d51dc0881`  
		Last Modified: Wed, 01 Feb 2023 22:05:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fadf00d4e1576917f9f926c63b23a0da65974f994a294b9998e071cea1cd4c`  
		Last Modified: Wed, 01 Feb 2023 22:05:35 GMT  
		Size: 185.9 KB (185896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c139e97bf357309f61490094b3d193f93d7de28d40b8cc8a17174b9924e17f54`  
		Last Modified: Wed, 01 Feb 2023 22:05:35 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c935817762c5abfbcd2c07fc983f3064411be8fe126198ca1cde85826ed4d3b4`  
		Last Modified: Wed, 01 Feb 2023 22:05:39 GMT  
		Size: 100.0 KB (99993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
