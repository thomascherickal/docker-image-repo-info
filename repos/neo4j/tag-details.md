<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.23`](#neo4j4423)
-	[`neo4j:4.4.23-community`](#neo4j4423-community)
-	[`neo4j:4.4.23-enterprise`](#neo4j4423-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-bullseye`](#neo4j5-bullseye)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-community-bullseye`](#neo4j5-community-bullseye)
-	[`neo4j:5-community-ubi8`](#neo4j5-community-ubi8)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5-enterprise-bullseye`](#neo4j5-enterprise-bullseye)
-	[`neo4j:5-enterprise-ubi8`](#neo4j5-enterprise-ubi8)
-	[`neo4j:5-ubi8`](#neo4j5-ubi8)
-	[`neo4j:5.10`](#neo4j510)
-	[`neo4j:5.10-bullseye`](#neo4j510-bullseye)
-	[`neo4j:5.10-community`](#neo4j510-community)
-	[`neo4j:5.10-community-bullseye`](#neo4j510-community-bullseye)
-	[`neo4j:5.10-community-ubi8`](#neo4j510-community-ubi8)
-	[`neo4j:5.10-enterprise`](#neo4j510-enterprise)
-	[`neo4j:5.10-enterprise-bullseye`](#neo4j510-enterprise-bullseye)
-	[`neo4j:5.10-enterprise-ubi8`](#neo4j510-enterprise-ubi8)
-	[`neo4j:5.10-ubi8`](#neo4j510-ubi8)
-	[`neo4j:5.10.0`](#neo4j5100)
-	[`neo4j:5.10.0-bullseye`](#neo4j5100-bullseye)
-	[`neo4j:5.10.0-community`](#neo4j5100-community)
-	[`neo4j:5.10.0-community-bullseye`](#neo4j5100-community-bullseye)
-	[`neo4j:5.10.0-community-ubi8`](#neo4j5100-community-ubi8)
-	[`neo4j:5.10.0-enterprise`](#neo4j5100-enterprise)
-	[`neo4j:5.10.0-enterprise-bullseye`](#neo4j5100-enterprise-bullseye)
-	[`neo4j:5.10.0-enterprise-ubi8`](#neo4j5100-enterprise-ubi8)
-	[`neo4j:5.10.0-ubi8`](#neo4j5100-ubi8)
-	[`neo4j:bullseye`](#neo4jbullseye)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:community-bullseye`](#neo4jcommunity-bullseye)
-	[`neo4j:community-ubi8`](#neo4jcommunity-ubi8)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:enterprise-bullseye`](#neo4jenterprise-bullseye)
-	[`neo4j:enterprise-ubi8`](#neo4jenterprise-ubi8)
-	[`neo4j:latest`](#neo4jlatest)
-	[`neo4j:ubi8`](#neo4jubi8)

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:085c2e6d3013437941c37881212dd9d3ff6ed97cc1d07b5bb668dcaf2cf6197f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:b481e162cb0e8ef1ef30320f83d19d0f89faaaf69dd34b6fc92559fd3528e424
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.5 MB (348470224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba84557d2af87b9f44856eb04742abbee733f17e42e9d586478ba4360bceac93`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 11:19:30 GMT
COPY dir:3cd19417e6ca044e31be7ef3c49c7d24f962c0f648fd205b421373092856c87f in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:20:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=85a7dfd2b7fa039b81f445cd945515c95b68ff40cf910701d38f81cd9f07b4dc NEO4J_TARBALL=neo4j-community-4.4.23-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:20:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:20:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:20:01 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:20:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:20:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:20:17 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:20:17 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:20:17 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:20:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:20:17 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099caecba99bf99b21cfbb7f1c23915fe48406202f54aa425cdb8d4341babebd`  
		Last Modified: Wed, 05 Jul 2023 11:32:56 GMT  
		Size: 198.5 MB (198549444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c13b1407cebc06b35f6f12839e83261af68a4cd54a64facfe3a08187e0144d1`  
		Last Modified: Mon, 10 Jul 2023 18:21:06 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220c02193e4eaabd08d9c8750e34cefcef513180d4e9aff719726455825fe096`  
		Last Modified: Mon, 10 Jul 2023 18:21:06 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d02ae349b47b22384f8d4cf178f92b4b521669b4653cc04114ad2b9a108e575`  
		Last Modified: Mon, 10 Jul 2023 18:21:13 GMT  
		Size: 118.5 MB (118490211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0531e2a4dd8b2e025a7c27b9cbbd618f2e58278b6408958abcbbba2387789fb3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343784443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25a1189484c3a6bfe99c97f1ce6042d5a15f6ca8673c4ea0eb40f359f1a98582`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 03:35:40 GMT
COPY dir:46f070668c95bcfc449ea3e3aa03838e4c3f9939658e6aebe91ca179e673aded in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:39:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=85a7dfd2b7fa039b81f445cd945515c95b68ff40cf910701d38f81cd9f07b4dc NEO4J_TARBALL=neo4j-community-4.4.23-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:39:45 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:39:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:39:45 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:39:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:39:59 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:39:59 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:39:59 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:39:59 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:39:59 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:39:59 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b90eb25a0fa4522274c461d519d4e554d5d39052358c321552f0848e5d55556`  
		Last Modified: Wed, 05 Jul 2023 03:46:58 GMT  
		Size: 195.3 MB (195324199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8563f02b952bac41911b94519dd19f450fb0c9334f768dfbf8a93e754637529`  
		Last Modified: Mon, 10 Jul 2023 18:40:31 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebfca2ae7d59aefb056ac70ab4d99f178634af7e9f3237dd520f0bff721113a`  
		Last Modified: Mon, 10 Jul 2023 18:40:31 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a384e0784de256ad7d54b762b5381856b45326967888ba01a5f7fc5668c5e8`  
		Last Modified: Mon, 10 Jul 2023 18:40:36 GMT  
		Size: 118.4 MB (118384077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:085c2e6d3013437941c37881212dd9d3ff6ed97cc1d07b5bb668dcaf2cf6197f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:b481e162cb0e8ef1ef30320f83d19d0f89faaaf69dd34b6fc92559fd3528e424
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.5 MB (348470224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba84557d2af87b9f44856eb04742abbee733f17e42e9d586478ba4360bceac93`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 11:19:30 GMT
COPY dir:3cd19417e6ca044e31be7ef3c49c7d24f962c0f648fd205b421373092856c87f in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:20:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=85a7dfd2b7fa039b81f445cd945515c95b68ff40cf910701d38f81cd9f07b4dc NEO4J_TARBALL=neo4j-community-4.4.23-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:20:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:20:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:20:01 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:20:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:20:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:20:17 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:20:17 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:20:17 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:20:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:20:17 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099caecba99bf99b21cfbb7f1c23915fe48406202f54aa425cdb8d4341babebd`  
		Last Modified: Wed, 05 Jul 2023 11:32:56 GMT  
		Size: 198.5 MB (198549444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c13b1407cebc06b35f6f12839e83261af68a4cd54a64facfe3a08187e0144d1`  
		Last Modified: Mon, 10 Jul 2023 18:21:06 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220c02193e4eaabd08d9c8750e34cefcef513180d4e9aff719726455825fe096`  
		Last Modified: Mon, 10 Jul 2023 18:21:06 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d02ae349b47b22384f8d4cf178f92b4b521669b4653cc04114ad2b9a108e575`  
		Last Modified: Mon, 10 Jul 2023 18:21:13 GMT  
		Size: 118.5 MB (118490211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0531e2a4dd8b2e025a7c27b9cbbd618f2e58278b6408958abcbbba2387789fb3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343784443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25a1189484c3a6bfe99c97f1ce6042d5a15f6ca8673c4ea0eb40f359f1a98582`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 03:35:40 GMT
COPY dir:46f070668c95bcfc449ea3e3aa03838e4c3f9939658e6aebe91ca179e673aded in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:39:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=85a7dfd2b7fa039b81f445cd945515c95b68ff40cf910701d38f81cd9f07b4dc NEO4J_TARBALL=neo4j-community-4.4.23-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:39:45 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:39:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:39:45 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:39:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:39:59 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:39:59 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:39:59 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:39:59 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:39:59 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:39:59 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b90eb25a0fa4522274c461d519d4e554d5d39052358c321552f0848e5d55556`  
		Last Modified: Wed, 05 Jul 2023 03:46:58 GMT  
		Size: 195.3 MB (195324199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8563f02b952bac41911b94519dd19f450fb0c9334f768dfbf8a93e754637529`  
		Last Modified: Mon, 10 Jul 2023 18:40:31 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebfca2ae7d59aefb056ac70ab4d99f178634af7e9f3237dd520f0bff721113a`  
		Last Modified: Mon, 10 Jul 2023 18:40:31 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a384e0784de256ad7d54b762b5381856b45326967888ba01a5f7fc5668c5e8`  
		Last Modified: Mon, 10 Jul 2023 18:40:36 GMT  
		Size: 118.4 MB (118384077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:fd9413c19bef1c597475420550a16f426b4d402cb988a868a16db6216d337d71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:36b142823c4ae196a4f4533742ac41aa1599d5901a3fb6ed04239d819688c2e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.8 MB (447780311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78154c1c350f32738c5c3405b83044f2bc353be441a78dce2f640772ac764bae`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 11:19:30 GMT
COPY dir:3cd19417e6ca044e31be7ef3c49c7d24f962c0f648fd205b421373092856c87f in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:20:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=77ba1ae0ffc59ff140587a7a8bcc7bb7cfb3a70fe327a37c3c0dbea700436d68 NEO4J_TARBALL=neo4j-enterprise-4.4.23-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:20:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:20:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:20:21 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:20:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:20:42 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:20:42 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:20:42 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:20:42 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:20:42 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:20:42 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099caecba99bf99b21cfbb7f1c23915fe48406202f54aa425cdb8d4341babebd`  
		Last Modified: Wed, 05 Jul 2023 11:32:56 GMT  
		Size: 198.5 MB (198549444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16697005a6eb8aa40ae566b45d4792054ba29a3f6203c46a82453cd2499293c7`  
		Last Modified: Mon, 10 Jul 2023 18:21:27 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb68b0f105c991e9d7cec49f518897602e123a4d617531483fa051d20a8d029a`  
		Last Modified: Mon, 10 Jul 2023 18:21:27 GMT  
		Size: 9.3 KB (9326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955b8a81330f91082609724b9f773e144f31763c075661a1a71ebe0d94fc1977`  
		Last Modified: Mon, 10 Jul 2023 18:21:36 GMT  
		Size: 217.8 MB (217800295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:d2671ad9c33db7c6e61924d5ce3352b8a43e4f7a40f3dc5a1198ec75a105fe78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.1 MB (443095103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9c0a93977f34511b8636b19abe71786781ffbc54e2aedd1c517c5fabe13ef7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 03:35:40 GMT
COPY dir:46f070668c95bcfc449ea3e3aa03838e4c3f9939658e6aebe91ca179e673aded in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:40:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=77ba1ae0ffc59ff140587a7a8bcc7bb7cfb3a70fe327a37c3c0dbea700436d68 NEO4J_TARBALL=neo4j-enterprise-4.4.23-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:40:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:40:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:40:01 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:40:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:40:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:40:15 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:40:15 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:40:15 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:40:15 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:40:15 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b90eb25a0fa4522274c461d519d4e554d5d39052358c321552f0848e5d55556`  
		Last Modified: Wed, 05 Jul 2023 03:46:58 GMT  
		Size: 195.3 MB (195324199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0725c443f8e4bda679cc0ac93798927e5ea62e774f0753c101df7354baf8dbd5`  
		Last Modified: Mon, 10 Jul 2023 18:40:49 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f252db47c49895d4f6ccadcbb176175b06df5c188259732bf706d6fa2a8e5c8e`  
		Last Modified: Mon, 10 Jul 2023 18:40:49 GMT  
		Size: 9.3 KB (9320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5233b4e913fc32223aada1e7209550f4202321215b3160dc8491958859324d`  
		Last Modified: Mon, 10 Jul 2023 18:40:57 GMT  
		Size: 217.7 MB (217694744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.23`

```console
$ docker pull neo4j@sha256:085c2e6d3013437941c37881212dd9d3ff6ed97cc1d07b5bb668dcaf2cf6197f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.23` - linux; amd64

```console
$ docker pull neo4j@sha256:b481e162cb0e8ef1ef30320f83d19d0f89faaaf69dd34b6fc92559fd3528e424
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.5 MB (348470224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba84557d2af87b9f44856eb04742abbee733f17e42e9d586478ba4360bceac93`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 11:19:30 GMT
COPY dir:3cd19417e6ca044e31be7ef3c49c7d24f962c0f648fd205b421373092856c87f in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:20:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=85a7dfd2b7fa039b81f445cd945515c95b68ff40cf910701d38f81cd9f07b4dc NEO4J_TARBALL=neo4j-community-4.4.23-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:20:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:20:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:20:01 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:20:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:20:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:20:17 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:20:17 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:20:17 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:20:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:20:17 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099caecba99bf99b21cfbb7f1c23915fe48406202f54aa425cdb8d4341babebd`  
		Last Modified: Wed, 05 Jul 2023 11:32:56 GMT  
		Size: 198.5 MB (198549444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c13b1407cebc06b35f6f12839e83261af68a4cd54a64facfe3a08187e0144d1`  
		Last Modified: Mon, 10 Jul 2023 18:21:06 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220c02193e4eaabd08d9c8750e34cefcef513180d4e9aff719726455825fe096`  
		Last Modified: Mon, 10 Jul 2023 18:21:06 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d02ae349b47b22384f8d4cf178f92b4b521669b4653cc04114ad2b9a108e575`  
		Last Modified: Mon, 10 Jul 2023 18:21:13 GMT  
		Size: 118.5 MB (118490211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.23` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0531e2a4dd8b2e025a7c27b9cbbd618f2e58278b6408958abcbbba2387789fb3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343784443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25a1189484c3a6bfe99c97f1ce6042d5a15f6ca8673c4ea0eb40f359f1a98582`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 03:35:40 GMT
COPY dir:46f070668c95bcfc449ea3e3aa03838e4c3f9939658e6aebe91ca179e673aded in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:39:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=85a7dfd2b7fa039b81f445cd945515c95b68ff40cf910701d38f81cd9f07b4dc NEO4J_TARBALL=neo4j-community-4.4.23-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:39:45 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:39:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:39:45 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:39:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:39:59 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:39:59 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:39:59 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:39:59 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:39:59 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:39:59 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b90eb25a0fa4522274c461d519d4e554d5d39052358c321552f0848e5d55556`  
		Last Modified: Wed, 05 Jul 2023 03:46:58 GMT  
		Size: 195.3 MB (195324199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8563f02b952bac41911b94519dd19f450fb0c9334f768dfbf8a93e754637529`  
		Last Modified: Mon, 10 Jul 2023 18:40:31 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebfca2ae7d59aefb056ac70ab4d99f178634af7e9f3237dd520f0bff721113a`  
		Last Modified: Mon, 10 Jul 2023 18:40:31 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a384e0784de256ad7d54b762b5381856b45326967888ba01a5f7fc5668c5e8`  
		Last Modified: Mon, 10 Jul 2023 18:40:36 GMT  
		Size: 118.4 MB (118384077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.23-community`

```console
$ docker pull neo4j@sha256:085c2e6d3013437941c37881212dd9d3ff6ed97cc1d07b5bb668dcaf2cf6197f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.23-community` - linux; amd64

```console
$ docker pull neo4j@sha256:b481e162cb0e8ef1ef30320f83d19d0f89faaaf69dd34b6fc92559fd3528e424
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.5 MB (348470224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba84557d2af87b9f44856eb04742abbee733f17e42e9d586478ba4360bceac93`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 11:19:30 GMT
COPY dir:3cd19417e6ca044e31be7ef3c49c7d24f962c0f648fd205b421373092856c87f in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:20:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=85a7dfd2b7fa039b81f445cd945515c95b68ff40cf910701d38f81cd9f07b4dc NEO4J_TARBALL=neo4j-community-4.4.23-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:20:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:20:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:20:01 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:20:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:20:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:20:17 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:20:17 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:20:17 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:20:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:20:17 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099caecba99bf99b21cfbb7f1c23915fe48406202f54aa425cdb8d4341babebd`  
		Last Modified: Wed, 05 Jul 2023 11:32:56 GMT  
		Size: 198.5 MB (198549444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c13b1407cebc06b35f6f12839e83261af68a4cd54a64facfe3a08187e0144d1`  
		Last Modified: Mon, 10 Jul 2023 18:21:06 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220c02193e4eaabd08d9c8750e34cefcef513180d4e9aff719726455825fe096`  
		Last Modified: Mon, 10 Jul 2023 18:21:06 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d02ae349b47b22384f8d4cf178f92b4b521669b4653cc04114ad2b9a108e575`  
		Last Modified: Mon, 10 Jul 2023 18:21:13 GMT  
		Size: 118.5 MB (118490211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.23-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0531e2a4dd8b2e025a7c27b9cbbd618f2e58278b6408958abcbbba2387789fb3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343784443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25a1189484c3a6bfe99c97f1ce6042d5a15f6ca8673c4ea0eb40f359f1a98582`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 03:35:40 GMT
COPY dir:46f070668c95bcfc449ea3e3aa03838e4c3f9939658e6aebe91ca179e673aded in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:39:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=85a7dfd2b7fa039b81f445cd945515c95b68ff40cf910701d38f81cd9f07b4dc NEO4J_TARBALL=neo4j-community-4.4.23-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:39:45 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:39:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:39:45 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:39:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:39:59 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:39:59 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:39:59 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:39:59 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:39:59 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:39:59 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b90eb25a0fa4522274c461d519d4e554d5d39052358c321552f0848e5d55556`  
		Last Modified: Wed, 05 Jul 2023 03:46:58 GMT  
		Size: 195.3 MB (195324199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8563f02b952bac41911b94519dd19f450fb0c9334f768dfbf8a93e754637529`  
		Last Modified: Mon, 10 Jul 2023 18:40:31 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebfca2ae7d59aefb056ac70ab4d99f178634af7e9f3237dd520f0bff721113a`  
		Last Modified: Mon, 10 Jul 2023 18:40:31 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a384e0784de256ad7d54b762b5381856b45326967888ba01a5f7fc5668c5e8`  
		Last Modified: Mon, 10 Jul 2023 18:40:36 GMT  
		Size: 118.4 MB (118384077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.23-enterprise`

```console
$ docker pull neo4j@sha256:fd9413c19bef1c597475420550a16f426b4d402cb988a868a16db6216d337d71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.23-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:36b142823c4ae196a4f4533742ac41aa1599d5901a3fb6ed04239d819688c2e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.8 MB (447780311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78154c1c350f32738c5c3405b83044f2bc353be441a78dce2f640772ac764bae`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 11:19:30 GMT
COPY dir:3cd19417e6ca044e31be7ef3c49c7d24f962c0f648fd205b421373092856c87f in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:20:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=77ba1ae0ffc59ff140587a7a8bcc7bb7cfb3a70fe327a37c3c0dbea700436d68 NEO4J_TARBALL=neo4j-enterprise-4.4.23-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:20:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:20:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:20:21 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:20:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:20:42 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:20:42 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:20:42 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:20:42 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:20:42 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:20:42 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099caecba99bf99b21cfbb7f1c23915fe48406202f54aa425cdb8d4341babebd`  
		Last Modified: Wed, 05 Jul 2023 11:32:56 GMT  
		Size: 198.5 MB (198549444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16697005a6eb8aa40ae566b45d4792054ba29a3f6203c46a82453cd2499293c7`  
		Last Modified: Mon, 10 Jul 2023 18:21:27 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb68b0f105c991e9d7cec49f518897602e123a4d617531483fa051d20a8d029a`  
		Last Modified: Mon, 10 Jul 2023 18:21:27 GMT  
		Size: 9.3 KB (9326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955b8a81330f91082609724b9f773e144f31763c075661a1a71ebe0d94fc1977`  
		Last Modified: Mon, 10 Jul 2023 18:21:36 GMT  
		Size: 217.8 MB (217800295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.23-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:d2671ad9c33db7c6e61924d5ce3352b8a43e4f7a40f3dc5a1198ec75a105fe78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.1 MB (443095103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9c0a93977f34511b8636b19abe71786781ffbc54e2aedd1c517c5fabe13ef7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 03:35:40 GMT
COPY dir:46f070668c95bcfc449ea3e3aa03838e4c3f9939658e6aebe91ca179e673aded in /opt/java/openjdk 
# Mon, 10 Jul 2023 18:40:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=77ba1ae0ffc59ff140587a7a8bcc7bb7cfb3a70fe327a37c3c0dbea700436d68 NEO4J_TARBALL=neo4j-enterprise-4.4.23-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 10 Jul 2023 18:40:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
# Mon, 10 Jul 2023 18:40:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 10 Jul 2023 18:40:01 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Mon, 10 Jul 2023 18:40:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.23-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 10 Jul 2023 18:40:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Jul 2023 18:40:15 GMT
WORKDIR /var/lib/neo4j
# Mon, 10 Jul 2023 18:40:15 GMT
VOLUME [/data /logs]
# Mon, 10 Jul 2023 18:40:15 GMT
EXPOSE 7473 7474 7687
# Mon, 10 Jul 2023 18:40:15 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 10 Jul 2023 18:40:15 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b90eb25a0fa4522274c461d519d4e554d5d39052358c321552f0848e5d55556`  
		Last Modified: Wed, 05 Jul 2023 03:46:58 GMT  
		Size: 195.3 MB (195324199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0725c443f8e4bda679cc0ac93798927e5ea62e774f0753c101df7354baf8dbd5`  
		Last Modified: Mon, 10 Jul 2023 18:40:49 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f252db47c49895d4f6ccadcbb176175b06df5c188259732bf706d6fa2a8e5c8e`  
		Last Modified: Mon, 10 Jul 2023 18:40:49 GMT  
		Size: 9.3 KB (9320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5233b4e913fc32223aada1e7209550f4202321215b3160dc8491958859324d`  
		Last Modified: Mon, 10 Jul 2023 18:40:57 GMT  
		Size: 217.7 MB (217694744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:d476f17c0e5c22a4559a4f3275b245b2f8a773e9b39f0224c24c8384998b02b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:79ea371edf6e9673c5508eff4a3f1bd82bd24a9b245972de73a2fe7ab025a3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.6 MB (341583649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec142860f24c22c0e0d2729a0d227aaf92830bd888f31bfd3e961f60e716368`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:15 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:42:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:42:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:42:35 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:42:35 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:42:35 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:42:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:42:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a2003ccc9bff898d52197b197450e5f9d299a5ac61a1f2b0c8617031eb2ea9`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b030f8fa6fcb4d46cee2540085eea25d237d613ebfb3d601299360b0e906f40a`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb71c33bfc11d85c4a4e2a6f0999cf8af96169719c624f9c5a21d16c7f2860b`  
		Last Modified: Wed, 19 Jul 2023 20:43:43 GMT  
		Size: 119.9 MB (119867913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6c18c470c2abc47e52745c24cf9c3886cf42abb202a61522e91ce8055b911a55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340132177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d343e548b4b3e1ac1e22559c657b5f2f69a50d0b42577cd735e6cc03ee612112`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:38 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:53:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:53:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:53:51 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:53:51 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:53:51 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:53:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:53:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48908fefa10dddf638d3bfe0bc2c55b1ec283ca0fcb7e2ffed729c75abbab870`  
		Last Modified: Wed, 19 Jul 2023 21:54:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f22f26bb8d1d33e5e90b5ff02e50039f764c6bc518a8860ca49d689c63f6a2`  
		Last Modified: Wed, 19 Jul 2023 21:54:38 GMT  
		Size: 9.3 KB (9349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568d3fde58f0fa1e76f41e6fa9ec0b1464cfa30e06a28e1b3ee42ae9ed12a0a0`  
		Last Modified: Wed, 19 Jul 2023 21:54:43 GMT  
		Size: 119.6 MB (119581580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-bullseye`

**does not exist** (yet?)

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:d476f17c0e5c22a4559a4f3275b245b2f8a773e9b39f0224c24c8384998b02b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:79ea371edf6e9673c5508eff4a3f1bd82bd24a9b245972de73a2fe7ab025a3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.6 MB (341583649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec142860f24c22c0e0d2729a0d227aaf92830bd888f31bfd3e961f60e716368`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:15 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:42:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:42:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:42:35 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:42:35 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:42:35 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:42:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:42:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a2003ccc9bff898d52197b197450e5f9d299a5ac61a1f2b0c8617031eb2ea9`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b030f8fa6fcb4d46cee2540085eea25d237d613ebfb3d601299360b0e906f40a`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb71c33bfc11d85c4a4e2a6f0999cf8af96169719c624f9c5a21d16c7f2860b`  
		Last Modified: Wed, 19 Jul 2023 20:43:43 GMT  
		Size: 119.9 MB (119867913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6c18c470c2abc47e52745c24cf9c3886cf42abb202a61522e91ce8055b911a55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340132177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d343e548b4b3e1ac1e22559c657b5f2f69a50d0b42577cd735e6cc03ee612112`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:38 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:53:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:53:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:53:51 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:53:51 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:53:51 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:53:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:53:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48908fefa10dddf638d3bfe0bc2c55b1ec283ca0fcb7e2ffed729c75abbab870`  
		Last Modified: Wed, 19 Jul 2023 21:54:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f22f26bb8d1d33e5e90b5ff02e50039f764c6bc518a8860ca49d689c63f6a2`  
		Last Modified: Wed, 19 Jul 2023 21:54:38 GMT  
		Size: 9.3 KB (9349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568d3fde58f0fa1e76f41e6fa9ec0b1464cfa30e06a28e1b3ee42ae9ed12a0a0`  
		Last Modified: Wed, 19 Jul 2023 21:54:43 GMT  
		Size: 119.6 MB (119581580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community-bullseye`

**does not exist** (yet?)

## `neo4j:5-community-ubi8`

**does not exist** (yet?)

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:d6ae764c32c34b4b0e122295e64c8439174a5ed31413881e98dd3b3971035cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ae47bd9d34974259281c752585035c2d97c04394bec086e203a6465d2c0eb567
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **622.6 MB (622619473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0921bf17e559e91456e9a3fc95a2206d224d4c4268ce34b1d7b9f0bd0fa9dca8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:38 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:39 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:43:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:43:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:43:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:43:11 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:43:11 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:43:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:43:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305a772a1f0398766dad78e8918cd6e2afd4fa62e6af50f678e0b22c12dbeae9`  
		Last Modified: Wed, 19 Jul 2023 20:44:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777d13371b09c3cb205758c2b7b606bf0581f800196dedf1340464f2522f8fc4`  
		Last Modified: Wed, 19 Jul 2023 20:44:10 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f1434ff981311c68c5ec9dc6e4994aad81566bd797acddfdadce673aaa4379`  
		Last Modified: Wed, 19 Jul 2023 20:44:27 GMT  
		Size: 400.9 MB (400903735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:036848d96c41a91caee92d98b9c018a4870682a080f9619342c6c1e135af5d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **621.2 MB (621169670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6772a4eb253b8efb709f984202f0293f6661e1d2b2a33e5685fe7427f2b27f8b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:55 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:54:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:54:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:54:15 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:54:15 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:54:15 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:54:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:54:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a245ca64b17dd72350308444a9c2957e650de56f0d71914091baf43208620d`  
		Last Modified: Wed, 19 Jul 2023 21:55:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc66b12c19ac7442e4921b947242d95258407ed3c132cb96a93c4f7c76afbb`  
		Last Modified: Wed, 19 Jul 2023 21:55:10 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db6781454f8bfa678ed580e377f24f4706edcdff38159d4d59f88fb7de23e56`  
		Last Modified: Wed, 19 Jul 2023 21:55:23 GMT  
		Size: 400.6 MB (400619071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise-bullseye`

**does not exist** (yet?)

## `neo4j:5-enterprise-ubi8`

**does not exist** (yet?)

## `neo4j:5-ubi8`

**does not exist** (yet?)

## `neo4j:5.10`

```console
$ docker pull neo4j@sha256:d476f17c0e5c22a4559a4f3275b245b2f8a773e9b39f0224c24c8384998b02b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.10` - linux; amd64

```console
$ docker pull neo4j@sha256:79ea371edf6e9673c5508eff4a3f1bd82bd24a9b245972de73a2fe7ab025a3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.6 MB (341583649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec142860f24c22c0e0d2729a0d227aaf92830bd888f31bfd3e961f60e716368`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:15 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:42:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:42:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:42:35 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:42:35 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:42:35 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:42:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:42:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a2003ccc9bff898d52197b197450e5f9d299a5ac61a1f2b0c8617031eb2ea9`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b030f8fa6fcb4d46cee2540085eea25d237d613ebfb3d601299360b0e906f40a`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb71c33bfc11d85c4a4e2a6f0999cf8af96169719c624f9c5a21d16c7f2860b`  
		Last Modified: Wed, 19 Jul 2023 20:43:43 GMT  
		Size: 119.9 MB (119867913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.10` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6c18c470c2abc47e52745c24cf9c3886cf42abb202a61522e91ce8055b911a55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340132177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d343e548b4b3e1ac1e22559c657b5f2f69a50d0b42577cd735e6cc03ee612112`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:38 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:53:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:53:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:53:51 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:53:51 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:53:51 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:53:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:53:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48908fefa10dddf638d3bfe0bc2c55b1ec283ca0fcb7e2ffed729c75abbab870`  
		Last Modified: Wed, 19 Jul 2023 21:54:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f22f26bb8d1d33e5e90b5ff02e50039f764c6bc518a8860ca49d689c63f6a2`  
		Last Modified: Wed, 19 Jul 2023 21:54:38 GMT  
		Size: 9.3 KB (9349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568d3fde58f0fa1e76f41e6fa9ec0b1464cfa30e06a28e1b3ee42ae9ed12a0a0`  
		Last Modified: Wed, 19 Jul 2023 21:54:43 GMT  
		Size: 119.6 MB (119581580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.10-bullseye`

**does not exist** (yet?)

## `neo4j:5.10-community`

```console
$ docker pull neo4j@sha256:d476f17c0e5c22a4559a4f3275b245b2f8a773e9b39f0224c24c8384998b02b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.10-community` - linux; amd64

```console
$ docker pull neo4j@sha256:79ea371edf6e9673c5508eff4a3f1bd82bd24a9b245972de73a2fe7ab025a3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.6 MB (341583649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec142860f24c22c0e0d2729a0d227aaf92830bd888f31bfd3e961f60e716368`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:15 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:42:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:42:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:42:35 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:42:35 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:42:35 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:42:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:42:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a2003ccc9bff898d52197b197450e5f9d299a5ac61a1f2b0c8617031eb2ea9`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b030f8fa6fcb4d46cee2540085eea25d237d613ebfb3d601299360b0e906f40a`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb71c33bfc11d85c4a4e2a6f0999cf8af96169719c624f9c5a21d16c7f2860b`  
		Last Modified: Wed, 19 Jul 2023 20:43:43 GMT  
		Size: 119.9 MB (119867913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.10-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6c18c470c2abc47e52745c24cf9c3886cf42abb202a61522e91ce8055b911a55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340132177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d343e548b4b3e1ac1e22559c657b5f2f69a50d0b42577cd735e6cc03ee612112`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:38 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:53:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:53:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:53:51 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:53:51 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:53:51 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:53:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:53:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48908fefa10dddf638d3bfe0bc2c55b1ec283ca0fcb7e2ffed729c75abbab870`  
		Last Modified: Wed, 19 Jul 2023 21:54:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f22f26bb8d1d33e5e90b5ff02e50039f764c6bc518a8860ca49d689c63f6a2`  
		Last Modified: Wed, 19 Jul 2023 21:54:38 GMT  
		Size: 9.3 KB (9349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568d3fde58f0fa1e76f41e6fa9ec0b1464cfa30e06a28e1b3ee42ae9ed12a0a0`  
		Last Modified: Wed, 19 Jul 2023 21:54:43 GMT  
		Size: 119.6 MB (119581580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.10-community-bullseye`

**does not exist** (yet?)

## `neo4j:5.10-community-ubi8`

**does not exist** (yet?)

## `neo4j:5.10-enterprise`

```console
$ docker pull neo4j@sha256:d6ae764c32c34b4b0e122295e64c8439174a5ed31413881e98dd3b3971035cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.10-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ae47bd9d34974259281c752585035c2d97c04394bec086e203a6465d2c0eb567
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **622.6 MB (622619473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0921bf17e559e91456e9a3fc95a2206d224d4c4268ce34b1d7b9f0bd0fa9dca8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:38 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:39 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:43:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:43:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:43:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:43:11 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:43:11 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:43:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:43:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305a772a1f0398766dad78e8918cd6e2afd4fa62e6af50f678e0b22c12dbeae9`  
		Last Modified: Wed, 19 Jul 2023 20:44:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777d13371b09c3cb205758c2b7b606bf0581f800196dedf1340464f2522f8fc4`  
		Last Modified: Wed, 19 Jul 2023 20:44:10 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f1434ff981311c68c5ec9dc6e4994aad81566bd797acddfdadce673aaa4379`  
		Last Modified: Wed, 19 Jul 2023 20:44:27 GMT  
		Size: 400.9 MB (400903735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.10-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:036848d96c41a91caee92d98b9c018a4870682a080f9619342c6c1e135af5d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **621.2 MB (621169670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6772a4eb253b8efb709f984202f0293f6661e1d2b2a33e5685fe7427f2b27f8b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:55 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:54:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:54:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:54:15 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:54:15 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:54:15 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:54:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:54:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a245ca64b17dd72350308444a9c2957e650de56f0d71914091baf43208620d`  
		Last Modified: Wed, 19 Jul 2023 21:55:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc66b12c19ac7442e4921b947242d95258407ed3c132cb96a93c4f7c76afbb`  
		Last Modified: Wed, 19 Jul 2023 21:55:10 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db6781454f8bfa678ed580e377f24f4706edcdff38159d4d59f88fb7de23e56`  
		Last Modified: Wed, 19 Jul 2023 21:55:23 GMT  
		Size: 400.6 MB (400619071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.10-enterprise-bullseye`

**does not exist** (yet?)

## `neo4j:5.10-enterprise-ubi8`

**does not exist** (yet?)

## `neo4j:5.10-ubi8`

**does not exist** (yet?)

## `neo4j:5.10.0`

```console
$ docker pull neo4j@sha256:d476f17c0e5c22a4559a4f3275b245b2f8a773e9b39f0224c24c8384998b02b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.10.0` - linux; amd64

```console
$ docker pull neo4j@sha256:79ea371edf6e9673c5508eff4a3f1bd82bd24a9b245972de73a2fe7ab025a3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.6 MB (341583649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec142860f24c22c0e0d2729a0d227aaf92830bd888f31bfd3e961f60e716368`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:15 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:42:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:42:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:42:35 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:42:35 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:42:35 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:42:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:42:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a2003ccc9bff898d52197b197450e5f9d299a5ac61a1f2b0c8617031eb2ea9`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b030f8fa6fcb4d46cee2540085eea25d237d613ebfb3d601299360b0e906f40a`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb71c33bfc11d85c4a4e2a6f0999cf8af96169719c624f9c5a21d16c7f2860b`  
		Last Modified: Wed, 19 Jul 2023 20:43:43 GMT  
		Size: 119.9 MB (119867913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.10.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6c18c470c2abc47e52745c24cf9c3886cf42abb202a61522e91ce8055b911a55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340132177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d343e548b4b3e1ac1e22559c657b5f2f69a50d0b42577cd735e6cc03ee612112`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:38 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:53:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:53:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:53:51 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:53:51 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:53:51 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:53:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:53:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48908fefa10dddf638d3bfe0bc2c55b1ec283ca0fcb7e2ffed729c75abbab870`  
		Last Modified: Wed, 19 Jul 2023 21:54:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f22f26bb8d1d33e5e90b5ff02e50039f764c6bc518a8860ca49d689c63f6a2`  
		Last Modified: Wed, 19 Jul 2023 21:54:38 GMT  
		Size: 9.3 KB (9349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568d3fde58f0fa1e76f41e6fa9ec0b1464cfa30e06a28e1b3ee42ae9ed12a0a0`  
		Last Modified: Wed, 19 Jul 2023 21:54:43 GMT  
		Size: 119.6 MB (119581580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.10.0-bullseye`

**does not exist** (yet?)

## `neo4j:5.10.0-community`

```console
$ docker pull neo4j@sha256:d476f17c0e5c22a4559a4f3275b245b2f8a773e9b39f0224c24c8384998b02b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.10.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:79ea371edf6e9673c5508eff4a3f1bd82bd24a9b245972de73a2fe7ab025a3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.6 MB (341583649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec142860f24c22c0e0d2729a0d227aaf92830bd888f31bfd3e961f60e716368`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:15 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:42:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:42:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:42:35 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:42:35 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:42:35 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:42:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:42:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a2003ccc9bff898d52197b197450e5f9d299a5ac61a1f2b0c8617031eb2ea9`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b030f8fa6fcb4d46cee2540085eea25d237d613ebfb3d601299360b0e906f40a`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb71c33bfc11d85c4a4e2a6f0999cf8af96169719c624f9c5a21d16c7f2860b`  
		Last Modified: Wed, 19 Jul 2023 20:43:43 GMT  
		Size: 119.9 MB (119867913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.10.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6c18c470c2abc47e52745c24cf9c3886cf42abb202a61522e91ce8055b911a55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340132177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d343e548b4b3e1ac1e22559c657b5f2f69a50d0b42577cd735e6cc03ee612112`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:38 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:53:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:53:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:53:51 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:53:51 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:53:51 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:53:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:53:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48908fefa10dddf638d3bfe0bc2c55b1ec283ca0fcb7e2ffed729c75abbab870`  
		Last Modified: Wed, 19 Jul 2023 21:54:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f22f26bb8d1d33e5e90b5ff02e50039f764c6bc518a8860ca49d689c63f6a2`  
		Last Modified: Wed, 19 Jul 2023 21:54:38 GMT  
		Size: 9.3 KB (9349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568d3fde58f0fa1e76f41e6fa9ec0b1464cfa30e06a28e1b3ee42ae9ed12a0a0`  
		Last Modified: Wed, 19 Jul 2023 21:54:43 GMT  
		Size: 119.6 MB (119581580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.10.0-community-bullseye`

**does not exist** (yet?)

## `neo4j:5.10.0-community-ubi8`

**does not exist** (yet?)

## `neo4j:5.10.0-enterprise`

```console
$ docker pull neo4j@sha256:d6ae764c32c34b4b0e122295e64c8439174a5ed31413881e98dd3b3971035cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.10.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ae47bd9d34974259281c752585035c2d97c04394bec086e203a6465d2c0eb567
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **622.6 MB (622619473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0921bf17e559e91456e9a3fc95a2206d224d4c4268ce34b1d7b9f0bd0fa9dca8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:38 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:39 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:43:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:43:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:43:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:43:11 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:43:11 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:43:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:43:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305a772a1f0398766dad78e8918cd6e2afd4fa62e6af50f678e0b22c12dbeae9`  
		Last Modified: Wed, 19 Jul 2023 20:44:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777d13371b09c3cb205758c2b7b606bf0581f800196dedf1340464f2522f8fc4`  
		Last Modified: Wed, 19 Jul 2023 20:44:10 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f1434ff981311c68c5ec9dc6e4994aad81566bd797acddfdadce673aaa4379`  
		Last Modified: Wed, 19 Jul 2023 20:44:27 GMT  
		Size: 400.9 MB (400903735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.10.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:036848d96c41a91caee92d98b9c018a4870682a080f9619342c6c1e135af5d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **621.2 MB (621169670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6772a4eb253b8efb709f984202f0293f6661e1d2b2a33e5685fe7427f2b27f8b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:55 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:54:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:54:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:54:15 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:54:15 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:54:15 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:54:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:54:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a245ca64b17dd72350308444a9c2957e650de56f0d71914091baf43208620d`  
		Last Modified: Wed, 19 Jul 2023 21:55:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc66b12c19ac7442e4921b947242d95258407ed3c132cb96a93c4f7c76afbb`  
		Last Modified: Wed, 19 Jul 2023 21:55:10 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db6781454f8bfa678ed580e377f24f4706edcdff38159d4d59f88fb7de23e56`  
		Last Modified: Wed, 19 Jul 2023 21:55:23 GMT  
		Size: 400.6 MB (400619071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.10.0-enterprise-bullseye`

**does not exist** (yet?)

## `neo4j:5.10.0-enterprise-ubi8`

**does not exist** (yet?)

## `neo4j:5.10.0-ubi8`

**does not exist** (yet?)

## `neo4j:bullseye`

**does not exist** (yet?)

## `neo4j:community`

```console
$ docker pull neo4j@sha256:d476f17c0e5c22a4559a4f3275b245b2f8a773e9b39f0224c24c8384998b02b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:79ea371edf6e9673c5508eff4a3f1bd82bd24a9b245972de73a2fe7ab025a3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.6 MB (341583649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec142860f24c22c0e0d2729a0d227aaf92830bd888f31bfd3e961f60e716368`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:15 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:42:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:42:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:42:35 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:42:35 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:42:35 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:42:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:42:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a2003ccc9bff898d52197b197450e5f9d299a5ac61a1f2b0c8617031eb2ea9`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b030f8fa6fcb4d46cee2540085eea25d237d613ebfb3d601299360b0e906f40a`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb71c33bfc11d85c4a4e2a6f0999cf8af96169719c624f9c5a21d16c7f2860b`  
		Last Modified: Wed, 19 Jul 2023 20:43:43 GMT  
		Size: 119.9 MB (119867913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6c18c470c2abc47e52745c24cf9c3886cf42abb202a61522e91ce8055b911a55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340132177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d343e548b4b3e1ac1e22559c657b5f2f69a50d0b42577cd735e6cc03ee612112`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:38 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:53:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:53:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:53:51 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:53:51 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:53:51 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:53:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:53:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48908fefa10dddf638d3bfe0bc2c55b1ec283ca0fcb7e2ffed729c75abbab870`  
		Last Modified: Wed, 19 Jul 2023 21:54:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f22f26bb8d1d33e5e90b5ff02e50039f764c6bc518a8860ca49d689c63f6a2`  
		Last Modified: Wed, 19 Jul 2023 21:54:38 GMT  
		Size: 9.3 KB (9349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568d3fde58f0fa1e76f41e6fa9ec0b1464cfa30e06a28e1b3ee42ae9ed12a0a0`  
		Last Modified: Wed, 19 Jul 2023 21:54:43 GMT  
		Size: 119.6 MB (119581580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community-bullseye`

**does not exist** (yet?)

## `neo4j:community-ubi8`

**does not exist** (yet?)

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:d6ae764c32c34b4b0e122295e64c8439174a5ed31413881e98dd3b3971035cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ae47bd9d34974259281c752585035c2d97c04394bec086e203a6465d2c0eb567
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **622.6 MB (622619473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0921bf17e559e91456e9a3fc95a2206d224d4c4268ce34b1d7b9f0bd0fa9dca8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:38 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:39 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:43:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:43:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:43:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:43:11 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:43:11 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:43:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:43:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305a772a1f0398766dad78e8918cd6e2afd4fa62e6af50f678e0b22c12dbeae9`  
		Last Modified: Wed, 19 Jul 2023 20:44:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777d13371b09c3cb205758c2b7b606bf0581f800196dedf1340464f2522f8fc4`  
		Last Modified: Wed, 19 Jul 2023 20:44:10 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f1434ff981311c68c5ec9dc6e4994aad81566bd797acddfdadce673aaa4379`  
		Last Modified: Wed, 19 Jul 2023 20:44:27 GMT  
		Size: 400.9 MB (400903735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:036848d96c41a91caee92d98b9c018a4870682a080f9619342c6c1e135af5d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **621.2 MB (621169670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6772a4eb253b8efb709f984202f0293f6661e1d2b2a33e5685fe7427f2b27f8b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:55 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:54:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:54:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:54:15 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:54:15 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:54:15 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:54:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:54:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a245ca64b17dd72350308444a9c2957e650de56f0d71914091baf43208620d`  
		Last Modified: Wed, 19 Jul 2023 21:55:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc66b12c19ac7442e4921b947242d95258407ed3c132cb96a93c4f7c76afbb`  
		Last Modified: Wed, 19 Jul 2023 21:55:10 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db6781454f8bfa678ed580e377f24f4706edcdff38159d4d59f88fb7de23e56`  
		Last Modified: Wed, 19 Jul 2023 21:55:23 GMT  
		Size: 400.6 MB (400619071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise-bullseye`

**does not exist** (yet?)

## `neo4j:enterprise-ubi8`

**does not exist** (yet?)

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:d476f17c0e5c22a4559a4f3275b245b2f8a773e9b39f0224c24c8384998b02b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:79ea371edf6e9673c5508eff4a3f1bd82bd24a9b245972de73a2fe7ab025a3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.6 MB (341583649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec142860f24c22c0e0d2729a0d227aaf92830bd888f31bfd3e961f60e716368`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 20:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 20:42:13 GMT
COPY dir:4f02f3c240ecc691ff41263b0454f619d51a2ba11a57fe51c0e31e7ff62a9194 in /opt/java/openjdk 
# Wed, 19 Jul 2023 20:42:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 20:42:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 20:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 20:42:15 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 20:42:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 20:42:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 20:42:35 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 20:42:35 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 20:42:35 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 20:42:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:42:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef95bdc735d909eaee3e2c5c5072bf884101807a69a15402bee83aab9a13f4`  
		Last Modified: Wed, 19 Jul 2023 20:43:50 GMT  
		Size: 192.6 MB (192580400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a2003ccc9bff898d52197b197450e5f9d299a5ac61a1f2b0c8617031eb2ea9`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b030f8fa6fcb4d46cee2540085eea25d237d613ebfb3d601299360b0e906f40a`  
		Last Modified: Wed, 19 Jul 2023 20:43:36 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb71c33bfc11d85c4a4e2a6f0999cf8af96169719c624f9c5a21d16c7f2860b`  
		Last Modified: Wed, 19 Jul 2023 20:43:43 GMT  
		Size: 119.9 MB (119867913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6c18c470c2abc47e52745c24cf9c3886cf42abb202a61522e91ce8055b911a55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340132177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d343e548b4b3e1ac1e22559c657b5f2f69a50d0b42577cd735e6cc03ee612112`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Wed, 19 Jul 2023 21:53:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 19 Jul 2023 21:53:33 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Wed, 19 Jul 2023 21:53:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 19 Jul 2023 21:53:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 19 Jul 2023 21:53:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 19 Jul 2023 21:53:38 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 19 Jul 2023 21:53:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Jul 2023 21:53:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Jul 2023 21:53:51 GMT
WORKDIR /var/lib/neo4j
# Wed, 19 Jul 2023 21:53:51 GMT
VOLUME [/data /logs]
# Wed, 19 Jul 2023 21:53:51 GMT
EXPOSE 7473 7474 7687
# Wed, 19 Jul 2023 21:53:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 21:53:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae78352a9d3c0d006bcb2ac05c5c40eff931299fa3ba06e5ae5312139478555`  
		Last Modified: Wed, 19 Jul 2023 21:54:49 GMT  
		Size: 191.4 MB (191387633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48908fefa10dddf638d3bfe0bc2c55b1ec283ca0fcb7e2ffed729c75abbab870`  
		Last Modified: Wed, 19 Jul 2023 21:54:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f22f26bb8d1d33e5e90b5ff02e50039f764c6bc518a8860ca49d689c63f6a2`  
		Last Modified: Wed, 19 Jul 2023 21:54:38 GMT  
		Size: 9.3 KB (9349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568d3fde58f0fa1e76f41e6fa9ec0b1464cfa30e06a28e1b3ee42ae9ed12a0a0`  
		Last Modified: Wed, 19 Jul 2023 21:54:43 GMT  
		Size: 119.6 MB (119581580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:ubi8`

**does not exist** (yet?)
