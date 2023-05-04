<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.19`](#neo4j4419)
-	[`neo4j:4.4.19-community`](#neo4j4419-community)
-	[`neo4j:4.4.19-enterprise`](#neo4j4419-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5.7`](#neo4j57)
-	[`neo4j:5.7-community`](#neo4j57-community)
-	[`neo4j:5.7-enterprise`](#neo4j57-enterprise)
-	[`neo4j:5.7.0`](#neo4j570)
-	[`neo4j:5.7.0-community`](#neo4j570-community)
-	[`neo4j:5.7.0-enterprise`](#neo4j570-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:5aa2c0bc6d3529dc5ac31d424e4992ad36d935ba76ec04434386d376b4e4bf2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:c025681468294eb912735b2cbb4a58bb918ef9443b78705d6917d394606d8a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.6 MB (349626075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbfbe17e6c90efdf848d08927657635b5643dc0895b23d9baa7cbe714c15cff`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:27:22 GMT
COPY dir:df592a42a629b9630bdf0ab57a63e6c60f66d91934439985e01efbb58723e9ee in /opt/java/openjdk 
# Wed, 03 May 2023 21:10:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:10:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 03 May 2023 21:10:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:40 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 03 May 2023 21:10:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:50 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:50 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:50 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ff29d68fcfaa0b79ea63e544be12bffb5a83bf5c3d7b0d8ce3ccbdc611171`  
		Last Modified: Wed, 03 May 2023 20:36:57 GMT  
		Size: 198.5 MB (198549520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1019d7bf682c44d6c7700d8a2e7bce3dcfa9baba99b54eec173ebfec7232c0`  
		Last Modified: Wed, 03 May 2023 21:12:11 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad43115f03fe553fb7f9e54668567093ff67409ae9e3752c89796a3267c8ec6f`  
		Last Modified: Wed, 03 May 2023 21:12:11 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de71868cf689640908b163a0ea61fa250a9d3d9dcc5a56239074972e4786f264`  
		Last Modified: Wed, 03 May 2023 21:12:17 GMT  
		Size: 119.7 MB (119660608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f785d0cdb940c0d3af0870ca1e978a96cda87b7b4ab383e90c78ad60d8a92a00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344907362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34d7e3d74bf44fafe1c31aa74bcca972894e24e9894854be6561210fee47536`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Thu, 04 May 2023 12:05:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:05:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Thu, 04 May 2023 12:05:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:05:30 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Thu, 04 May 2023 12:05:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:39 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:39 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:40 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:40 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78b87eea2caf98f51733ab05c70e2390e47ba43561b4d5e64ce1f035adb4d5b`  
		Last Modified: Thu, 04 May 2023 12:06:56 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1297f0820ec77dc87fca58cb3c7d1452001027792bf525bfa87191b9540b93c`  
		Last Modified: Thu, 04 May 2023 12:06:56 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a718454e9752be9cb18bdd6adabffd967c492a2a835f258eb859c09a9708aff6`  
		Last Modified: Thu, 04 May 2023 12:07:01 GMT  
		Size: 119.5 MB (119517959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:5aa2c0bc6d3529dc5ac31d424e4992ad36d935ba76ec04434386d376b4e4bf2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:c025681468294eb912735b2cbb4a58bb918ef9443b78705d6917d394606d8a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.6 MB (349626075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbfbe17e6c90efdf848d08927657635b5643dc0895b23d9baa7cbe714c15cff`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:27:22 GMT
COPY dir:df592a42a629b9630bdf0ab57a63e6c60f66d91934439985e01efbb58723e9ee in /opt/java/openjdk 
# Wed, 03 May 2023 21:10:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:10:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 03 May 2023 21:10:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:40 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 03 May 2023 21:10:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:50 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:50 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:50 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ff29d68fcfaa0b79ea63e544be12bffb5a83bf5c3d7b0d8ce3ccbdc611171`  
		Last Modified: Wed, 03 May 2023 20:36:57 GMT  
		Size: 198.5 MB (198549520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1019d7bf682c44d6c7700d8a2e7bce3dcfa9baba99b54eec173ebfec7232c0`  
		Last Modified: Wed, 03 May 2023 21:12:11 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad43115f03fe553fb7f9e54668567093ff67409ae9e3752c89796a3267c8ec6f`  
		Last Modified: Wed, 03 May 2023 21:12:11 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de71868cf689640908b163a0ea61fa250a9d3d9dcc5a56239074972e4786f264`  
		Last Modified: Wed, 03 May 2023 21:12:17 GMT  
		Size: 119.7 MB (119660608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f785d0cdb940c0d3af0870ca1e978a96cda87b7b4ab383e90c78ad60d8a92a00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344907362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34d7e3d74bf44fafe1c31aa74bcca972894e24e9894854be6561210fee47536`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Thu, 04 May 2023 12:05:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:05:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Thu, 04 May 2023 12:05:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:05:30 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Thu, 04 May 2023 12:05:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:39 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:39 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:40 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:40 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78b87eea2caf98f51733ab05c70e2390e47ba43561b4d5e64ce1f035adb4d5b`  
		Last Modified: Thu, 04 May 2023 12:06:56 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1297f0820ec77dc87fca58cb3c7d1452001027792bf525bfa87191b9540b93c`  
		Last Modified: Thu, 04 May 2023 12:06:56 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a718454e9752be9cb18bdd6adabffd967c492a2a835f258eb859c09a9708aff6`  
		Last Modified: Thu, 04 May 2023 12:07:01 GMT  
		Size: 119.5 MB (119517959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:11d21a44a13bde3e5cd1fdc69066b5313240b9c1b5df0b9f03205065f5ad2dc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:24cd67b04137978808eae14d4a188ad650821d90cfb33918bda61fc982c33e85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.4 MB (446393563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcaae9c6538cf10c8f7a635f1a7455db12c36fa524550e8edde4a49b399dba76`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:27:22 GMT
COPY dir:df592a42a629b9630bdf0ab57a63e6c60f66d91934439985e01efbb58723e9ee in /opt/java/openjdk 
# Wed, 03 May 2023 21:10:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e9ecf2706abff535c4ac9e902ca36257ab23af96be3386ea54f0ec17dcb7cf8e NEO4J_TARBALL=neo4j-enterprise-4.4.19-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:10:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
# Wed, 03 May 2023 21:10:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:53 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 03 May 2023 21:11:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:11:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:11:06 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:11:06 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:11:06 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:11:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:11:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ff29d68fcfaa0b79ea63e544be12bffb5a83bf5c3d7b0d8ce3ccbdc611171`  
		Last Modified: Wed, 03 May 2023 20:36:57 GMT  
		Size: 198.5 MB (198549520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c19104d4ad42bd6054842bd5ddc7b4d7608dac7f9555991e2cfff9728f71d7`  
		Last Modified: Wed, 03 May 2023 21:12:29 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65addb70dcad20f1f954ed4aa3ecc8524dff1b20a23cf93a24806fc1a85f66cd`  
		Last Modified: Wed, 03 May 2023 21:12:29 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae8c2f278ab09edca13e1c469af27ee9a123483df1bd67d8542cd3500ee9f4a`  
		Last Modified: Wed, 03 May 2023 21:12:38 GMT  
		Size: 216.4 MB (216428098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:65eb92cf8d5ab246fe228d11dd3102c436ae8217847439db489ecc9291a86611
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.7 MB (441675410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4360bfabdd1eb2c0428c3a518d33db00eabdab6dfe5a0c124470923fe72302df`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Thu, 04 May 2023 12:05:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e9ecf2706abff535c4ac9e902ca36257ab23af96be3386ea54f0ec17dcb7cf8e NEO4J_TARBALL=neo4j-enterprise-4.4.19-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:05:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
# Thu, 04 May 2023 12:05:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:05:43 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Thu, 04 May 2023 12:05:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:56 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:56 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:56 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:56 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d6afc98d2829f19f6050c43e8f70813fbb02303cf8c4fa0969c7c2aa1e3978`  
		Last Modified: Thu, 04 May 2023 12:07:13 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a2a66cd05153c19d51918da9fc8e1a6790f7f43b934e51022f6a8a76fd1247`  
		Last Modified: Thu, 04 May 2023 12:07:13 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bdbb9ab3ee1ad3e4c95ec756618fd425be6f9293237d84d540b7a92154e2ea`  
		Last Modified: Thu, 04 May 2023 12:07:21 GMT  
		Size: 216.3 MB (216286011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.19`

```console
$ docker pull neo4j@sha256:5aa2c0bc6d3529dc5ac31d424e4992ad36d935ba76ec04434386d376b4e4bf2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.19` - linux; amd64

```console
$ docker pull neo4j@sha256:c025681468294eb912735b2cbb4a58bb918ef9443b78705d6917d394606d8a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.6 MB (349626075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbfbe17e6c90efdf848d08927657635b5643dc0895b23d9baa7cbe714c15cff`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:27:22 GMT
COPY dir:df592a42a629b9630bdf0ab57a63e6c60f66d91934439985e01efbb58723e9ee in /opt/java/openjdk 
# Wed, 03 May 2023 21:10:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:10:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 03 May 2023 21:10:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:40 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 03 May 2023 21:10:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:50 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:50 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:50 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ff29d68fcfaa0b79ea63e544be12bffb5a83bf5c3d7b0d8ce3ccbdc611171`  
		Last Modified: Wed, 03 May 2023 20:36:57 GMT  
		Size: 198.5 MB (198549520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1019d7bf682c44d6c7700d8a2e7bce3dcfa9baba99b54eec173ebfec7232c0`  
		Last Modified: Wed, 03 May 2023 21:12:11 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad43115f03fe553fb7f9e54668567093ff67409ae9e3752c89796a3267c8ec6f`  
		Last Modified: Wed, 03 May 2023 21:12:11 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de71868cf689640908b163a0ea61fa250a9d3d9dcc5a56239074972e4786f264`  
		Last Modified: Wed, 03 May 2023 21:12:17 GMT  
		Size: 119.7 MB (119660608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.19` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f785d0cdb940c0d3af0870ca1e978a96cda87b7b4ab383e90c78ad60d8a92a00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344907362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34d7e3d74bf44fafe1c31aa74bcca972894e24e9894854be6561210fee47536`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Thu, 04 May 2023 12:05:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:05:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Thu, 04 May 2023 12:05:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:05:30 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Thu, 04 May 2023 12:05:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:39 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:39 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:40 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:40 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78b87eea2caf98f51733ab05c70e2390e47ba43561b4d5e64ce1f035adb4d5b`  
		Last Modified: Thu, 04 May 2023 12:06:56 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1297f0820ec77dc87fca58cb3c7d1452001027792bf525bfa87191b9540b93c`  
		Last Modified: Thu, 04 May 2023 12:06:56 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a718454e9752be9cb18bdd6adabffd967c492a2a835f258eb859c09a9708aff6`  
		Last Modified: Thu, 04 May 2023 12:07:01 GMT  
		Size: 119.5 MB (119517959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.19-community`

```console
$ docker pull neo4j@sha256:5aa2c0bc6d3529dc5ac31d424e4992ad36d935ba76ec04434386d376b4e4bf2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.19-community` - linux; amd64

```console
$ docker pull neo4j@sha256:c025681468294eb912735b2cbb4a58bb918ef9443b78705d6917d394606d8a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.6 MB (349626075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbfbe17e6c90efdf848d08927657635b5643dc0895b23d9baa7cbe714c15cff`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:27:22 GMT
COPY dir:df592a42a629b9630bdf0ab57a63e6c60f66d91934439985e01efbb58723e9ee in /opt/java/openjdk 
# Wed, 03 May 2023 21:10:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:10:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 03 May 2023 21:10:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:40 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 03 May 2023 21:10:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:50 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:50 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:50 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ff29d68fcfaa0b79ea63e544be12bffb5a83bf5c3d7b0d8ce3ccbdc611171`  
		Last Modified: Wed, 03 May 2023 20:36:57 GMT  
		Size: 198.5 MB (198549520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1019d7bf682c44d6c7700d8a2e7bce3dcfa9baba99b54eec173ebfec7232c0`  
		Last Modified: Wed, 03 May 2023 21:12:11 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad43115f03fe553fb7f9e54668567093ff67409ae9e3752c89796a3267c8ec6f`  
		Last Modified: Wed, 03 May 2023 21:12:11 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de71868cf689640908b163a0ea61fa250a9d3d9dcc5a56239074972e4786f264`  
		Last Modified: Wed, 03 May 2023 21:12:17 GMT  
		Size: 119.7 MB (119660608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.19-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f785d0cdb940c0d3af0870ca1e978a96cda87b7b4ab383e90c78ad60d8a92a00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344907362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34d7e3d74bf44fafe1c31aa74bcca972894e24e9894854be6561210fee47536`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Thu, 04 May 2023 12:05:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:05:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Thu, 04 May 2023 12:05:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:05:30 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Thu, 04 May 2023 12:05:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:39 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:39 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:40 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:40 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78b87eea2caf98f51733ab05c70e2390e47ba43561b4d5e64ce1f035adb4d5b`  
		Last Modified: Thu, 04 May 2023 12:06:56 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1297f0820ec77dc87fca58cb3c7d1452001027792bf525bfa87191b9540b93c`  
		Last Modified: Thu, 04 May 2023 12:06:56 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a718454e9752be9cb18bdd6adabffd967c492a2a835f258eb859c09a9708aff6`  
		Last Modified: Thu, 04 May 2023 12:07:01 GMT  
		Size: 119.5 MB (119517959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.19-enterprise`

```console
$ docker pull neo4j@sha256:11d21a44a13bde3e5cd1fdc69066b5313240b9c1b5df0b9f03205065f5ad2dc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.19-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:24cd67b04137978808eae14d4a188ad650821d90cfb33918bda61fc982c33e85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.4 MB (446393563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcaae9c6538cf10c8f7a635f1a7455db12c36fa524550e8edde4a49b399dba76`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:27:22 GMT
COPY dir:df592a42a629b9630bdf0ab57a63e6c60f66d91934439985e01efbb58723e9ee in /opt/java/openjdk 
# Wed, 03 May 2023 21:10:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e9ecf2706abff535c4ac9e902ca36257ab23af96be3386ea54f0ec17dcb7cf8e NEO4J_TARBALL=neo4j-enterprise-4.4.19-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:10:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
# Wed, 03 May 2023 21:10:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:53 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 03 May 2023 21:11:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:11:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:11:06 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:11:06 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:11:06 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:11:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:11:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ff29d68fcfaa0b79ea63e544be12bffb5a83bf5c3d7b0d8ce3ccbdc611171`  
		Last Modified: Wed, 03 May 2023 20:36:57 GMT  
		Size: 198.5 MB (198549520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c19104d4ad42bd6054842bd5ddc7b4d7608dac7f9555991e2cfff9728f71d7`  
		Last Modified: Wed, 03 May 2023 21:12:29 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65addb70dcad20f1f954ed4aa3ecc8524dff1b20a23cf93a24806fc1a85f66cd`  
		Last Modified: Wed, 03 May 2023 21:12:29 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae8c2f278ab09edca13e1c469af27ee9a123483df1bd67d8542cd3500ee9f4a`  
		Last Modified: Wed, 03 May 2023 21:12:38 GMT  
		Size: 216.4 MB (216428098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.19-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:65eb92cf8d5ab246fe228d11dd3102c436ae8217847439db489ecc9291a86611
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.7 MB (441675410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4360bfabdd1eb2c0428c3a518d33db00eabdab6dfe5a0c124470923fe72302df`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Thu, 04 May 2023 12:05:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e9ecf2706abff535c4ac9e902ca36257ab23af96be3386ea54f0ec17dcb7cf8e NEO4J_TARBALL=neo4j-enterprise-4.4.19-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:05:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
# Thu, 04 May 2023 12:05:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:05:43 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Thu, 04 May 2023 12:05:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:56 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:56 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:56 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:56 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d6afc98d2829f19f6050c43e8f70813fbb02303cf8c4fa0969c7c2aa1e3978`  
		Last Modified: Thu, 04 May 2023 12:07:13 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a2a66cd05153c19d51918da9fc8e1a6790f7f43b934e51022f6a8a76fd1247`  
		Last Modified: Thu, 04 May 2023 12:07:13 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bdbb9ab3ee1ad3e4c95ec756618fd425be6f9293237d84d540b7a92154e2ea`  
		Last Modified: Thu, 04 May 2023 12:07:21 GMT  
		Size: 216.3 MB (216286011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:ed6eb77058badabf0bcfda50da1f2dd5b53314f6afaacaed17eb1b65b64e3b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:135374c22967b8b028cfe0ec231e8faa28bb189dcb703f7c13487c6a43ae8722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339670142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc3aa6987130b610e932d5f648d9bcf34ba20f08f2ade3e01358ed68bdafcf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:09:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:09:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:11 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:11 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc29b8a0be2fdad2c0209669f62e4a52c8f1822951fd3606aee9871f291d458`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473676f5c4b0591fda9c3a2dc4d07de297f88ad552f76e8f8c149e35c2d1c5c2`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93765534ca788832bdfd3a07f7f80c9b8272a126028f2b2b9f44bce7399bf5d5`  
		Last Modified: Wed, 03 May 2023 21:11:25 GMT  
		Size: 115.7 MB (115673571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7aa4ae79e62f700964a424d6166309162ad421ea7241cdfef8782cb7b5abf210
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (336981794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6c0929c126c1a2abcd1b5af1ca7420955f76624ac87ea1d5e06f14b84b271`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:04:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:04:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:04:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:04:48 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:01 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:01 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a8328b0b62b333b941f4f72d41fbe9f1cb67c1bdfd42ef100aa881314e839`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ce690ce0b7d3890d98ff9ccdded5c33f4227911f17a5595392105e27326e3`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 8.8 KB (8773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b6be57bf03bc40983fbb0f78148f99a9c9fc273d643783cc2d9a6ed968b1a`  
		Last Modified: Thu, 04 May 2023 12:06:14 GMT  
		Size: 115.5 MB (115528758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:ed6eb77058badabf0bcfda50da1f2dd5b53314f6afaacaed17eb1b65b64e3b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:135374c22967b8b028cfe0ec231e8faa28bb189dcb703f7c13487c6a43ae8722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339670142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc3aa6987130b610e932d5f648d9bcf34ba20f08f2ade3e01358ed68bdafcf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:09:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:09:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:11 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:11 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc29b8a0be2fdad2c0209669f62e4a52c8f1822951fd3606aee9871f291d458`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473676f5c4b0591fda9c3a2dc4d07de297f88ad552f76e8f8c149e35c2d1c5c2`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93765534ca788832bdfd3a07f7f80c9b8272a126028f2b2b9f44bce7399bf5d5`  
		Last Modified: Wed, 03 May 2023 21:11:25 GMT  
		Size: 115.7 MB (115673571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7aa4ae79e62f700964a424d6166309162ad421ea7241cdfef8782cb7b5abf210
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (336981794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6c0929c126c1a2abcd1b5af1ca7420955f76624ac87ea1d5e06f14b84b271`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:04:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:04:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:04:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:04:48 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:01 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:01 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a8328b0b62b333b941f4f72d41fbe9f1cb67c1bdfd42ef100aa881314e839`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ce690ce0b7d3890d98ff9ccdded5c33f4227911f17a5595392105e27326e3`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 8.8 KB (8773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b6be57bf03bc40983fbb0f78148f99a9c9fc273d643783cc2d9a6ed968b1a`  
		Last Modified: Thu, 04 May 2023 12:06:14 GMT  
		Size: 115.5 MB (115528758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:16fe2db96720d35739853ca3206a1f3c8ab89c80c89847a818117bb63d2a4259
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:c5374710b0c030a4bb2aeb24063b96defe07fb8c734cee9c02c68d24bc6a917b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **604.1 MB (604135721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251cc4980cb5b46904354ed301f894460a85ee6a9c7c9f7a29caecec5d103240`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:10:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:10:15 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:16 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:32 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:33 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:33 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:33 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:33 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:33 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:33 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069006ee6f68bbfa2f63568d190ac9c3fee8821bf75102d1c1245f45165d65cf`  
		Last Modified: Wed, 03 May 2023 21:11:45 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2168d6eaa4f94cb727d5db4014c9f6b927a996fc32add8714f06f256887f8a`  
		Last Modified: Wed, 03 May 2023 21:11:44 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560b208648ba4f9761e0d4a0810c7912790d2e72c631f5364f5bd3b3b6505a2`  
		Last Modified: Wed, 03 May 2023 21:11:59 GMT  
		Size: 380.1 MB (380139150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:94abe8120c5430ab066aea1692491fa9d4ecf8d504a807510d5498a1562eadfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.4 MB (601449266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d30c05a208e81fc92ba79e35c04df9af40e8950da321169bfa87bf06e621d7d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:05:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:05:06 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:05:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:05:07 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:25 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:25 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73a1fc72b29e2bb1ea0dd76ad5507ef446c37ba2ec53af00c078d2f158d3424`  
		Last Modified: Thu, 04 May 2023 12:06:33 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b19eaac8bbe54d4c8bc4102e86c17dbff7bea7fa395db92ddd87c0dd8ae40c`  
		Last Modified: Thu, 04 May 2023 12:06:33 GMT  
		Size: 8.8 KB (8772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa3fe131fde0ce072e7b87753cf16cd5d86a83e95ebe1ea85581e4b7cf01a8f`  
		Last Modified: Thu, 04 May 2023 12:06:45 GMT  
		Size: 380.0 MB (379996227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7`

```console
$ docker pull neo4j@sha256:ed6eb77058badabf0bcfda50da1f2dd5b53314f6afaacaed17eb1b65b64e3b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7` - linux; amd64

```console
$ docker pull neo4j@sha256:135374c22967b8b028cfe0ec231e8faa28bb189dcb703f7c13487c6a43ae8722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339670142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc3aa6987130b610e932d5f648d9bcf34ba20f08f2ade3e01358ed68bdafcf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:09:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:09:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:11 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:11 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc29b8a0be2fdad2c0209669f62e4a52c8f1822951fd3606aee9871f291d458`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473676f5c4b0591fda9c3a2dc4d07de297f88ad552f76e8f8c149e35c2d1c5c2`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93765534ca788832bdfd3a07f7f80c9b8272a126028f2b2b9f44bce7399bf5d5`  
		Last Modified: Wed, 03 May 2023 21:11:25 GMT  
		Size: 115.7 MB (115673571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7aa4ae79e62f700964a424d6166309162ad421ea7241cdfef8782cb7b5abf210
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (336981794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6c0929c126c1a2abcd1b5af1ca7420955f76624ac87ea1d5e06f14b84b271`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:04:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:04:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:04:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:04:48 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:01 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:01 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a8328b0b62b333b941f4f72d41fbe9f1cb67c1bdfd42ef100aa881314e839`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ce690ce0b7d3890d98ff9ccdded5c33f4227911f17a5595392105e27326e3`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 8.8 KB (8773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b6be57bf03bc40983fbb0f78148f99a9c9fc273d643783cc2d9a6ed968b1a`  
		Last Modified: Thu, 04 May 2023 12:06:14 GMT  
		Size: 115.5 MB (115528758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7-community`

```console
$ docker pull neo4j@sha256:ed6eb77058badabf0bcfda50da1f2dd5b53314f6afaacaed17eb1b65b64e3b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7-community` - linux; amd64

```console
$ docker pull neo4j@sha256:135374c22967b8b028cfe0ec231e8faa28bb189dcb703f7c13487c6a43ae8722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339670142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc3aa6987130b610e932d5f648d9bcf34ba20f08f2ade3e01358ed68bdafcf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:09:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:09:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:11 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:11 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc29b8a0be2fdad2c0209669f62e4a52c8f1822951fd3606aee9871f291d458`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473676f5c4b0591fda9c3a2dc4d07de297f88ad552f76e8f8c149e35c2d1c5c2`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93765534ca788832bdfd3a07f7f80c9b8272a126028f2b2b9f44bce7399bf5d5`  
		Last Modified: Wed, 03 May 2023 21:11:25 GMT  
		Size: 115.7 MB (115673571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7aa4ae79e62f700964a424d6166309162ad421ea7241cdfef8782cb7b5abf210
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (336981794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6c0929c126c1a2abcd1b5af1ca7420955f76624ac87ea1d5e06f14b84b271`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:04:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:04:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:04:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:04:48 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:01 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:01 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a8328b0b62b333b941f4f72d41fbe9f1cb67c1bdfd42ef100aa881314e839`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ce690ce0b7d3890d98ff9ccdded5c33f4227911f17a5595392105e27326e3`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 8.8 KB (8773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b6be57bf03bc40983fbb0f78148f99a9c9fc273d643783cc2d9a6ed968b1a`  
		Last Modified: Thu, 04 May 2023 12:06:14 GMT  
		Size: 115.5 MB (115528758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7-enterprise`

```console
$ docker pull neo4j@sha256:16fe2db96720d35739853ca3206a1f3c8ab89c80c89847a818117bb63d2a4259
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:c5374710b0c030a4bb2aeb24063b96defe07fb8c734cee9c02c68d24bc6a917b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **604.1 MB (604135721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251cc4980cb5b46904354ed301f894460a85ee6a9c7c9f7a29caecec5d103240`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:10:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:10:15 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:16 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:32 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:33 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:33 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:33 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:33 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:33 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:33 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069006ee6f68bbfa2f63568d190ac9c3fee8821bf75102d1c1245f45165d65cf`  
		Last Modified: Wed, 03 May 2023 21:11:45 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2168d6eaa4f94cb727d5db4014c9f6b927a996fc32add8714f06f256887f8a`  
		Last Modified: Wed, 03 May 2023 21:11:44 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560b208648ba4f9761e0d4a0810c7912790d2e72c631f5364f5bd3b3b6505a2`  
		Last Modified: Wed, 03 May 2023 21:11:59 GMT  
		Size: 380.1 MB (380139150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:94abe8120c5430ab066aea1692491fa9d4ecf8d504a807510d5498a1562eadfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.4 MB (601449266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d30c05a208e81fc92ba79e35c04df9af40e8950da321169bfa87bf06e621d7d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:05:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:05:06 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:05:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:05:07 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:25 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:25 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73a1fc72b29e2bb1ea0dd76ad5507ef446c37ba2ec53af00c078d2f158d3424`  
		Last Modified: Thu, 04 May 2023 12:06:33 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b19eaac8bbe54d4c8bc4102e86c17dbff7bea7fa395db92ddd87c0dd8ae40c`  
		Last Modified: Thu, 04 May 2023 12:06:33 GMT  
		Size: 8.8 KB (8772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa3fe131fde0ce072e7b87753cf16cd5d86a83e95ebe1ea85581e4b7cf01a8f`  
		Last Modified: Thu, 04 May 2023 12:06:45 GMT  
		Size: 380.0 MB (379996227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7.0`

```console
$ docker pull neo4j@sha256:ed6eb77058badabf0bcfda50da1f2dd5b53314f6afaacaed17eb1b65b64e3b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7.0` - linux; amd64

```console
$ docker pull neo4j@sha256:135374c22967b8b028cfe0ec231e8faa28bb189dcb703f7c13487c6a43ae8722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339670142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc3aa6987130b610e932d5f648d9bcf34ba20f08f2ade3e01358ed68bdafcf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:09:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:09:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:11 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:11 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc29b8a0be2fdad2c0209669f62e4a52c8f1822951fd3606aee9871f291d458`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473676f5c4b0591fda9c3a2dc4d07de297f88ad552f76e8f8c149e35c2d1c5c2`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93765534ca788832bdfd3a07f7f80c9b8272a126028f2b2b9f44bce7399bf5d5`  
		Last Modified: Wed, 03 May 2023 21:11:25 GMT  
		Size: 115.7 MB (115673571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7aa4ae79e62f700964a424d6166309162ad421ea7241cdfef8782cb7b5abf210
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (336981794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6c0929c126c1a2abcd1b5af1ca7420955f76624ac87ea1d5e06f14b84b271`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:04:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:04:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:04:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:04:48 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:01 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:01 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a8328b0b62b333b941f4f72d41fbe9f1cb67c1bdfd42ef100aa881314e839`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ce690ce0b7d3890d98ff9ccdded5c33f4227911f17a5595392105e27326e3`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 8.8 KB (8773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b6be57bf03bc40983fbb0f78148f99a9c9fc273d643783cc2d9a6ed968b1a`  
		Last Modified: Thu, 04 May 2023 12:06:14 GMT  
		Size: 115.5 MB (115528758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7.0-community`

```console
$ docker pull neo4j@sha256:ed6eb77058badabf0bcfda50da1f2dd5b53314f6afaacaed17eb1b65b64e3b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:135374c22967b8b028cfe0ec231e8faa28bb189dcb703f7c13487c6a43ae8722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339670142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc3aa6987130b610e932d5f648d9bcf34ba20f08f2ade3e01358ed68bdafcf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:09:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:09:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:11 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:11 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc29b8a0be2fdad2c0209669f62e4a52c8f1822951fd3606aee9871f291d458`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473676f5c4b0591fda9c3a2dc4d07de297f88ad552f76e8f8c149e35c2d1c5c2`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93765534ca788832bdfd3a07f7f80c9b8272a126028f2b2b9f44bce7399bf5d5`  
		Last Modified: Wed, 03 May 2023 21:11:25 GMT  
		Size: 115.7 MB (115673571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7aa4ae79e62f700964a424d6166309162ad421ea7241cdfef8782cb7b5abf210
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (336981794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6c0929c126c1a2abcd1b5af1ca7420955f76624ac87ea1d5e06f14b84b271`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:04:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:04:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:04:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:04:48 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:01 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:01 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a8328b0b62b333b941f4f72d41fbe9f1cb67c1bdfd42ef100aa881314e839`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ce690ce0b7d3890d98ff9ccdded5c33f4227911f17a5595392105e27326e3`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 8.8 KB (8773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b6be57bf03bc40983fbb0f78148f99a9c9fc273d643783cc2d9a6ed968b1a`  
		Last Modified: Thu, 04 May 2023 12:06:14 GMT  
		Size: 115.5 MB (115528758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7.0-enterprise`

```console
$ docker pull neo4j@sha256:16fe2db96720d35739853ca3206a1f3c8ab89c80c89847a818117bb63d2a4259
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:c5374710b0c030a4bb2aeb24063b96defe07fb8c734cee9c02c68d24bc6a917b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **604.1 MB (604135721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251cc4980cb5b46904354ed301f894460a85ee6a9c7c9f7a29caecec5d103240`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:10:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:10:15 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:16 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:32 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:33 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:33 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:33 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:33 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:33 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:33 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069006ee6f68bbfa2f63568d190ac9c3fee8821bf75102d1c1245f45165d65cf`  
		Last Modified: Wed, 03 May 2023 21:11:45 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2168d6eaa4f94cb727d5db4014c9f6b927a996fc32add8714f06f256887f8a`  
		Last Modified: Wed, 03 May 2023 21:11:44 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560b208648ba4f9761e0d4a0810c7912790d2e72c631f5364f5bd3b3b6505a2`  
		Last Modified: Wed, 03 May 2023 21:11:59 GMT  
		Size: 380.1 MB (380139150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:94abe8120c5430ab066aea1692491fa9d4ecf8d504a807510d5498a1562eadfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.4 MB (601449266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d30c05a208e81fc92ba79e35c04df9af40e8950da321169bfa87bf06e621d7d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:05:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:05:06 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:05:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:05:07 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:25 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:25 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73a1fc72b29e2bb1ea0dd76ad5507ef446c37ba2ec53af00c078d2f158d3424`  
		Last Modified: Thu, 04 May 2023 12:06:33 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b19eaac8bbe54d4c8bc4102e86c17dbff7bea7fa395db92ddd87c0dd8ae40c`  
		Last Modified: Thu, 04 May 2023 12:06:33 GMT  
		Size: 8.8 KB (8772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa3fe131fde0ce072e7b87753cf16cd5d86a83e95ebe1ea85581e4b7cf01a8f`  
		Last Modified: Thu, 04 May 2023 12:06:45 GMT  
		Size: 380.0 MB (379996227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:ed6eb77058badabf0bcfda50da1f2dd5b53314f6afaacaed17eb1b65b64e3b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:135374c22967b8b028cfe0ec231e8faa28bb189dcb703f7c13487c6a43ae8722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339670142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc3aa6987130b610e932d5f648d9bcf34ba20f08f2ade3e01358ed68bdafcf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:09:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:09:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:11 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:11 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc29b8a0be2fdad2c0209669f62e4a52c8f1822951fd3606aee9871f291d458`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473676f5c4b0591fda9c3a2dc4d07de297f88ad552f76e8f8c149e35c2d1c5c2`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93765534ca788832bdfd3a07f7f80c9b8272a126028f2b2b9f44bce7399bf5d5`  
		Last Modified: Wed, 03 May 2023 21:11:25 GMT  
		Size: 115.7 MB (115673571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7aa4ae79e62f700964a424d6166309162ad421ea7241cdfef8782cb7b5abf210
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (336981794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6c0929c126c1a2abcd1b5af1ca7420955f76624ac87ea1d5e06f14b84b271`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:04:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:04:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:04:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:04:48 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:01 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:01 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a8328b0b62b333b941f4f72d41fbe9f1cb67c1bdfd42ef100aa881314e839`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ce690ce0b7d3890d98ff9ccdded5c33f4227911f17a5595392105e27326e3`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 8.8 KB (8773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b6be57bf03bc40983fbb0f78148f99a9c9fc273d643783cc2d9a6ed968b1a`  
		Last Modified: Thu, 04 May 2023 12:06:14 GMT  
		Size: 115.5 MB (115528758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:16fe2db96720d35739853ca3206a1f3c8ab89c80c89847a818117bb63d2a4259
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:c5374710b0c030a4bb2aeb24063b96defe07fb8c734cee9c02c68d24bc6a917b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **604.1 MB (604135721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251cc4980cb5b46904354ed301f894460a85ee6a9c7c9f7a29caecec5d103240`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:10:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:10:15 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:16 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:32 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:33 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:33 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:33 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:33 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:33 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:33 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069006ee6f68bbfa2f63568d190ac9c3fee8821bf75102d1c1245f45165d65cf`  
		Last Modified: Wed, 03 May 2023 21:11:45 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2168d6eaa4f94cb727d5db4014c9f6b927a996fc32add8714f06f256887f8a`  
		Last Modified: Wed, 03 May 2023 21:11:44 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560b208648ba4f9761e0d4a0810c7912790d2e72c631f5364f5bd3b3b6505a2`  
		Last Modified: Wed, 03 May 2023 21:11:59 GMT  
		Size: 380.1 MB (380139150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:94abe8120c5430ab066aea1692491fa9d4ecf8d504a807510d5498a1562eadfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.4 MB (601449266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d30c05a208e81fc92ba79e35c04df9af40e8950da321169bfa87bf06e621d7d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:05:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:05:06 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:05:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:05:07 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:25 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:25 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73a1fc72b29e2bb1ea0dd76ad5507ef446c37ba2ec53af00c078d2f158d3424`  
		Last Modified: Thu, 04 May 2023 12:06:33 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b19eaac8bbe54d4c8bc4102e86c17dbff7bea7fa395db92ddd87c0dd8ae40c`  
		Last Modified: Thu, 04 May 2023 12:06:33 GMT  
		Size: 8.8 KB (8772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa3fe131fde0ce072e7b87753cf16cd5d86a83e95ebe1ea85581e4b7cf01a8f`  
		Last Modified: Thu, 04 May 2023 12:06:45 GMT  
		Size: 380.0 MB (379996227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:ed6eb77058badabf0bcfda50da1f2dd5b53314f6afaacaed17eb1b65b64e3b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:135374c22967b8b028cfe0ec231e8faa28bb189dcb703f7c13487c6a43ae8722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339670142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc3aa6987130b610e932d5f648d9bcf34ba20f08f2ade3e01358ed68bdafcf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:09:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:09:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:11 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:11 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc29b8a0be2fdad2c0209669f62e4a52c8f1822951fd3606aee9871f291d458`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473676f5c4b0591fda9c3a2dc4d07de297f88ad552f76e8f8c149e35c2d1c5c2`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93765534ca788832bdfd3a07f7f80c9b8272a126028f2b2b9f44bce7399bf5d5`  
		Last Modified: Wed, 03 May 2023 21:11:25 GMT  
		Size: 115.7 MB (115673571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7aa4ae79e62f700964a424d6166309162ad421ea7241cdfef8782cb7b5abf210
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (336981794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6c0929c126c1a2abcd1b5af1ca7420955f76624ac87ea1d5e06f14b84b271`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 12:04:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:04:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:04:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:04:48 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:01 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:01 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a8328b0b62b333b941f4f72d41fbe9f1cb67c1bdfd42ef100aa881314e839`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ce690ce0b7d3890d98ff9ccdded5c33f4227911f17a5595392105e27326e3`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 8.8 KB (8773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b6be57bf03bc40983fbb0f78148f99a9c9fc273d643783cc2d9a6ed968b1a`  
		Last Modified: Thu, 04 May 2023 12:06:14 GMT  
		Size: 115.5 MB (115528758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
