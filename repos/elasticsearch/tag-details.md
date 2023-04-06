<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.9`](#elasticsearch7179)
-	[`elasticsearch:8.7.0`](#elasticsearch870)

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

## `elasticsearch:8.7.0`

```console
$ docker pull elasticsearch@sha256:53e51bde90897d77fdbc53677331504bbbdcc788cb7aadcd8fe707a77733dbb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.7.0` - linux; amd64

```console
$ docker pull elasticsearch@sha256:861409a3479ce337308777570ea6caa179731c59e10181d2931a110766b0d2fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **639.6 MB (639613326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd60cca4e217c3f4d53eeee302b4b2b380c42cfd8cdcc935e9f6f25a268a3f35`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Mon, 27 Mar 2023 16:37:53 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Mon, 27 Mar 2023 16:37:55 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Mon, 27 Mar 2023 16:37:55 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 27 Mar 2023 16:37:55 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 27 Mar 2023 16:38:20 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Mon, 27 Mar 2023 16:38:20 GMT
COPY /bin/tini /bin/tini # buildkit
# Mon, 27 Mar 2023 16:38:20 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 16:38:20 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Mon, 27 Mar 2023 16:38:21 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Mon, 27 Mar 2023 16:38:21 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 27 Mar 2023 16:38:22 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 27 Mar 2023 16:38:22 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Mon, 27 Mar 2023 16:38:22 GMT
LABEL org.label-schema.build-date=2023-03-27T16:31:09.816451435Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=09520b59b6bc1057340b55750186466ea715e30e org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.7.0 org.opencontainers.image.created=2023-03-27T16:31:09.816451435Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=09520b59b6bc1057340b55750186466ea715e30e org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.7.0
# Mon, 27 Mar 2023 16:38:22 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 27 Mar 2023 16:38:22 GMT
CMD ["eswrapper"]
# Mon, 27 Mar 2023 16:38:22 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b287011f53a09c4d25c18a711552f4a62dd0f23e2f1fe3f02725f9773c40d10`  
		Last Modified: Thu, 30 Mar 2023 10:16:43 GMT  
		Size: 7.5 MB (7548376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f255bc0a54829951c5cb873430124e22c049df3abb0ce69320496827c30f8ef`  
		Last Modified: Thu, 30 Mar 2023 10:16:41 GMT  
		Size: 4.3 KB (4342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09511866c788193506723916084783dfca27ab3ad11dd755e7159c587b2bd80d`  
		Last Modified: Thu, 30 Mar 2023 10:17:44 GMT  
		Size: 603.2 MB (603178994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16c6ab898ef214b656b6c8dbd69706db41f77d0224511aeef5497fccf6ca5d0`  
		Last Modified: Thu, 30 Mar 2023 10:16:41 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc74db58581feb30398ea692fd35d7109e924657f418e7205a6ad997efe0b19`  
		Last Modified: Thu, 30 Mar 2023 10:16:41 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f8b401ffd4ace80fe7fb11c363ba38044742ec4e9ff34c8282ddf51637b810`  
		Last Modified: Thu, 30 Mar 2023 10:16:39 GMT  
		Size: 191.9 KB (191866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b2a650458898318481e9faf714a2e1d4424d9caad802486d90ed1d41381631`  
		Last Modified: Thu, 30 Mar 2023 10:16:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d64276d029733a37b2b307e5c3c4589c1825232cb6f2ffed8eeddb885d8895`  
		Last Modified: Thu, 30 Mar 2023 10:16:39 GMT  
		Size: 100.0 KB (99990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.7.0` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:a274d408fd8b69e80ea8f68606bbd991fe43e3ad336702a6d0fc612727cac526
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.3 MB (433301151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff634962ccc807d269895c852eea6d85330e084d1043d87a05f4b15365dbb15f`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Mon, 27 Mar 2023 16:38:08 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Mon, 27 Mar 2023 16:38:17 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Mon, 27 Mar 2023 16:38:20 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 27 Mar 2023 16:38:20 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 27 Mar 2023 16:38:26 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Mon, 27 Mar 2023 16:38:26 GMT
COPY /bin/tini /bin/tini # buildkit
# Mon, 27 Mar 2023 16:38:26 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 16:38:26 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Mon, 27 Mar 2023 16:38:27 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Mon, 27 Mar 2023 16:38:27 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 27 Mar 2023 16:38:29 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 27 Mar 2023 16:38:29 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Mon, 27 Mar 2023 16:38:29 GMT
LABEL org.label-schema.build-date=2023-03-27T16:31:09.816451435Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=09520b59b6bc1057340b55750186466ea715e30e org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.7.0 org.opencontainers.image.created=2023-03-27T16:31:09.816451435Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=09520b59b6bc1057340b55750186466ea715e30e org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.7.0
# Mon, 27 Mar 2023 16:38:29 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 27 Mar 2023 16:38:29 GMT
CMD ["eswrapper"]
# Mon, 27 Mar 2023 16:38:29 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44855302c38745f1a3b3d780290e05dab2d23cdbe5534ea8a53a5d0921aa9205`  
		Last Modified: Sat, 01 Apr 2023 12:47:43 GMT  
		Size: 7.4 MB (7371195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3a763928da856857c6d56abc65812b11cbf88b638ff5bbb17e6eb5833c9ecf`  
		Last Modified: Sat, 01 Apr 2023 12:47:39 GMT  
		Size: 4.4 KB (4355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272fac4b94aaccaa54a474d8e40518f620fde4842d2e29bc418b090fc33f300d`  
		Last Modified: Sat, 01 Apr 2023 12:48:23 GMT  
		Size: 398.4 MB (398432291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8826095872f5f8e078ec4604670162359f4691c01e8c3de2df034974d4480ab5`  
		Last Modified: Sat, 01 Apr 2023 12:47:34 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea570cf35ecf08b5564b4cf1b2540c10c8c5aa6fd4b36cf3789a21fc63f82e0b`  
		Last Modified: Sat, 01 Apr 2023 12:47:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cf2ef2e42ee039ce11fd07670c8d963a35caeef2fe61185515a6e7f87bbf8a`  
		Last Modified: Sat, 01 Apr 2023 12:47:35 GMT  
		Size: 185.9 KB (185896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6048523026c9447cf01be9fcc69f9d13c8aa8a28d385ba4568cce5f3731a56`  
		Last Modified: Sat, 01 Apr 2023 12:47:34 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7141c1e223096a1c598ee2b2f7d8eedf4fe4c9cf6db17293e217cb0754e7898`  
		Last Modified: Sat, 01 Apr 2023 12:47:35 GMT  
		Size: 100.0 KB (99988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
