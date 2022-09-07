<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.3`](#neo4j43)
-	[`neo4j:4.3-community`](#neo4j43-community)
-	[`neo4j:4.3-enterprise`](#neo4j43-enterprise)
-	[`neo4j:4.3.15`](#neo4j4315)
-	[`neo4j:4.3.15-community`](#neo4j4315-community)
-	[`neo4j:4.3.15-enterprise`](#neo4j4315-enterprise)
-	[`neo4j:4.3.16`](#neo4j4316)
-	[`neo4j:4.3.16-community`](#neo4j4316-community)
-	[`neo4j:4.3.16-enterprise`](#neo4j4316-enterprise)
-	[`neo4j:4.3.17`](#neo4j4317)
-	[`neo4j:4.3.17-community`](#neo4j4317-community)
-	[`neo4j:4.3.17-enterprise`](#neo4j4317-enterprise)
-	[`neo4j:4.3.18`](#neo4j4318)
-	[`neo4j:4.3.18-community`](#neo4j4318-community)
-	[`neo4j:4.3.18-enterprise`](#neo4j4318-enterprise)
-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.10`](#neo4j4410)
-	[`neo4j:4.4.10-community`](#neo4j4410-community)
-	[`neo4j:4.4.10-enterprise`](#neo4j4410-enterprise)
-	[`neo4j:4.4.11`](#neo4j4411)
-	[`neo4j:4.4.11-community`](#neo4j4411-community)
-	[`neo4j:4.4.11-enterprise`](#neo4j4411-enterprise)
-	[`neo4j:4.4.9`](#neo4j449)
-	[`neo4j:4.4.9-community`](#neo4j449-community)
-	[`neo4j:4.4.9-enterprise`](#neo4j449-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.3`

```console
$ docker pull neo4j@sha256:87bf9369b916a6f33ce72cae616752d8c335d75c96f9cb3c3997e676e6426b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3` - linux; amd64

```console
$ docker pull neo4j@sha256:028a42bf0d7e9f69b30090331d80a31039dcc797b1afee1a1e6f9f806e507d2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359746403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa4f992e93ac459b3195bbe05b55bc255d1fd85789dbc960985f9891e65577b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:33:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9148d4cb479de4a48e1dd9acdb835f4d5074d4da2dd261fb4ec8f158782d08 NEO4J_TARBALL=neo4j-community-4.3.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:33:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
# Fri, 02 Sep 2022 11:33:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:33:56 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:34:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:34:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:34:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:34:12 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:34:12 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:34:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:34:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8c2611a98c8d348a366432173936da753b7c8a50b4d0d0e10af5a0ed7356f7`  
		Last Modified: Fri, 02 Sep 2022 11:40:51 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b564462fea14402830a69547945aa7e12f30bbd05d93700b5ab69bb6bb9767d5`  
		Last Modified: Fri, 02 Sep 2022 11:40:50 GMT  
		Size: 7.6 KB (7618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab73414fb02efe097ce8053f40d7f958e44b965ce5763856b7a4af9c89b560c`  
		Last Modified: Fri, 02 Sep 2022 11:40:57 GMT  
		Size: 130.2 MB (130228557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3-community`

```console
$ docker pull neo4j@sha256:87bf9369b916a6f33ce72cae616752d8c335d75c96f9cb3c3997e676e6426b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3-community` - linux; amd64

```console
$ docker pull neo4j@sha256:028a42bf0d7e9f69b30090331d80a31039dcc797b1afee1a1e6f9f806e507d2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359746403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa4f992e93ac459b3195bbe05b55bc255d1fd85789dbc960985f9891e65577b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:33:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9148d4cb479de4a48e1dd9acdb835f4d5074d4da2dd261fb4ec8f158782d08 NEO4J_TARBALL=neo4j-community-4.3.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:33:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
# Fri, 02 Sep 2022 11:33:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:33:56 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:34:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:34:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:34:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:34:12 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:34:12 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:34:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:34:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8c2611a98c8d348a366432173936da753b7c8a50b4d0d0e10af5a0ed7356f7`  
		Last Modified: Fri, 02 Sep 2022 11:40:51 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b564462fea14402830a69547945aa7e12f30bbd05d93700b5ab69bb6bb9767d5`  
		Last Modified: Fri, 02 Sep 2022 11:40:50 GMT  
		Size: 7.6 KB (7618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab73414fb02efe097ce8053f40d7f958e44b965ce5763856b7a4af9c89b560c`  
		Last Modified: Fri, 02 Sep 2022 11:40:57 GMT  
		Size: 130.2 MB (130228557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3-enterprise`

```console
$ docker pull neo4j@sha256:eff34e32e73a216195f56b0cb573b2dca4a75f514d24b808aa41ee4fdbb5e088
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:5b00f86e90a997704636d80839e838ab4188ec51e675f4e5c6a0440a497f1846
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.2 MB (390232494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aa5e180162add094b4a1276a0edb356229cf551b3f39e38ff01e4cf28bd9793`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:34:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=061cf9efbdeb1af81a31a419d75afd9c9c922db53a54ab2d2d6cc1f1641c3081 NEO4J_TARBALL=neo4j-enterprise-4.3.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:34:16 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.17-unix.tar.gz
# Fri, 02 Sep 2022 11:34:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:34:17 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:34:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:34:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:34:29 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:34:29 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:34:30 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:34:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:34:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cbf2978291f6bf7c40a14e7bd96a5e7ebd7fbe6f6cc91f97793e18380a74e6`  
		Last Modified: Fri, 02 Sep 2022 11:41:11 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d181082b2695226c16a08adf02b382711c2f3a78a6225437f60a7f88991d99d9`  
		Last Modified: Fri, 02 Sep 2022 11:41:11 GMT  
		Size: 7.6 KB (7617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759ce96803ac39c0c4b5b2a7a9ac9d5f6f415ce55711b1d86877f81fb549ff83`  
		Last Modified: Fri, 02 Sep 2022 11:41:19 GMT  
		Size: 160.7 MB (160714647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.15`

```console
$ docker pull neo4j@sha256:9db153edec5a3745df2d93b9d574520f41177be2be0d5fbca6af03f1836ceb5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.15` - linux; amd64

```console
$ docker pull neo4j@sha256:ddb0a3d72965489dcde5f3a8a701e3833a2f6e928ab20be473c515c3816deb79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.9 MB (357879479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c19e40e93c19241dad2fafc92ef318cf8ea9f52ecb3fba1bc00bb40073a3b0`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:35:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=09bfaf1b60bc3498133ef10a7322c5edd66077e7dae0234415ef1d41c4315f36 NEO4J_TARBALL=neo4j-community-4.3.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:35:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.15-unix.tar.gz
# Fri, 02 Sep 2022 11:35:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:35:18 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:35:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:35:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:35:35 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:35:35 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:35:35 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:35:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:35:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d7a8002de4fac4d2d911674e9f33d6504c73c1f351c272aaf6b0c52871ba4d`  
		Last Modified: Fri, 02 Sep 2022 11:41:59 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472378291a21de9f4504eb3df82ca7eb5048c08a56b6f65664079ae33b3c1c4a`  
		Last Modified: Fri, 02 Sep 2022 11:41:59 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a37a2254f302686226b48759a96abc110ebd0041aedd233abe0979a41ab99bd`  
		Last Modified: Fri, 02 Sep 2022 11:42:05 GMT  
		Size: 128.4 MB (128361617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.15-community`

```console
$ docker pull neo4j@sha256:9db153edec5a3745df2d93b9d574520f41177be2be0d5fbca6af03f1836ceb5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.15-community` - linux; amd64

```console
$ docker pull neo4j@sha256:ddb0a3d72965489dcde5f3a8a701e3833a2f6e928ab20be473c515c3816deb79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.9 MB (357879479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c19e40e93c19241dad2fafc92ef318cf8ea9f52ecb3fba1bc00bb40073a3b0`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:35:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=09bfaf1b60bc3498133ef10a7322c5edd66077e7dae0234415ef1d41c4315f36 NEO4J_TARBALL=neo4j-community-4.3.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:35:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.15-unix.tar.gz
# Fri, 02 Sep 2022 11:35:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:35:18 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:35:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:35:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:35:35 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:35:35 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:35:35 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:35:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:35:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d7a8002de4fac4d2d911674e9f33d6504c73c1f351c272aaf6b0c52871ba4d`  
		Last Modified: Fri, 02 Sep 2022 11:41:59 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472378291a21de9f4504eb3df82ca7eb5048c08a56b6f65664079ae33b3c1c4a`  
		Last Modified: Fri, 02 Sep 2022 11:41:59 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a37a2254f302686226b48759a96abc110ebd0041aedd233abe0979a41ab99bd`  
		Last Modified: Fri, 02 Sep 2022 11:42:05 GMT  
		Size: 128.4 MB (128361617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.15-enterprise`

```console
$ docker pull neo4j@sha256:937ea2a10a11e6aad5cc78ad65914c2017f3790057410aeb2ab96c19cae719b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.15-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:095b0a358a7f10b0843d1847e344dad380dd8db5e2a9b286484bf38636118d48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.4 MB (388360870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbd71467c0e98f7f2727250dddc706086e94a5b893e16c61745f275ad1f05f4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:35:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=baba74056f917273932675a4a797ef5f926c433c08b230224b2d9985ae41424f NEO4J_TARBALL=neo4j-enterprise-4.3.15-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:35:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.15-unix.tar.gz
# Fri, 02 Sep 2022 11:35:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:35:42 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:35:59 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:36:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:36:00 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:36:00 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:36:00 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:36:00 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:36:00 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02967553dd75110bb4406a4aac24942f0bd17c1dbafa189e223b9e414deb7bf5`  
		Last Modified: Fri, 02 Sep 2022 11:42:15 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83dd7033dd817effbc0c1798a7a13e2880ba2678433c1ff0c844f45351c97aa9`  
		Last Modified: Fri, 02 Sep 2022 11:42:15 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4decf41074dfeab0d8c47930028e3018ff4a98d0a085113e0896f06d99d0f`  
		Last Modified: Fri, 02 Sep 2022 11:42:23 GMT  
		Size: 158.8 MB (158843019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.16`

```console
$ docker pull neo4j@sha256:ca278b353594966aa6f42a376c7b2af0ac8217f169492ec23777893ff5d6150a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.16` - linux; amd64

```console
$ docker pull neo4j@sha256:4a5f50a909bf761a64ff4d61bb3d227e637e799c3ef69408a5775c292b1da0cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.9 MB (357892009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:593920e97375be6772a800c9f3665727ebfa420e171d704c5ae89d9cf3878d5d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:34:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a51652705e4f2c443a30883a9ba25f4929b89c891c265ab26a354ee75d97c5c6 NEO4J_TARBALL=neo4j-community-4.3.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:34:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.16-unix.tar.gz
# Fri, 02 Sep 2022 11:34:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:34:34 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:34:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:34:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:34:50 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:34:50 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:34:50 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:34:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:34:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2e96d8090fc1093cc3d67799063210ce71a21fba583bedeea5e4c512102d41`  
		Last Modified: Fri, 02 Sep 2022 11:41:28 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507adde7008d0ff5177d38e59159d969168af775f18b2b5a75dac2048a7c24d0`  
		Last Modified: Fri, 02 Sep 2022 11:41:28 GMT  
		Size: 7.6 KB (7621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbf8fb9d97fb03b0f95f04a924b29f141d4a0cd3e8d0105103e93cfae915f1f`  
		Last Modified: Fri, 02 Sep 2022 11:41:35 GMT  
		Size: 128.4 MB (128374162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.16-community`

```console
$ docker pull neo4j@sha256:ca278b353594966aa6f42a376c7b2af0ac8217f169492ec23777893ff5d6150a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.16-community` - linux; amd64

```console
$ docker pull neo4j@sha256:4a5f50a909bf761a64ff4d61bb3d227e637e799c3ef69408a5775c292b1da0cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.9 MB (357892009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:593920e97375be6772a800c9f3665727ebfa420e171d704c5ae89d9cf3878d5d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:34:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a51652705e4f2c443a30883a9ba25f4929b89c891c265ab26a354ee75d97c5c6 NEO4J_TARBALL=neo4j-community-4.3.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:34:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.16-unix.tar.gz
# Fri, 02 Sep 2022 11:34:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:34:34 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:34:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:34:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:34:50 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:34:50 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:34:50 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:34:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:34:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2e96d8090fc1093cc3d67799063210ce71a21fba583bedeea5e4c512102d41`  
		Last Modified: Fri, 02 Sep 2022 11:41:28 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507adde7008d0ff5177d38e59159d969168af775f18b2b5a75dac2048a7c24d0`  
		Last Modified: Fri, 02 Sep 2022 11:41:28 GMT  
		Size: 7.6 KB (7621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbf8fb9d97fb03b0f95f04a924b29f141d4a0cd3e8d0105103e93cfae915f1f`  
		Last Modified: Fri, 02 Sep 2022 11:41:35 GMT  
		Size: 128.4 MB (128374162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.16-enterprise`

```console
$ docker pull neo4j@sha256:75fc6211e6e7f065d3bb98329c87600301340cf3222e0e5329531d1c0a2be57b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.16-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:91d294c37c48b4a7fc9bd982da1e5bfd006fa6dda7510c6f5534fd00915a7088
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.4 MB (388377188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c57097d32c2106f92501660b09d8e3e56b0239ae7b6aac49ba0ee1f02515da91`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:34:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9b5335af913c464d0b9cb0692b496cbb2682de99b556a5d7342054824e85debe NEO4J_TARBALL=neo4j-enterprise-4.3.16-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:34:53 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.16-unix.tar.gz
# Fri, 02 Sep 2022 11:34:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:34:54 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:35:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:35:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:35:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:35:12 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:35:12 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:35:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:35:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf0352f8c45f130f2bb83e1d2f18be358ccd59d92fd5f86bacbfe66f2238f0c`  
		Last Modified: Fri, 02 Sep 2022 11:41:44 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9252f21ee7835678943918c7e3185a6314c3077d40a9044a591f06b64088dc99`  
		Last Modified: Fri, 02 Sep 2022 11:41:44 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bbfbfc758f6a91fd206c2c24b37348cd21c1288e67b50b1eba2c006366321f`  
		Last Modified: Fri, 02 Sep 2022 11:41:52 GMT  
		Size: 158.9 MB (158859339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.17`

```console
$ docker pull neo4j@sha256:87bf9369b916a6f33ce72cae616752d8c335d75c96f9cb3c3997e676e6426b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.17` - linux; amd64

```console
$ docker pull neo4j@sha256:028a42bf0d7e9f69b30090331d80a31039dcc797b1afee1a1e6f9f806e507d2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359746403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa4f992e93ac459b3195bbe05b55bc255d1fd85789dbc960985f9891e65577b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:33:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9148d4cb479de4a48e1dd9acdb835f4d5074d4da2dd261fb4ec8f158782d08 NEO4J_TARBALL=neo4j-community-4.3.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:33:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
# Fri, 02 Sep 2022 11:33:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:33:56 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:34:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:34:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:34:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:34:12 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:34:12 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:34:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:34:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8c2611a98c8d348a366432173936da753b7c8a50b4d0d0e10af5a0ed7356f7`  
		Last Modified: Fri, 02 Sep 2022 11:40:51 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b564462fea14402830a69547945aa7e12f30bbd05d93700b5ab69bb6bb9767d5`  
		Last Modified: Fri, 02 Sep 2022 11:40:50 GMT  
		Size: 7.6 KB (7618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab73414fb02efe097ce8053f40d7f958e44b965ce5763856b7a4af9c89b560c`  
		Last Modified: Fri, 02 Sep 2022 11:40:57 GMT  
		Size: 130.2 MB (130228557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.17-community`

```console
$ docker pull neo4j@sha256:87bf9369b916a6f33ce72cae616752d8c335d75c96f9cb3c3997e676e6426b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.17-community` - linux; amd64

```console
$ docker pull neo4j@sha256:028a42bf0d7e9f69b30090331d80a31039dcc797b1afee1a1e6f9f806e507d2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359746403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa4f992e93ac459b3195bbe05b55bc255d1fd85789dbc960985f9891e65577b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:33:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9148d4cb479de4a48e1dd9acdb835f4d5074d4da2dd261fb4ec8f158782d08 NEO4J_TARBALL=neo4j-community-4.3.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:33:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
# Fri, 02 Sep 2022 11:33:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:33:56 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:34:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:34:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:34:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:34:12 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:34:12 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:34:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:34:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8c2611a98c8d348a366432173936da753b7c8a50b4d0d0e10af5a0ed7356f7`  
		Last Modified: Fri, 02 Sep 2022 11:40:51 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b564462fea14402830a69547945aa7e12f30bbd05d93700b5ab69bb6bb9767d5`  
		Last Modified: Fri, 02 Sep 2022 11:40:50 GMT  
		Size: 7.6 KB (7618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab73414fb02efe097ce8053f40d7f958e44b965ce5763856b7a4af9c89b560c`  
		Last Modified: Fri, 02 Sep 2022 11:40:57 GMT  
		Size: 130.2 MB (130228557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.17-enterprise`

```console
$ docker pull neo4j@sha256:eff34e32e73a216195f56b0cb573b2dca4a75f514d24b808aa41ee4fdbb5e088
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.17-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:5b00f86e90a997704636d80839e838ab4188ec51e675f4e5c6a0440a497f1846
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.2 MB (390232494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aa5e180162add094b4a1276a0edb356229cf551b3f39e38ff01e4cf28bd9793`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:34:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=061cf9efbdeb1af81a31a419d75afd9c9c922db53a54ab2d2d6cc1f1641c3081 NEO4J_TARBALL=neo4j-enterprise-4.3.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:34:16 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.17-unix.tar.gz
# Fri, 02 Sep 2022 11:34:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:34:17 GMT
COPY multi:7f654dae9c34c4836d2dba726eda4454b4ec5547ee00cb65a6d0f4e9a5ba930b in /startup/ 
# Fri, 02 Sep 2022 11:34:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:34:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:34:29 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:34:29 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:34:30 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:34:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:34:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cbf2978291f6bf7c40a14e7bd96a5e7ebd7fbe6f6cc91f97793e18380a74e6`  
		Last Modified: Fri, 02 Sep 2022 11:41:11 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d181082b2695226c16a08adf02b382711c2f3a78a6225437f60a7f88991d99d9`  
		Last Modified: Fri, 02 Sep 2022 11:41:11 GMT  
		Size: 7.6 KB (7617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759ce96803ac39c0c4b5b2a7a9ac9d5f6f415ce55711b1d86877f81fb549ff83`  
		Last Modified: Fri, 02 Sep 2022 11:41:19 GMT  
		Size: 160.7 MB (160714647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.18`

```console
$ docker pull neo4j@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `neo4j:4.3.18-community`

```console
$ docker pull neo4j@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `neo4j:4.3.18-enterprise`

```console
$ docker pull neo4j@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:418d2168b6a275345ce748b5c7a2ff3ab5011c4687c1e31cdbde9e399fc664c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:9507716bec4ca7d48ab0037255c5419266033619ff8355c2e6a44fa1b3c8fe44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.5 MB (364537914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f5876b8aa043c64234bb02803ecb6aa6a518eee4d19a076b38df6b4e34fa9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:31:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=869ecb89ce36fe457b4d4c4fcaa48fdf2f2d739c45323bd2c8ccdf09aa11abbf NEO4J_TARBALL=neo4j-community-4.4.10-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:31:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 11:31:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:31:41 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:31:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:31:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:31:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:31:55 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:31:55 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:31:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:31:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f992a8f96b44906367e7df1757bb4d1efa17bb01c3ae2d72bc9cbde7b6750`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c343745c86d04ce9eb039476b43408a016a0d79525849c203fb90828ad656`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 7.6 KB (7614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6e702c7c721e45a25e71ee1c6314bfe151cf63524beb784bc0fa536d7e00c5`  
		Last Modified: Fri, 02 Sep 2022 11:39:12 GMT  
		Size: 135.0 MB (135020071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6e23f8985f37c5f73a181ef08b97dc6f91a30dbff41169330464ff452a9818ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359689153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be5bece553e8afc0924244b8735d765220716c4e2847f7bcd37402a5e77dbce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Wed, 07 Sep 2022 18:40:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=28810daac5de4a5d5b77ce2da7d7c3da4c5ccf13288bad885b833c35b96100c8 NEO4J_TARBALL=neo4j-community-4.4.11-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 07 Sep 2022 18:40:16 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
# Wed, 07 Sep 2022 18:40:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 07 Sep 2022 18:40:19 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 07 Sep 2022 18:40:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 07 Sep 2022 18:40:30 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Sep 2022 18:40:31 GMT
WORKDIR /var/lib/neo4j
# Wed, 07 Sep 2022 18:40:32 GMT
VOLUME [/data /logs]
# Wed, 07 Sep 2022 18:40:33 GMT
EXPOSE 7473 7474 7687
# Wed, 07 Sep 2022 18:40:34 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 07 Sep 2022 18:40:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31b9357381bc63974a52b519130fc7be72ecfbaa7aa63afd7168d3b6304703`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e906c0279c826c5d1292427d9465b014b03fa4a076c06253729b6994b743bfd`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de213bd8dd684e20b128be0c029a9fabf773a7950c2a4a1c376b56d046689bb5`  
		Last Modified: Wed, 07 Sep 2022 18:42:16 GMT  
		Size: 134.7 MB (134746137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:418d2168b6a275345ce748b5c7a2ff3ab5011c4687c1e31cdbde9e399fc664c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:9507716bec4ca7d48ab0037255c5419266033619ff8355c2e6a44fa1b3c8fe44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.5 MB (364537914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f5876b8aa043c64234bb02803ecb6aa6a518eee4d19a076b38df6b4e34fa9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:31:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=869ecb89ce36fe457b4d4c4fcaa48fdf2f2d739c45323bd2c8ccdf09aa11abbf NEO4J_TARBALL=neo4j-community-4.4.10-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:31:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 11:31:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:31:41 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:31:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:31:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:31:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:31:55 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:31:55 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:31:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:31:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f992a8f96b44906367e7df1757bb4d1efa17bb01c3ae2d72bc9cbde7b6750`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c343745c86d04ce9eb039476b43408a016a0d79525849c203fb90828ad656`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 7.6 KB (7614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6e702c7c721e45a25e71ee1c6314bfe151cf63524beb784bc0fa536d7e00c5`  
		Last Modified: Fri, 02 Sep 2022 11:39:12 GMT  
		Size: 135.0 MB (135020071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6e23f8985f37c5f73a181ef08b97dc6f91a30dbff41169330464ff452a9818ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359689153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be5bece553e8afc0924244b8735d765220716c4e2847f7bcd37402a5e77dbce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Wed, 07 Sep 2022 18:40:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=28810daac5de4a5d5b77ce2da7d7c3da4c5ccf13288bad885b833c35b96100c8 NEO4J_TARBALL=neo4j-community-4.4.11-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 07 Sep 2022 18:40:16 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
# Wed, 07 Sep 2022 18:40:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 07 Sep 2022 18:40:19 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 07 Sep 2022 18:40:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 07 Sep 2022 18:40:30 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Sep 2022 18:40:31 GMT
WORKDIR /var/lib/neo4j
# Wed, 07 Sep 2022 18:40:32 GMT
VOLUME [/data /logs]
# Wed, 07 Sep 2022 18:40:33 GMT
EXPOSE 7473 7474 7687
# Wed, 07 Sep 2022 18:40:34 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 07 Sep 2022 18:40:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31b9357381bc63974a52b519130fc7be72ecfbaa7aa63afd7168d3b6304703`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e906c0279c826c5d1292427d9465b014b03fa4a076c06253729b6994b743bfd`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de213bd8dd684e20b128be0c029a9fabf773a7950c2a4a1c376b56d046689bb5`  
		Last Modified: Wed, 07 Sep 2022 18:42:16 GMT  
		Size: 134.7 MB (134746137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:6fe1cfc8a73940463d985123470cc052a3a930de1dd7b5357261355ef1620ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b83e02e921658c8ec492189caac7e537ae72b8c6e4a3ddae14f5057440fcaa07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.9 MB (460892697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1365145891c6182d3da810c57922ae329efb5a7e477221f51f32de467b9fbfb0`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:32:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=444e8b6fd366a60fe35f868b5e3ff84509113c3fcd35d5131e07dfcce8fb9c1a NEO4J_TARBALL=neo4j-enterprise-4.4.10-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:32:02 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 11:32:03 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:32:03 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:32:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:32:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:32:25 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:32:25 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:32:25 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:32:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:32:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822c16587c0146782c3aeb842f65a776604891146b177384e9289735afd2b129`  
		Last Modified: Fri, 02 Sep 2022 11:39:37 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4922a559b0c79c16dc1367661731cd424c76609443ae9cdac51588f4101f3`  
		Last Modified: Fri, 02 Sep 2022 11:39:37 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf56cbfd227b1fa82d744319dbcc90c9f96501fcf69628129a4135600dde69b`  
		Last Modified: Fri, 02 Sep 2022 11:39:48 GMT  
		Size: 231.4 MB (231374858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5a32838d7a1863e4ed0b789474dd29d5702924f47310e197c9aff721015dadde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.4 MB (456440243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cfcc68eff9bae14e803e9068acb51353765f81250b2ea2ddcb94e950121ec47`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Wed, 07 Sep 2022 18:40:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2d62050d2297db74344d3369b6ba1a7e7ae17e71f688f61f4b88c56b08e49969 NEO4J_TARBALL=neo4j-enterprise-4.4.11-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 07 Sep 2022 18:40:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.11-unix.tar.gz
# Wed, 07 Sep 2022 18:40:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.11-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 07 Sep 2022 18:40:47 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 07 Sep 2022 18:41:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 07 Sep 2022 18:41:08 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Sep 2022 18:41:08 GMT
WORKDIR /var/lib/neo4j
# Wed, 07 Sep 2022 18:41:09 GMT
VOLUME [/data /logs]
# Wed, 07 Sep 2022 18:41:10 GMT
EXPOSE 7473 7474 7687
# Wed, 07 Sep 2022 18:41:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 07 Sep 2022 18:41:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a20fc6c9b53594658e8aa6ee4ba561de29833e2c0a2e19a0128a6e574e2fd5`  
		Last Modified: Wed, 07 Sep 2022 18:42:39 GMT  
		Size: 3.8 KB (3832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ff8024eedc7611a8b914f640b6e226e89a614748cb164ae2b89fb31699e39d`  
		Last Modified: Wed, 07 Sep 2022 18:42:39 GMT  
		Size: 7.6 KB (7584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f52b4dc42b081931710c1a005440bd82b24c26a187868589c8ff42734d77581`  
		Last Modified: Wed, 07 Sep 2022 18:42:59 GMT  
		Size: 231.5 MB (231497230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.10`

```console
$ docker pull neo4j@sha256:a124ecdfdbbb8800e2c7f227bc9484e14380ea0db9b7ada4d997040c51bf8fa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.10` - linux; amd64

```console
$ docker pull neo4j@sha256:9507716bec4ca7d48ab0037255c5419266033619ff8355c2e6a44fa1b3c8fe44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.5 MB (364537914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f5876b8aa043c64234bb02803ecb6aa6a518eee4d19a076b38df6b4e34fa9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:31:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=869ecb89ce36fe457b4d4c4fcaa48fdf2f2d739c45323bd2c8ccdf09aa11abbf NEO4J_TARBALL=neo4j-community-4.4.10-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:31:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 11:31:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:31:41 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:31:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:31:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:31:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:31:55 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:31:55 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:31:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:31:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f992a8f96b44906367e7df1757bb4d1efa17bb01c3ae2d72bc9cbde7b6750`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c343745c86d04ce9eb039476b43408a016a0d79525849c203fb90828ad656`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 7.6 KB (7614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6e702c7c721e45a25e71ee1c6314bfe151cf63524beb784bc0fa536d7e00c5`  
		Last Modified: Fri, 02 Sep 2022 11:39:12 GMT  
		Size: 135.0 MB (135020071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.10` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:59c75ca94b724c88c364d6767d65a3ee76cad3d8f3838bbd6ce32a67799e09b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.6 MB (359615470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f36360118ffdeb4e7b3018673ccd482fb66a11d7507242749cdf70b790401e6b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Fri, 02 Sep 2022 09:03:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=869ecb89ce36fe457b4d4c4fcaa48fdf2f2d739c45323bd2c8ccdf09aa11abbf NEO4J_TARBALL=neo4j-community-4.4.10-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 09:03:48 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 09:03:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 09:03:51 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 09:04:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:04:03 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 09:04:03 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 09:04:04 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 09:04:05 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 09:04:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 09:04:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e7fdb1472aa6f061c775abedf23e4f16aa4ada3ef8b692cdd625e98557bf71`  
		Last Modified: Fri, 02 Sep 2022 09:08:23 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56147f5f4dad746dd94e07c52a0e2520929bfe6a1cd7b6e195c903d36e476b2`  
		Last Modified: Fri, 02 Sep 2022 09:08:23 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30184574d2881463f882baf663ca4c76a232ea5af9e428d2941bcf4a09030c71`  
		Last Modified: Fri, 02 Sep 2022 09:08:32 GMT  
		Size: 134.7 MB (134672452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.10-community`

```console
$ docker pull neo4j@sha256:a124ecdfdbbb8800e2c7f227bc9484e14380ea0db9b7ada4d997040c51bf8fa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.10-community` - linux; amd64

```console
$ docker pull neo4j@sha256:9507716bec4ca7d48ab0037255c5419266033619ff8355c2e6a44fa1b3c8fe44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.5 MB (364537914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f5876b8aa043c64234bb02803ecb6aa6a518eee4d19a076b38df6b4e34fa9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:31:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=869ecb89ce36fe457b4d4c4fcaa48fdf2f2d739c45323bd2c8ccdf09aa11abbf NEO4J_TARBALL=neo4j-community-4.4.10-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:31:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 11:31:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:31:41 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:31:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:31:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:31:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:31:55 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:31:55 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:31:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:31:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f992a8f96b44906367e7df1757bb4d1efa17bb01c3ae2d72bc9cbde7b6750`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c343745c86d04ce9eb039476b43408a016a0d79525849c203fb90828ad656`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 7.6 KB (7614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6e702c7c721e45a25e71ee1c6314bfe151cf63524beb784bc0fa536d7e00c5`  
		Last Modified: Fri, 02 Sep 2022 11:39:12 GMT  
		Size: 135.0 MB (135020071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.10-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:59c75ca94b724c88c364d6767d65a3ee76cad3d8f3838bbd6ce32a67799e09b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.6 MB (359615470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f36360118ffdeb4e7b3018673ccd482fb66a11d7507242749cdf70b790401e6b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Fri, 02 Sep 2022 09:03:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=869ecb89ce36fe457b4d4c4fcaa48fdf2f2d739c45323bd2c8ccdf09aa11abbf NEO4J_TARBALL=neo4j-community-4.4.10-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 09:03:48 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 09:03:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 09:03:51 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 09:04:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:04:03 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 09:04:03 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 09:04:04 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 09:04:05 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 09:04:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 09:04:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e7fdb1472aa6f061c775abedf23e4f16aa4ada3ef8b692cdd625e98557bf71`  
		Last Modified: Fri, 02 Sep 2022 09:08:23 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56147f5f4dad746dd94e07c52a0e2520929bfe6a1cd7b6e195c903d36e476b2`  
		Last Modified: Fri, 02 Sep 2022 09:08:23 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30184574d2881463f882baf663ca4c76a232ea5af9e428d2941bcf4a09030c71`  
		Last Modified: Fri, 02 Sep 2022 09:08:32 GMT  
		Size: 134.7 MB (134672452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.10-enterprise`

```console
$ docker pull neo4j@sha256:950eadb5d9fdd7270f34a9cdad1fb7c1536e09aed8a599bfc8900076aa164462
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.10-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b83e02e921658c8ec492189caac7e537ae72b8c6e4a3ddae14f5057440fcaa07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.9 MB (460892697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1365145891c6182d3da810c57922ae329efb5a7e477221f51f32de467b9fbfb0`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:32:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=444e8b6fd366a60fe35f868b5e3ff84509113c3fcd35d5131e07dfcce8fb9c1a NEO4J_TARBALL=neo4j-enterprise-4.4.10-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:32:02 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 11:32:03 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:32:03 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:32:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:32:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:32:25 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:32:25 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:32:25 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:32:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:32:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822c16587c0146782c3aeb842f65a776604891146b177384e9289735afd2b129`  
		Last Modified: Fri, 02 Sep 2022 11:39:37 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4922a559b0c79c16dc1367661731cd424c76609443ae9cdac51588f4101f3`  
		Last Modified: Fri, 02 Sep 2022 11:39:37 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf56cbfd227b1fa82d744319dbcc90c9f96501fcf69628129a4135600dde69b`  
		Last Modified: Fri, 02 Sep 2022 11:39:48 GMT  
		Size: 231.4 MB (231374858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.10-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f6be7a462c05c4d1faf0df203767aca4d5ae178b3646a9c2642e09ee695ca2a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.0 MB (455970092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779beec38e8fc0d9d93ef78a8cec1f74a985a23396530704f28956e73b693231`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Fri, 02 Sep 2022 09:04:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=444e8b6fd366a60fe35f868b5e3ff84509113c3fcd35d5131e07dfcce8fb9c1a NEO4J_TARBALL=neo4j-enterprise-4.4.10-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 09:04:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 09:04:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 09:04:20 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 09:04:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:04:42 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 09:04:43 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 09:04:44 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 09:04:45 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 09:04:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 09:04:47 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cd008761449169d36f5f63cce5c1a3f01f8f7c150f659a2b1b89a18f0d41b4`  
		Last Modified: Fri, 02 Sep 2022 09:09:01 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4560c50204ec4abb344230d3629a178913ab1106012984d84c65c09ea13de6`  
		Last Modified: Fri, 02 Sep 2022 09:09:01 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c81544dafcd4b067de58b2f7755dc346221ba0067a0b1b9d50b89c80536122`  
		Last Modified: Fri, 02 Sep 2022 09:09:16 GMT  
		Size: 231.0 MB (231027073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.11`

```console
$ docker pull neo4j@sha256:b24211126378ee8ecf8a497f911eb5a18aa7814fb3b75cd86484694eaf721f66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:4.4.11` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6e23f8985f37c5f73a181ef08b97dc6f91a30dbff41169330464ff452a9818ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359689153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be5bece553e8afc0924244b8735d765220716c4e2847f7bcd37402a5e77dbce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Wed, 07 Sep 2022 18:40:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=28810daac5de4a5d5b77ce2da7d7c3da4c5ccf13288bad885b833c35b96100c8 NEO4J_TARBALL=neo4j-community-4.4.11-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 07 Sep 2022 18:40:16 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
# Wed, 07 Sep 2022 18:40:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 07 Sep 2022 18:40:19 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 07 Sep 2022 18:40:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 07 Sep 2022 18:40:30 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Sep 2022 18:40:31 GMT
WORKDIR /var/lib/neo4j
# Wed, 07 Sep 2022 18:40:32 GMT
VOLUME [/data /logs]
# Wed, 07 Sep 2022 18:40:33 GMT
EXPOSE 7473 7474 7687
# Wed, 07 Sep 2022 18:40:34 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 07 Sep 2022 18:40:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31b9357381bc63974a52b519130fc7be72ecfbaa7aa63afd7168d3b6304703`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e906c0279c826c5d1292427d9465b014b03fa4a076c06253729b6994b743bfd`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de213bd8dd684e20b128be0c029a9fabf773a7950c2a4a1c376b56d046689bb5`  
		Last Modified: Wed, 07 Sep 2022 18:42:16 GMT  
		Size: 134.7 MB (134746137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.11-community`

```console
$ docker pull neo4j@sha256:b24211126378ee8ecf8a497f911eb5a18aa7814fb3b75cd86484694eaf721f66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:4.4.11-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6e23f8985f37c5f73a181ef08b97dc6f91a30dbff41169330464ff452a9818ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359689153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be5bece553e8afc0924244b8735d765220716c4e2847f7bcd37402a5e77dbce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Wed, 07 Sep 2022 18:40:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=28810daac5de4a5d5b77ce2da7d7c3da4c5ccf13288bad885b833c35b96100c8 NEO4J_TARBALL=neo4j-community-4.4.11-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 07 Sep 2022 18:40:16 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
# Wed, 07 Sep 2022 18:40:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 07 Sep 2022 18:40:19 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 07 Sep 2022 18:40:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 07 Sep 2022 18:40:30 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Sep 2022 18:40:31 GMT
WORKDIR /var/lib/neo4j
# Wed, 07 Sep 2022 18:40:32 GMT
VOLUME [/data /logs]
# Wed, 07 Sep 2022 18:40:33 GMT
EXPOSE 7473 7474 7687
# Wed, 07 Sep 2022 18:40:34 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 07 Sep 2022 18:40:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31b9357381bc63974a52b519130fc7be72ecfbaa7aa63afd7168d3b6304703`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e906c0279c826c5d1292427d9465b014b03fa4a076c06253729b6994b743bfd`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de213bd8dd684e20b128be0c029a9fabf773a7950c2a4a1c376b56d046689bb5`  
		Last Modified: Wed, 07 Sep 2022 18:42:16 GMT  
		Size: 134.7 MB (134746137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.11-enterprise`

```console
$ docker pull neo4j@sha256:4579d6f1cd384520ed92cac815e15f4a66a024a6c1db95158d75c2c116aad63a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:4.4.11-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5a32838d7a1863e4ed0b789474dd29d5702924f47310e197c9aff721015dadde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.4 MB (456440243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cfcc68eff9bae14e803e9068acb51353765f81250b2ea2ddcb94e950121ec47`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Wed, 07 Sep 2022 18:40:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2d62050d2297db74344d3369b6ba1a7e7ae17e71f688f61f4b88c56b08e49969 NEO4J_TARBALL=neo4j-enterprise-4.4.11-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 07 Sep 2022 18:40:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.11-unix.tar.gz
# Wed, 07 Sep 2022 18:40:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.11-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 07 Sep 2022 18:40:47 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 07 Sep 2022 18:41:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 07 Sep 2022 18:41:08 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Sep 2022 18:41:08 GMT
WORKDIR /var/lib/neo4j
# Wed, 07 Sep 2022 18:41:09 GMT
VOLUME [/data /logs]
# Wed, 07 Sep 2022 18:41:10 GMT
EXPOSE 7473 7474 7687
# Wed, 07 Sep 2022 18:41:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 07 Sep 2022 18:41:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a20fc6c9b53594658e8aa6ee4ba561de29833e2c0a2e19a0128a6e574e2fd5`  
		Last Modified: Wed, 07 Sep 2022 18:42:39 GMT  
		Size: 3.8 KB (3832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ff8024eedc7611a8b914f640b6e226e89a614748cb164ae2b89fb31699e39d`  
		Last Modified: Wed, 07 Sep 2022 18:42:39 GMT  
		Size: 7.6 KB (7584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f52b4dc42b081931710c1a005440bd82b24c26a187868589c8ff42734d77581`  
		Last Modified: Wed, 07 Sep 2022 18:42:59 GMT  
		Size: 231.5 MB (231497230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.9`

```console
$ docker pull neo4j@sha256:366182e04406898ceee9c4cacec06e34fc98c17160293a76c4080254c77fc85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.9` - linux; amd64

```console
$ docker pull neo4j@sha256:4522aaae3f5dcc07df83b7c97bb675b10d9a506ff5dc505f6bfe61b8846adc6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.3 MB (364344137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f33d24b034cafc112dc0cddfcb5e1d06db307c2f89a8d0e6a66f6601e47ea72`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:32:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4ee12a98d2dd819d6f08408429014b65264097a812ba5978c14836d6bbccb4a0 NEO4J_TARBALL=neo4j-community-4.4.9-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:32:30 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
# Fri, 02 Sep 2022 11:32:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:32:31 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:32:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:32:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:32:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:32:48 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:32:48 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:32:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:32:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4841f6f6d005ee3c025ee487bae7495b195c741d97b3747fbba762f65df35a95`  
		Last Modified: Fri, 02 Sep 2022 11:40:00 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3c2cce6afe083fec21b4d649da9eb5d9c6c93c03ce5d00ae34f6c85895d28d`  
		Last Modified: Fri, 02 Sep 2022 11:40:00 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a9465970effe756c5a9230a1aca4a04ac374122a166095635f96f15554257`  
		Last Modified: Fri, 02 Sep 2022 11:40:07 GMT  
		Size: 134.8 MB (134826297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.9` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6cbc6492defc4b313d419b5f5f143ee420bb4d01c29a1af975077e3d9091c685
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.4 MB (359421326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac627194b05572cdd0b792ee7b638c594546c9ff10a2198926be591729e4c128`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Fri, 02 Sep 2022 09:04:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4ee12a98d2dd819d6f08408429014b65264097a812ba5978c14836d6bbccb4a0 NEO4J_TARBALL=neo4j-community-4.4.9-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 09:04:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
# Fri, 02 Sep 2022 09:04:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 09:04:57 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 09:05:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:05:14 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 09:05:14 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 09:05:15 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 09:05:16 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 09:05:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 09:05:18 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a684d54c45848a71ed1a85dabce21c31fe6e8e86a0f15a66a549b53fdd92727`  
		Last Modified: Fri, 02 Sep 2022 09:09:30 GMT  
		Size: 3.8 KB (3833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925e9fb7260e9b1fa482c13ad3809e746c030465a9c78ee5129fad6bf6dc8f6c`  
		Last Modified: Fri, 02 Sep 2022 09:09:30 GMT  
		Size: 7.6 KB (7586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50177bb24fda171a7625af273f76d30b481638e88f4e0afc2a630fbdb98a5b5`  
		Last Modified: Fri, 02 Sep 2022 09:09:39 GMT  
		Size: 134.5 MB (134478310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.9-community`

```console
$ docker pull neo4j@sha256:366182e04406898ceee9c4cacec06e34fc98c17160293a76c4080254c77fc85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.9-community` - linux; amd64

```console
$ docker pull neo4j@sha256:4522aaae3f5dcc07df83b7c97bb675b10d9a506ff5dc505f6bfe61b8846adc6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.3 MB (364344137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f33d24b034cafc112dc0cddfcb5e1d06db307c2f89a8d0e6a66f6601e47ea72`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:32:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4ee12a98d2dd819d6f08408429014b65264097a812ba5978c14836d6bbccb4a0 NEO4J_TARBALL=neo4j-community-4.4.9-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:32:30 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
# Fri, 02 Sep 2022 11:32:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:32:31 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:32:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:32:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:32:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:32:48 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:32:48 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:32:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:32:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4841f6f6d005ee3c025ee487bae7495b195c741d97b3747fbba762f65df35a95`  
		Last Modified: Fri, 02 Sep 2022 11:40:00 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3c2cce6afe083fec21b4d649da9eb5d9c6c93c03ce5d00ae34f6c85895d28d`  
		Last Modified: Fri, 02 Sep 2022 11:40:00 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a9465970effe756c5a9230a1aca4a04ac374122a166095635f96f15554257`  
		Last Modified: Fri, 02 Sep 2022 11:40:07 GMT  
		Size: 134.8 MB (134826297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.9-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6cbc6492defc4b313d419b5f5f143ee420bb4d01c29a1af975077e3d9091c685
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.4 MB (359421326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac627194b05572cdd0b792ee7b638c594546c9ff10a2198926be591729e4c128`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Fri, 02 Sep 2022 09:04:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4ee12a98d2dd819d6f08408429014b65264097a812ba5978c14836d6bbccb4a0 NEO4J_TARBALL=neo4j-community-4.4.9-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 09:04:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
# Fri, 02 Sep 2022 09:04:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 09:04:57 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 09:05:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.9-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:05:14 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 09:05:14 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 09:05:15 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 09:05:16 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 09:05:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 09:05:18 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a684d54c45848a71ed1a85dabce21c31fe6e8e86a0f15a66a549b53fdd92727`  
		Last Modified: Fri, 02 Sep 2022 09:09:30 GMT  
		Size: 3.8 KB (3833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925e9fb7260e9b1fa482c13ad3809e746c030465a9c78ee5129fad6bf6dc8f6c`  
		Last Modified: Fri, 02 Sep 2022 09:09:30 GMT  
		Size: 7.6 KB (7586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50177bb24fda171a7625af273f76d30b481638e88f4e0afc2a630fbdb98a5b5`  
		Last Modified: Fri, 02 Sep 2022 09:09:39 GMT  
		Size: 134.5 MB (134478310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.9-enterprise`

```console
$ docker pull neo4j@sha256:d2dcfe1ab497006c2a9b49c04d7f9f7ea0fff7e0cae860d1cfecf80b6b7ecdf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.9-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:cfafc09309c0f76b7f79b2f119db6be6ab5bb3717aaf4a2ef5021b25aa3866f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.5 MB (456523263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a855ec6244e3bbf98d6d0018b305ad187ebf874031448a3d137e2697efe1cb2`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:32:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=747b2e71b273d8f0dd82cdb594aca02b87f03f445d2ee5eaba561c8ebd474bb0 NEO4J_TARBALL=neo4j-enterprise-4.4.9-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:32:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.9-unix.tar.gz
# Fri, 02 Sep 2022 11:32:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.9-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:32:55 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:33:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.9-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:33:17 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:33:17 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:33:18 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:33:18 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:33:18 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:33:18 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b2de4f6026930abd4013a9597caa90577561269b8045abba9a3fbb5eac63b`  
		Last Modified: Fri, 02 Sep 2022 11:40:16 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78470fe67a2cdb8f619e164a144a8f634ed6c6c001ec83cca9249ee120ab3269`  
		Last Modified: Fri, 02 Sep 2022 11:40:16 GMT  
		Size: 7.6 KB (7608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec72fe9c75dcc35a4f0251f058ba1aa5f0c4454063b66cfc3ea5380da2f33a64`  
		Last Modified: Fri, 02 Sep 2022 11:40:27 GMT  
		Size: 227.0 MB (227005425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.9-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:94170ee8f24ed2d376e52c86e1f4f2c2ec35a1612c14419573377b4dcd075793
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **451.6 MB (451599651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35ed1a461db41ece98497adfc8bcf4b2c37896769d3967c9f9b2bb4f058aa2a9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Fri, 02 Sep 2022 09:05:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=747b2e71b273d8f0dd82cdb594aca02b87f03f445d2ee5eaba561c8ebd474bb0 NEO4J_TARBALL=neo4j-enterprise-4.4.9-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 09:05:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.9-unix.tar.gz
# Fri, 02 Sep 2022 09:05:27 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.9-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 09:05:29 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 09:05:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.9-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:05:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 09:05:50 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 09:05:51 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 09:05:52 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 09:05:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 09:05:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c429c20d79f109a4814267534e45dfda7852006ceb4da15ee4a0df1744e05324`  
		Last Modified: Fri, 02 Sep 2022 09:09:50 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35ba8ad02a9ba0302c267d52e685a092c122d6d26e8af7178de40c606f904af`  
		Last Modified: Fri, 02 Sep 2022 09:09:50 GMT  
		Size: 7.6 KB (7586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4715305ac02b1852a31dcde7b712e5fd6938d938b3105210bc2a2d0f299441`  
		Last Modified: Fri, 02 Sep 2022 09:10:05 GMT  
		Size: 226.7 MB (226656632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:418d2168b6a275345ce748b5c7a2ff3ab5011c4687c1e31cdbde9e399fc664c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:9507716bec4ca7d48ab0037255c5419266033619ff8355c2e6a44fa1b3c8fe44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.5 MB (364537914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f5876b8aa043c64234bb02803ecb6aa6a518eee4d19a076b38df6b4e34fa9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:31:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=869ecb89ce36fe457b4d4c4fcaa48fdf2f2d739c45323bd2c8ccdf09aa11abbf NEO4J_TARBALL=neo4j-community-4.4.10-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:31:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 11:31:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:31:41 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:31:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:31:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:31:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:31:55 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:31:55 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:31:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:31:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f992a8f96b44906367e7df1757bb4d1efa17bb01c3ae2d72bc9cbde7b6750`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c343745c86d04ce9eb039476b43408a016a0d79525849c203fb90828ad656`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 7.6 KB (7614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6e702c7c721e45a25e71ee1c6314bfe151cf63524beb784bc0fa536d7e00c5`  
		Last Modified: Fri, 02 Sep 2022 11:39:12 GMT  
		Size: 135.0 MB (135020071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6e23f8985f37c5f73a181ef08b97dc6f91a30dbff41169330464ff452a9818ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359689153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be5bece553e8afc0924244b8735d765220716c4e2847f7bcd37402a5e77dbce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Wed, 07 Sep 2022 18:40:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=28810daac5de4a5d5b77ce2da7d7c3da4c5ccf13288bad885b833c35b96100c8 NEO4J_TARBALL=neo4j-community-4.4.11-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 07 Sep 2022 18:40:16 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
# Wed, 07 Sep 2022 18:40:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 07 Sep 2022 18:40:19 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 07 Sep 2022 18:40:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 07 Sep 2022 18:40:30 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Sep 2022 18:40:31 GMT
WORKDIR /var/lib/neo4j
# Wed, 07 Sep 2022 18:40:32 GMT
VOLUME [/data /logs]
# Wed, 07 Sep 2022 18:40:33 GMT
EXPOSE 7473 7474 7687
# Wed, 07 Sep 2022 18:40:34 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 07 Sep 2022 18:40:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31b9357381bc63974a52b519130fc7be72ecfbaa7aa63afd7168d3b6304703`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e906c0279c826c5d1292427d9465b014b03fa4a076c06253729b6994b743bfd`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de213bd8dd684e20b128be0c029a9fabf773a7950c2a4a1c376b56d046689bb5`  
		Last Modified: Wed, 07 Sep 2022 18:42:16 GMT  
		Size: 134.7 MB (134746137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:6fe1cfc8a73940463d985123470cc052a3a930de1dd7b5357261355ef1620ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b83e02e921658c8ec492189caac7e537ae72b8c6e4a3ddae14f5057440fcaa07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.9 MB (460892697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1365145891c6182d3da810c57922ae329efb5a7e477221f51f32de467b9fbfb0`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:32:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=444e8b6fd366a60fe35f868b5e3ff84509113c3fcd35d5131e07dfcce8fb9c1a NEO4J_TARBALL=neo4j-enterprise-4.4.10-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:32:02 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 11:32:03 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:32:03 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:32:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:32:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:32:25 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:32:25 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:32:25 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:32:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:32:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822c16587c0146782c3aeb842f65a776604891146b177384e9289735afd2b129`  
		Last Modified: Fri, 02 Sep 2022 11:39:37 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4922a559b0c79c16dc1367661731cd424c76609443ae9cdac51588f4101f3`  
		Last Modified: Fri, 02 Sep 2022 11:39:37 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf56cbfd227b1fa82d744319dbcc90c9f96501fcf69628129a4135600dde69b`  
		Last Modified: Fri, 02 Sep 2022 11:39:48 GMT  
		Size: 231.4 MB (231374858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5a32838d7a1863e4ed0b789474dd29d5702924f47310e197c9aff721015dadde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.4 MB (456440243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cfcc68eff9bae14e803e9068acb51353765f81250b2ea2ddcb94e950121ec47`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Wed, 07 Sep 2022 18:40:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2d62050d2297db74344d3369b6ba1a7e7ae17e71f688f61f4b88c56b08e49969 NEO4J_TARBALL=neo4j-enterprise-4.4.11-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 07 Sep 2022 18:40:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.11-unix.tar.gz
# Wed, 07 Sep 2022 18:40:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.11-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 07 Sep 2022 18:40:47 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 07 Sep 2022 18:41:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 07 Sep 2022 18:41:08 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Sep 2022 18:41:08 GMT
WORKDIR /var/lib/neo4j
# Wed, 07 Sep 2022 18:41:09 GMT
VOLUME [/data /logs]
# Wed, 07 Sep 2022 18:41:10 GMT
EXPOSE 7473 7474 7687
# Wed, 07 Sep 2022 18:41:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 07 Sep 2022 18:41:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a20fc6c9b53594658e8aa6ee4ba561de29833e2c0a2e19a0128a6e574e2fd5`  
		Last Modified: Wed, 07 Sep 2022 18:42:39 GMT  
		Size: 3.8 KB (3832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ff8024eedc7611a8b914f640b6e226e89a614748cb164ae2b89fb31699e39d`  
		Last Modified: Wed, 07 Sep 2022 18:42:39 GMT  
		Size: 7.6 KB (7584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f52b4dc42b081931710c1a005440bd82b24c26a187868589c8ff42734d77581`  
		Last Modified: Wed, 07 Sep 2022 18:42:59 GMT  
		Size: 231.5 MB (231497230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:418d2168b6a275345ce748b5c7a2ff3ab5011c4687c1e31cdbde9e399fc664c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:9507716bec4ca7d48ab0037255c5419266033619ff8355c2e6a44fa1b3c8fe44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.5 MB (364537914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f5876b8aa043c64234bb02803ecb6aa6a518eee4d19a076b38df6b4e34fa9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:31:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=869ecb89ce36fe457b4d4c4fcaa48fdf2f2d739c45323bd2c8ccdf09aa11abbf NEO4J_TARBALL=neo4j-community-4.4.10-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:31:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 11:31:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:31:41 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:31:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:31:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:31:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:31:55 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:31:55 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:31:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:31:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f992a8f96b44906367e7df1757bb4d1efa17bb01c3ae2d72bc9cbde7b6750`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c343745c86d04ce9eb039476b43408a016a0d79525849c203fb90828ad656`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 7.6 KB (7614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6e702c7c721e45a25e71ee1c6314bfe151cf63524beb784bc0fa536d7e00c5`  
		Last Modified: Fri, 02 Sep 2022 11:39:12 GMT  
		Size: 135.0 MB (135020071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6e23f8985f37c5f73a181ef08b97dc6f91a30dbff41169330464ff452a9818ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359689153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be5bece553e8afc0924244b8735d765220716c4e2847f7bcd37402a5e77dbce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Wed, 07 Sep 2022 18:40:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=28810daac5de4a5d5b77ce2da7d7c3da4c5ccf13288bad885b833c35b96100c8 NEO4J_TARBALL=neo4j-community-4.4.11-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 07 Sep 2022 18:40:16 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
# Wed, 07 Sep 2022 18:40:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 07 Sep 2022 18:40:19 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 07 Sep 2022 18:40:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 07 Sep 2022 18:40:30 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Sep 2022 18:40:31 GMT
WORKDIR /var/lib/neo4j
# Wed, 07 Sep 2022 18:40:32 GMT
VOLUME [/data /logs]
# Wed, 07 Sep 2022 18:40:33 GMT
EXPOSE 7473 7474 7687
# Wed, 07 Sep 2022 18:40:34 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 07 Sep 2022 18:40:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31b9357381bc63974a52b519130fc7be72ecfbaa7aa63afd7168d3b6304703`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e906c0279c826c5d1292427d9465b014b03fa4a076c06253729b6994b743bfd`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de213bd8dd684e20b128be0c029a9fabf773a7950c2a4a1c376b56d046689bb5`  
		Last Modified: Wed, 07 Sep 2022 18:42:16 GMT  
		Size: 134.7 MB (134746137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
