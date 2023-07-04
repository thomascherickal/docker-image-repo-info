<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.22`](#neo4j4422)
-	[`neo4j:4.4.22-community`](#neo4j4422-community)
-	[`neo4j:4.4.22-enterprise`](#neo4j4422-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5.9`](#neo4j59)
-	[`neo4j:5.9-community`](#neo4j59-community)
-	[`neo4j:5.9-enterprise`](#neo4j59-enterprise)
-	[`neo4j:5.9.0`](#neo4j590)
-	[`neo4j:5.9.0-community`](#neo4j590-community)
-	[`neo4j:5.9.0-enterprise`](#neo4j590-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:8ce245ad271d33ffeb6f7abd48abd30b15607747af41923ce332def367cb93f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:b03b67d179ada54e57856a3547e51a3d1a58554ab7ca09a8616973c2cdd887ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.4 MB (348437813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6099945ca974cace482bc4ee5d5a56827380cb10a800b2a69dea8de566aed6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:03:33 GMT
COPY dir:8166f0419dcb1797526932f102a2cde39418897507eef5904ae1b596b03e4941 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:21:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a4a150531e421f7bd24a00b3cfb8d923b898035f2ac987c68ead7d69ef321b06 NEO4J_TARBALL=neo4j-community-4.4.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:21:24 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 17:21:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:21:25 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 17:21:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:21:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:21:36 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:21:37 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:21:37 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:21:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:21:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d40bd43d5fd5578d52b821d800d9245b2c75c4719bd86ef77c02cb13aa774`  
		Last Modified: Tue, 04 Jul 2023 04:13:44 GMT  
		Size: 198.5 MB (198549452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fc4637f52cb05a3b31c2efa74b4c2ad78074d695dc8ec3e7130797b6c23855`  
		Last Modified: Tue, 04 Jul 2023 17:23:11 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb30f4cc53e96cbd00eee7f1b7cda8c4642e1259dc2e38535e1ed6c06eefc05`  
		Last Modified: Tue, 04 Jul 2023 17:23:11 GMT  
		Size: 9.3 KB (9326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569dc57ff3a67f067a0f1d7c96b40a6eb791f8715d1e37eb2bce57cedb9d14a5`  
		Last Modified: Tue, 04 Jul 2023 17:23:16 GMT  
		Size: 118.5 MB (118457791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bd5c788f5bcefb559ea421f817147ae97e150b2d4a3e357fec15c6f109db582
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343751784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3f46b3f22be2c2a71de1805a81006eec2cd572e16265009b360b5daa8fb817`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:35:19 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:35:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a4a150531e421f7bd24a00b3cfb8d923b898035f2ac987c68ead7d69ef321b06 NEO4J_TARBALL=neo4j-community-4.4.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:35:23 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 06:35:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:35:24 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 06:35:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:35:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:35:38 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:35:39 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:35:39 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:35:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:35:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fccefcb482635b3259449981a784fc2012a529dac3559c916400e0c1558529`  
		Last Modified: Tue, 04 Jul 2023 06:37:25 GMT  
		Size: 195.3 MB (195324205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97973f720365351bb1affd42f5b336dab6f3f77029b84df579d53ef7eb5467a`  
		Last Modified: Tue, 04 Jul 2023 06:37:14 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef5344b0adba04a5da63e6fa7b7b4b78d1e41aaf532ac6e64169feb1c160680`  
		Last Modified: Tue, 04 Jul 2023 06:37:14 GMT  
		Size: 9.3 KB (9327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544d9b78c5f43953f3e27950c8a04dab4b295dda8095a6c8bfda44221f1c818f`  
		Last Modified: Tue, 04 Jul 2023 06:37:18 GMT  
		Size: 118.4 MB (118351410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:8ce245ad271d33ffeb6f7abd48abd30b15607747af41923ce332def367cb93f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:b03b67d179ada54e57856a3547e51a3d1a58554ab7ca09a8616973c2cdd887ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.4 MB (348437813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6099945ca974cace482bc4ee5d5a56827380cb10a800b2a69dea8de566aed6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:03:33 GMT
COPY dir:8166f0419dcb1797526932f102a2cde39418897507eef5904ae1b596b03e4941 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:21:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a4a150531e421f7bd24a00b3cfb8d923b898035f2ac987c68ead7d69ef321b06 NEO4J_TARBALL=neo4j-community-4.4.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:21:24 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 17:21:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:21:25 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 17:21:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:21:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:21:36 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:21:37 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:21:37 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:21:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:21:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d40bd43d5fd5578d52b821d800d9245b2c75c4719bd86ef77c02cb13aa774`  
		Last Modified: Tue, 04 Jul 2023 04:13:44 GMT  
		Size: 198.5 MB (198549452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fc4637f52cb05a3b31c2efa74b4c2ad78074d695dc8ec3e7130797b6c23855`  
		Last Modified: Tue, 04 Jul 2023 17:23:11 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb30f4cc53e96cbd00eee7f1b7cda8c4642e1259dc2e38535e1ed6c06eefc05`  
		Last Modified: Tue, 04 Jul 2023 17:23:11 GMT  
		Size: 9.3 KB (9326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569dc57ff3a67f067a0f1d7c96b40a6eb791f8715d1e37eb2bce57cedb9d14a5`  
		Last Modified: Tue, 04 Jul 2023 17:23:16 GMT  
		Size: 118.5 MB (118457791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bd5c788f5bcefb559ea421f817147ae97e150b2d4a3e357fec15c6f109db582
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343751784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3f46b3f22be2c2a71de1805a81006eec2cd572e16265009b360b5daa8fb817`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:35:19 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:35:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a4a150531e421f7bd24a00b3cfb8d923b898035f2ac987c68ead7d69ef321b06 NEO4J_TARBALL=neo4j-community-4.4.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:35:23 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 06:35:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:35:24 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 06:35:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:35:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:35:38 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:35:39 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:35:39 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:35:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:35:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fccefcb482635b3259449981a784fc2012a529dac3559c916400e0c1558529`  
		Last Modified: Tue, 04 Jul 2023 06:37:25 GMT  
		Size: 195.3 MB (195324205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97973f720365351bb1affd42f5b336dab6f3f77029b84df579d53ef7eb5467a`  
		Last Modified: Tue, 04 Jul 2023 06:37:14 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef5344b0adba04a5da63e6fa7b7b4b78d1e41aaf532ac6e64169feb1c160680`  
		Last Modified: Tue, 04 Jul 2023 06:37:14 GMT  
		Size: 9.3 KB (9327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544d9b78c5f43953f3e27950c8a04dab4b295dda8095a6c8bfda44221f1c818f`  
		Last Modified: Tue, 04 Jul 2023 06:37:18 GMT  
		Size: 118.4 MB (118351410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:c415ed12c7499165e0b6d2639d049f4e9859451c193179e15ba53a597482772a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:8c03ae027c79fd4bbc009aab8110f1b12bc11bf4a427f2c2e050036693419fa7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.8 MB (447762090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231c7e766cc52e413255c4cc683b5aa13f800a2297f8f531fed7a4b41aec95f3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:03:33 GMT
COPY dir:8166f0419dcb1797526932f102a2cde39418897507eef5904ae1b596b03e4941 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:21:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ec49ac0f429a7e05ab21e48c8bc6273274c82df6f75221b85cec0c53a51ef840 NEO4J_TARBALL=neo4j-enterprise-4.4.22-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:21:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 17:21:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:21:42 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 17:21:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:21:56 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:21:56 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:21:56 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:21:56 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:21:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:21:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d40bd43d5fd5578d52b821d800d9245b2c75c4719bd86ef77c02cb13aa774`  
		Last Modified: Tue, 04 Jul 2023 04:13:44 GMT  
		Size: 198.5 MB (198549452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df50bf288e8d6df9ab9fd4a4c7d826483fb8f73c9e280f420a13fb1dd00db3c5`  
		Last Modified: Tue, 04 Jul 2023 17:23:28 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af43be9174b5d82b31e944fb8ad8b38a21f2f65eaeaca64135e3df235d35cbc`  
		Last Modified: Tue, 04 Jul 2023 17:23:28 GMT  
		Size: 9.3 KB (9327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ae20830e8149e841dc81c9d58948f776b95b79ed734dab27963f99af3f01bc`  
		Last Modified: Tue, 04 Jul 2023 17:23:38 GMT  
		Size: 217.8 MB (217782067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6b113164787c72acb401288cc539a2c63e89d77c19b7b34bede60aee492b039f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.1 MB (443074102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d35c8b2d8322767d72d1b0ac2cb53d3af201760e97732b0d38fa09e81c0d6bf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:35:19 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:35:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ec49ac0f429a7e05ab21e48c8bc6273274c82df6f75221b85cec0c53a51ef840 NEO4J_TARBALL=neo4j-enterprise-4.4.22-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:35:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 06:35:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:35:45 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 06:36:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:36:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:36:06 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:36:06 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:36:06 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:36:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:36:06 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fccefcb482635b3259449981a784fc2012a529dac3559c916400e0c1558529`  
		Last Modified: Tue, 04 Jul 2023 06:37:25 GMT  
		Size: 195.3 MB (195324205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835e3da3584541f879967b51d01d72f998910e7ce61a1e8b2b2c90f90cfeb12c`  
		Last Modified: Tue, 04 Jul 2023 06:37:36 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e024cb6cf7ad1f191de432829ecaf90718ee764c6714a481b7cc124b955377`  
		Last Modified: Tue, 04 Jul 2023 06:37:36 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489287abfe63d498bca83f108d8f16fe6d934c0beb71a0446669965b19117cb7`  
		Last Modified: Tue, 04 Jul 2023 06:37:44 GMT  
		Size: 217.7 MB (217673731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.22`

```console
$ docker pull neo4j@sha256:8ce245ad271d33ffeb6f7abd48abd30b15607747af41923ce332def367cb93f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.22` - linux; amd64

```console
$ docker pull neo4j@sha256:b03b67d179ada54e57856a3547e51a3d1a58554ab7ca09a8616973c2cdd887ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.4 MB (348437813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6099945ca974cace482bc4ee5d5a56827380cb10a800b2a69dea8de566aed6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:03:33 GMT
COPY dir:8166f0419dcb1797526932f102a2cde39418897507eef5904ae1b596b03e4941 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:21:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a4a150531e421f7bd24a00b3cfb8d923b898035f2ac987c68ead7d69ef321b06 NEO4J_TARBALL=neo4j-community-4.4.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:21:24 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 17:21:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:21:25 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 17:21:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:21:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:21:36 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:21:37 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:21:37 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:21:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:21:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d40bd43d5fd5578d52b821d800d9245b2c75c4719bd86ef77c02cb13aa774`  
		Last Modified: Tue, 04 Jul 2023 04:13:44 GMT  
		Size: 198.5 MB (198549452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fc4637f52cb05a3b31c2efa74b4c2ad78074d695dc8ec3e7130797b6c23855`  
		Last Modified: Tue, 04 Jul 2023 17:23:11 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb30f4cc53e96cbd00eee7f1b7cda8c4642e1259dc2e38535e1ed6c06eefc05`  
		Last Modified: Tue, 04 Jul 2023 17:23:11 GMT  
		Size: 9.3 KB (9326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569dc57ff3a67f067a0f1d7c96b40a6eb791f8715d1e37eb2bce57cedb9d14a5`  
		Last Modified: Tue, 04 Jul 2023 17:23:16 GMT  
		Size: 118.5 MB (118457791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.22` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bd5c788f5bcefb559ea421f817147ae97e150b2d4a3e357fec15c6f109db582
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343751784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3f46b3f22be2c2a71de1805a81006eec2cd572e16265009b360b5daa8fb817`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:35:19 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:35:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a4a150531e421f7bd24a00b3cfb8d923b898035f2ac987c68ead7d69ef321b06 NEO4J_TARBALL=neo4j-community-4.4.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:35:23 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 06:35:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:35:24 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 06:35:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:35:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:35:38 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:35:39 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:35:39 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:35:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:35:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fccefcb482635b3259449981a784fc2012a529dac3559c916400e0c1558529`  
		Last Modified: Tue, 04 Jul 2023 06:37:25 GMT  
		Size: 195.3 MB (195324205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97973f720365351bb1affd42f5b336dab6f3f77029b84df579d53ef7eb5467a`  
		Last Modified: Tue, 04 Jul 2023 06:37:14 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef5344b0adba04a5da63e6fa7b7b4b78d1e41aaf532ac6e64169feb1c160680`  
		Last Modified: Tue, 04 Jul 2023 06:37:14 GMT  
		Size: 9.3 KB (9327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544d9b78c5f43953f3e27950c8a04dab4b295dda8095a6c8bfda44221f1c818f`  
		Last Modified: Tue, 04 Jul 2023 06:37:18 GMT  
		Size: 118.4 MB (118351410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.22-community`

```console
$ docker pull neo4j@sha256:8ce245ad271d33ffeb6f7abd48abd30b15607747af41923ce332def367cb93f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.22-community` - linux; amd64

```console
$ docker pull neo4j@sha256:b03b67d179ada54e57856a3547e51a3d1a58554ab7ca09a8616973c2cdd887ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.4 MB (348437813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6099945ca974cace482bc4ee5d5a56827380cb10a800b2a69dea8de566aed6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:03:33 GMT
COPY dir:8166f0419dcb1797526932f102a2cde39418897507eef5904ae1b596b03e4941 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:21:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a4a150531e421f7bd24a00b3cfb8d923b898035f2ac987c68ead7d69ef321b06 NEO4J_TARBALL=neo4j-community-4.4.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:21:24 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 17:21:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:21:25 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 17:21:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:21:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:21:36 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:21:37 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:21:37 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:21:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:21:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d40bd43d5fd5578d52b821d800d9245b2c75c4719bd86ef77c02cb13aa774`  
		Last Modified: Tue, 04 Jul 2023 04:13:44 GMT  
		Size: 198.5 MB (198549452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fc4637f52cb05a3b31c2efa74b4c2ad78074d695dc8ec3e7130797b6c23855`  
		Last Modified: Tue, 04 Jul 2023 17:23:11 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb30f4cc53e96cbd00eee7f1b7cda8c4642e1259dc2e38535e1ed6c06eefc05`  
		Last Modified: Tue, 04 Jul 2023 17:23:11 GMT  
		Size: 9.3 KB (9326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569dc57ff3a67f067a0f1d7c96b40a6eb791f8715d1e37eb2bce57cedb9d14a5`  
		Last Modified: Tue, 04 Jul 2023 17:23:16 GMT  
		Size: 118.5 MB (118457791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.22-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bd5c788f5bcefb559ea421f817147ae97e150b2d4a3e357fec15c6f109db582
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343751784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3f46b3f22be2c2a71de1805a81006eec2cd572e16265009b360b5daa8fb817`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:35:19 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:35:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a4a150531e421f7bd24a00b3cfb8d923b898035f2ac987c68ead7d69ef321b06 NEO4J_TARBALL=neo4j-community-4.4.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:35:23 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 06:35:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:35:24 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 06:35:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:35:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:35:38 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:35:39 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:35:39 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:35:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:35:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fccefcb482635b3259449981a784fc2012a529dac3559c916400e0c1558529`  
		Last Modified: Tue, 04 Jul 2023 06:37:25 GMT  
		Size: 195.3 MB (195324205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97973f720365351bb1affd42f5b336dab6f3f77029b84df579d53ef7eb5467a`  
		Last Modified: Tue, 04 Jul 2023 06:37:14 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef5344b0adba04a5da63e6fa7b7b4b78d1e41aaf532ac6e64169feb1c160680`  
		Last Modified: Tue, 04 Jul 2023 06:37:14 GMT  
		Size: 9.3 KB (9327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544d9b78c5f43953f3e27950c8a04dab4b295dda8095a6c8bfda44221f1c818f`  
		Last Modified: Tue, 04 Jul 2023 06:37:18 GMT  
		Size: 118.4 MB (118351410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.22-enterprise`

```console
$ docker pull neo4j@sha256:c415ed12c7499165e0b6d2639d049f4e9859451c193179e15ba53a597482772a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.22-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:8c03ae027c79fd4bbc009aab8110f1b12bc11bf4a427f2c2e050036693419fa7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.8 MB (447762090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231c7e766cc52e413255c4cc683b5aa13f800a2297f8f531fed7a4b41aec95f3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:03:33 GMT
COPY dir:8166f0419dcb1797526932f102a2cde39418897507eef5904ae1b596b03e4941 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:21:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ec49ac0f429a7e05ab21e48c8bc6273274c82df6f75221b85cec0c53a51ef840 NEO4J_TARBALL=neo4j-enterprise-4.4.22-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:21:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 17:21:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:21:42 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 17:21:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:21:56 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:21:56 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:21:56 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:21:56 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:21:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:21:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d40bd43d5fd5578d52b821d800d9245b2c75c4719bd86ef77c02cb13aa774`  
		Last Modified: Tue, 04 Jul 2023 04:13:44 GMT  
		Size: 198.5 MB (198549452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df50bf288e8d6df9ab9fd4a4c7d826483fb8f73c9e280f420a13fb1dd00db3c5`  
		Last Modified: Tue, 04 Jul 2023 17:23:28 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af43be9174b5d82b31e944fb8ad8b38a21f2f65eaeaca64135e3df235d35cbc`  
		Last Modified: Tue, 04 Jul 2023 17:23:28 GMT  
		Size: 9.3 KB (9327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ae20830e8149e841dc81c9d58948f776b95b79ed734dab27963f99af3f01bc`  
		Last Modified: Tue, 04 Jul 2023 17:23:38 GMT  
		Size: 217.8 MB (217782067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.22-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6b113164787c72acb401288cc539a2c63e89d77c19b7b34bede60aee492b039f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.1 MB (443074102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d35c8b2d8322767d72d1b0ac2cb53d3af201760e97732b0d38fa09e81c0d6bf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:35:19 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:35:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ec49ac0f429a7e05ab21e48c8bc6273274c82df6f75221b85cec0c53a51ef840 NEO4J_TARBALL=neo4j-enterprise-4.4.22-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:35:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
# Tue, 04 Jul 2023 06:35:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:35:45 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Tue, 04 Jul 2023 06:36:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:36:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:36:06 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:36:06 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:36:06 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:36:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:36:06 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fccefcb482635b3259449981a784fc2012a529dac3559c916400e0c1558529`  
		Last Modified: Tue, 04 Jul 2023 06:37:25 GMT  
		Size: 195.3 MB (195324205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835e3da3584541f879967b51d01d72f998910e7ce61a1e8b2b2c90f90cfeb12c`  
		Last Modified: Tue, 04 Jul 2023 06:37:36 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e024cb6cf7ad1f191de432829ecaf90718ee764c6714a481b7cc124b955377`  
		Last Modified: Tue, 04 Jul 2023 06:37:36 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489287abfe63d498bca83f108d8f16fe6d934c0beb71a0446669965b19117cb7`  
		Last Modified: Tue, 04 Jul 2023 06:37:44 GMT  
		Size: 217.7 MB (217673731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:93684114e9961735c1312802d88b6295a75b425a2f5826cb8248529b8f06921f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:56ceb318b79315af073cad11c39446c99530c1b051e7006e18a4ca805383cc52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339764620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6225dd46452249271ff53463cd4c962b7f5645214423fec46a4162295a8bf435`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:20:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:20:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:20:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:20:44 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:20:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:20:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:20:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:20:57 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:20:57 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afa9b3f536783089b8230b0cd2bc0eb9727b192b071a19f0fbe7c91dcf940bb`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacc8baa2aac9c647538ceb39c1e59c611d6e43b9215dfcc30fcbbe64cc6eb0`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 9.4 KB (9368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6c0fb808423cc74fd89f637d31c471ef2893be64d3c47503ee0ad8030c997f`  
		Last Modified: Tue, 04 Jul 2023 17:22:23 GMT  
		Size: 115.8 MB (115753701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:ab9c060c7ff61a54b35a7b38fc09f4cb143f210c2c7711c04d19802b0b97f10f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337110137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2aa94390a4d91363d5896f5f9c83921b57d038fa1fefc849bf32f4c662ab5d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:33 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:34:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:34:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:34:48 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:34:49 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:34:49 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:34:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:34:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31bbf0eb561b1650f22e928cbeccb17872671effa64cad96c568923c773c5e1`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7602e07641dac1311b8a2427efdb849b9749894a1a9ed64979931ed3d6f03bdc`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925b08e9954cc34ec2861c0b6ea5ade09ae1a9361db08e6c22d2c5eba5010b65`  
		Last Modified: Tue, 04 Jul 2023 06:36:23 GMT  
		Size: 115.6 MB (115646236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:93684114e9961735c1312802d88b6295a75b425a2f5826cb8248529b8f06921f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:56ceb318b79315af073cad11c39446c99530c1b051e7006e18a4ca805383cc52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339764620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6225dd46452249271ff53463cd4c962b7f5645214423fec46a4162295a8bf435`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:20:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:20:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:20:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:20:44 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:20:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:20:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:20:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:20:57 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:20:57 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afa9b3f536783089b8230b0cd2bc0eb9727b192b071a19f0fbe7c91dcf940bb`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacc8baa2aac9c647538ceb39c1e59c611d6e43b9215dfcc30fcbbe64cc6eb0`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 9.4 KB (9368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6c0fb808423cc74fd89f637d31c471ef2893be64d3c47503ee0ad8030c997f`  
		Last Modified: Tue, 04 Jul 2023 17:22:23 GMT  
		Size: 115.8 MB (115753701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:ab9c060c7ff61a54b35a7b38fc09f4cb143f210c2c7711c04d19802b0b97f10f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337110137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2aa94390a4d91363d5896f5f9c83921b57d038fa1fefc849bf32f4c662ab5d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:33 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:34:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:34:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:34:48 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:34:49 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:34:49 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:34:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:34:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31bbf0eb561b1650f22e928cbeccb17872671effa64cad96c568923c773c5e1`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7602e07641dac1311b8a2427efdb849b9749894a1a9ed64979931ed3d6f03bdc`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925b08e9954cc34ec2861c0b6ea5ade09ae1a9361db08e6c22d2c5eba5010b65`  
		Last Modified: Tue, 04 Jul 2023 06:36:23 GMT  
		Size: 115.6 MB (115646236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:6b96a248881100cc1933ed1e2f876ca17ac8138028950815824834afab757599
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ea1c4453a2053b97b8cb06ad56df3c30d9180661156fed9e14bcea4bbc2418ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.7 MB (617745671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e5444ff1b29cf9fefef7604273556c2d43cb3354fbbff37cd7f0abc235e60f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:21:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=978819870e976f903ecfb68a8e22ee5ea498779ee14a0c4d9f0f98fc29230ccb NEO4J_TARBALL=neo4j-enterprise-5.9.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:21:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:21:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:21:01 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:21:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:21:19 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:21:19 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:21:19 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:21:19 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:21:20 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:21:20 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18d4eb232eb5306440a582c9f2d9610be6c51d5518cd4d1c3472e1cc0de40c`  
		Last Modified: Tue, 04 Jul 2023 17:22:43 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947e093535bfa8b8393da45080bde93dc7cb2ffa768b256e5bd081bf7436a20`  
		Last Modified: Tue, 04 Jul 2023 17:22:43 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3943ee1048805605e62569fb57f45ee82a4907e06b48e47b6066e7f02c46449`  
		Last Modified: Tue, 04 Jul 2023 17:22:59 GMT  
		Size: 393.7 MB (393734749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:34ccc1bd75af18944b35db27f14a3747b099d89c062ebbae6d1ce13b4c3afd1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **615.1 MB (615092882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a0584d04469afc9b6f9b5dabf6d8c470fa180ae3aeb3b7a28fd24a8ae6e59e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=978819870e976f903ecfb68a8e22ee5ea498779ee14a0c4d9f0f98fc29230ccb NEO4J_TARBALL=neo4j-enterprise-5.9.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:53 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:54 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:35:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:35:13 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:35:13 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:35:13 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:35:14 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:35:14 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:35:14 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd0804164ff5a7a8bac70caaa09e39349c9e0dbb8baef6d0ff03058ca910cac`  
		Last Modified: Tue, 04 Jul 2023 06:36:48 GMT  
		Size: 3.9 KB (3892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a8710006fb7822fddd6ed807ef02ffd3ec563cea959c37a3bf53fca4f7d956`  
		Last Modified: Tue, 04 Jul 2023 06:36:49 GMT  
		Size: 9.4 KB (9370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38a745a710edaf1eadcb2d76e64bd6030fb941963f87a919d7e899aaee490fa`  
		Last Modified: Tue, 04 Jul 2023 06:37:02 GMT  
		Size: 393.6 MB (393628976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.9`

```console
$ docker pull neo4j@sha256:93684114e9961735c1312802d88b6295a75b425a2f5826cb8248529b8f06921f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.9` - linux; amd64

```console
$ docker pull neo4j@sha256:56ceb318b79315af073cad11c39446c99530c1b051e7006e18a4ca805383cc52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339764620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6225dd46452249271ff53463cd4c962b7f5645214423fec46a4162295a8bf435`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:20:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:20:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:20:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:20:44 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:20:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:20:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:20:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:20:57 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:20:57 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afa9b3f536783089b8230b0cd2bc0eb9727b192b071a19f0fbe7c91dcf940bb`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacc8baa2aac9c647538ceb39c1e59c611d6e43b9215dfcc30fcbbe64cc6eb0`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 9.4 KB (9368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6c0fb808423cc74fd89f637d31c471ef2893be64d3c47503ee0ad8030c997f`  
		Last Modified: Tue, 04 Jul 2023 17:22:23 GMT  
		Size: 115.8 MB (115753701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.9` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:ab9c060c7ff61a54b35a7b38fc09f4cb143f210c2c7711c04d19802b0b97f10f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337110137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2aa94390a4d91363d5896f5f9c83921b57d038fa1fefc849bf32f4c662ab5d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:33 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:34:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:34:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:34:48 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:34:49 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:34:49 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:34:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:34:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31bbf0eb561b1650f22e928cbeccb17872671effa64cad96c568923c773c5e1`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7602e07641dac1311b8a2427efdb849b9749894a1a9ed64979931ed3d6f03bdc`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925b08e9954cc34ec2861c0b6ea5ade09ae1a9361db08e6c22d2c5eba5010b65`  
		Last Modified: Tue, 04 Jul 2023 06:36:23 GMT  
		Size: 115.6 MB (115646236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.9-community`

```console
$ docker pull neo4j@sha256:93684114e9961735c1312802d88b6295a75b425a2f5826cb8248529b8f06921f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.9-community` - linux; amd64

```console
$ docker pull neo4j@sha256:56ceb318b79315af073cad11c39446c99530c1b051e7006e18a4ca805383cc52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339764620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6225dd46452249271ff53463cd4c962b7f5645214423fec46a4162295a8bf435`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:20:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:20:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:20:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:20:44 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:20:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:20:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:20:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:20:57 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:20:57 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afa9b3f536783089b8230b0cd2bc0eb9727b192b071a19f0fbe7c91dcf940bb`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacc8baa2aac9c647538ceb39c1e59c611d6e43b9215dfcc30fcbbe64cc6eb0`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 9.4 KB (9368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6c0fb808423cc74fd89f637d31c471ef2893be64d3c47503ee0ad8030c997f`  
		Last Modified: Tue, 04 Jul 2023 17:22:23 GMT  
		Size: 115.8 MB (115753701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.9-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:ab9c060c7ff61a54b35a7b38fc09f4cb143f210c2c7711c04d19802b0b97f10f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337110137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2aa94390a4d91363d5896f5f9c83921b57d038fa1fefc849bf32f4c662ab5d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:33 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:34:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:34:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:34:48 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:34:49 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:34:49 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:34:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:34:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31bbf0eb561b1650f22e928cbeccb17872671effa64cad96c568923c773c5e1`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7602e07641dac1311b8a2427efdb849b9749894a1a9ed64979931ed3d6f03bdc`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925b08e9954cc34ec2861c0b6ea5ade09ae1a9361db08e6c22d2c5eba5010b65`  
		Last Modified: Tue, 04 Jul 2023 06:36:23 GMT  
		Size: 115.6 MB (115646236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.9-enterprise`

```console
$ docker pull neo4j@sha256:6b96a248881100cc1933ed1e2f876ca17ac8138028950815824834afab757599
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.9-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ea1c4453a2053b97b8cb06ad56df3c30d9180661156fed9e14bcea4bbc2418ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.7 MB (617745671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e5444ff1b29cf9fefef7604273556c2d43cb3354fbbff37cd7f0abc235e60f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:21:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=978819870e976f903ecfb68a8e22ee5ea498779ee14a0c4d9f0f98fc29230ccb NEO4J_TARBALL=neo4j-enterprise-5.9.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:21:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:21:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:21:01 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:21:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:21:19 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:21:19 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:21:19 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:21:19 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:21:20 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:21:20 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18d4eb232eb5306440a582c9f2d9610be6c51d5518cd4d1c3472e1cc0de40c`  
		Last Modified: Tue, 04 Jul 2023 17:22:43 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947e093535bfa8b8393da45080bde93dc7cb2ffa768b256e5bd081bf7436a20`  
		Last Modified: Tue, 04 Jul 2023 17:22:43 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3943ee1048805605e62569fb57f45ee82a4907e06b48e47b6066e7f02c46449`  
		Last Modified: Tue, 04 Jul 2023 17:22:59 GMT  
		Size: 393.7 MB (393734749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.9-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:34ccc1bd75af18944b35db27f14a3747b099d89c062ebbae6d1ce13b4c3afd1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **615.1 MB (615092882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a0584d04469afc9b6f9b5dabf6d8c470fa180ae3aeb3b7a28fd24a8ae6e59e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=978819870e976f903ecfb68a8e22ee5ea498779ee14a0c4d9f0f98fc29230ccb NEO4J_TARBALL=neo4j-enterprise-5.9.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:53 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:54 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:35:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:35:13 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:35:13 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:35:13 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:35:14 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:35:14 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:35:14 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd0804164ff5a7a8bac70caaa09e39349c9e0dbb8baef6d0ff03058ca910cac`  
		Last Modified: Tue, 04 Jul 2023 06:36:48 GMT  
		Size: 3.9 KB (3892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a8710006fb7822fddd6ed807ef02ffd3ec563cea959c37a3bf53fca4f7d956`  
		Last Modified: Tue, 04 Jul 2023 06:36:49 GMT  
		Size: 9.4 KB (9370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38a745a710edaf1eadcb2d76e64bd6030fb941963f87a919d7e899aaee490fa`  
		Last Modified: Tue, 04 Jul 2023 06:37:02 GMT  
		Size: 393.6 MB (393628976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.9.0`

```console
$ docker pull neo4j@sha256:93684114e9961735c1312802d88b6295a75b425a2f5826cb8248529b8f06921f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.9.0` - linux; amd64

```console
$ docker pull neo4j@sha256:56ceb318b79315af073cad11c39446c99530c1b051e7006e18a4ca805383cc52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339764620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6225dd46452249271ff53463cd4c962b7f5645214423fec46a4162295a8bf435`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:20:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:20:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:20:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:20:44 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:20:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:20:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:20:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:20:57 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:20:57 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afa9b3f536783089b8230b0cd2bc0eb9727b192b071a19f0fbe7c91dcf940bb`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacc8baa2aac9c647538ceb39c1e59c611d6e43b9215dfcc30fcbbe64cc6eb0`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 9.4 KB (9368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6c0fb808423cc74fd89f637d31c471ef2893be64d3c47503ee0ad8030c997f`  
		Last Modified: Tue, 04 Jul 2023 17:22:23 GMT  
		Size: 115.8 MB (115753701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.9.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:ab9c060c7ff61a54b35a7b38fc09f4cb143f210c2c7711c04d19802b0b97f10f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337110137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2aa94390a4d91363d5896f5f9c83921b57d038fa1fefc849bf32f4c662ab5d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:33 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:34:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:34:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:34:48 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:34:49 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:34:49 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:34:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:34:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31bbf0eb561b1650f22e928cbeccb17872671effa64cad96c568923c773c5e1`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7602e07641dac1311b8a2427efdb849b9749894a1a9ed64979931ed3d6f03bdc`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925b08e9954cc34ec2861c0b6ea5ade09ae1a9361db08e6c22d2c5eba5010b65`  
		Last Modified: Tue, 04 Jul 2023 06:36:23 GMT  
		Size: 115.6 MB (115646236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.9.0-community`

```console
$ docker pull neo4j@sha256:93684114e9961735c1312802d88b6295a75b425a2f5826cb8248529b8f06921f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.9.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:56ceb318b79315af073cad11c39446c99530c1b051e7006e18a4ca805383cc52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339764620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6225dd46452249271ff53463cd4c962b7f5645214423fec46a4162295a8bf435`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:20:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:20:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:20:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:20:44 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:20:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:20:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:20:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:20:57 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:20:57 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afa9b3f536783089b8230b0cd2bc0eb9727b192b071a19f0fbe7c91dcf940bb`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacc8baa2aac9c647538ceb39c1e59c611d6e43b9215dfcc30fcbbe64cc6eb0`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 9.4 KB (9368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6c0fb808423cc74fd89f637d31c471ef2893be64d3c47503ee0ad8030c997f`  
		Last Modified: Tue, 04 Jul 2023 17:22:23 GMT  
		Size: 115.8 MB (115753701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.9.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:ab9c060c7ff61a54b35a7b38fc09f4cb143f210c2c7711c04d19802b0b97f10f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337110137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2aa94390a4d91363d5896f5f9c83921b57d038fa1fefc849bf32f4c662ab5d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:33 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:34:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:34:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:34:48 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:34:49 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:34:49 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:34:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:34:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31bbf0eb561b1650f22e928cbeccb17872671effa64cad96c568923c773c5e1`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7602e07641dac1311b8a2427efdb849b9749894a1a9ed64979931ed3d6f03bdc`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925b08e9954cc34ec2861c0b6ea5ade09ae1a9361db08e6c22d2c5eba5010b65`  
		Last Modified: Tue, 04 Jul 2023 06:36:23 GMT  
		Size: 115.6 MB (115646236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.9.0-enterprise`

```console
$ docker pull neo4j@sha256:6b96a248881100cc1933ed1e2f876ca17ac8138028950815824834afab757599
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.9.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ea1c4453a2053b97b8cb06ad56df3c30d9180661156fed9e14bcea4bbc2418ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.7 MB (617745671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e5444ff1b29cf9fefef7604273556c2d43cb3354fbbff37cd7f0abc235e60f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:21:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=978819870e976f903ecfb68a8e22ee5ea498779ee14a0c4d9f0f98fc29230ccb NEO4J_TARBALL=neo4j-enterprise-5.9.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:21:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:21:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:21:01 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:21:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:21:19 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:21:19 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:21:19 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:21:19 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:21:20 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:21:20 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18d4eb232eb5306440a582c9f2d9610be6c51d5518cd4d1c3472e1cc0de40c`  
		Last Modified: Tue, 04 Jul 2023 17:22:43 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947e093535bfa8b8393da45080bde93dc7cb2ffa768b256e5bd081bf7436a20`  
		Last Modified: Tue, 04 Jul 2023 17:22:43 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3943ee1048805605e62569fb57f45ee82a4907e06b48e47b6066e7f02c46449`  
		Last Modified: Tue, 04 Jul 2023 17:22:59 GMT  
		Size: 393.7 MB (393734749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.9.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:34ccc1bd75af18944b35db27f14a3747b099d89c062ebbae6d1ce13b4c3afd1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **615.1 MB (615092882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a0584d04469afc9b6f9b5dabf6d8c470fa180ae3aeb3b7a28fd24a8ae6e59e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=978819870e976f903ecfb68a8e22ee5ea498779ee14a0c4d9f0f98fc29230ccb NEO4J_TARBALL=neo4j-enterprise-5.9.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:53 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:54 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:35:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:35:13 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:35:13 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:35:13 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:35:14 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:35:14 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:35:14 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd0804164ff5a7a8bac70caaa09e39349c9e0dbb8baef6d0ff03058ca910cac`  
		Last Modified: Tue, 04 Jul 2023 06:36:48 GMT  
		Size: 3.9 KB (3892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a8710006fb7822fddd6ed807ef02ffd3ec563cea959c37a3bf53fca4f7d956`  
		Last Modified: Tue, 04 Jul 2023 06:36:49 GMT  
		Size: 9.4 KB (9370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38a745a710edaf1eadcb2d76e64bd6030fb941963f87a919d7e899aaee490fa`  
		Last Modified: Tue, 04 Jul 2023 06:37:02 GMT  
		Size: 393.6 MB (393628976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:93684114e9961735c1312802d88b6295a75b425a2f5826cb8248529b8f06921f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:56ceb318b79315af073cad11c39446c99530c1b051e7006e18a4ca805383cc52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339764620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6225dd46452249271ff53463cd4c962b7f5645214423fec46a4162295a8bf435`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:20:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:20:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:20:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:20:44 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:20:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:20:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:20:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:20:57 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:20:57 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afa9b3f536783089b8230b0cd2bc0eb9727b192b071a19f0fbe7c91dcf940bb`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacc8baa2aac9c647538ceb39c1e59c611d6e43b9215dfcc30fcbbe64cc6eb0`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 9.4 KB (9368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6c0fb808423cc74fd89f637d31c471ef2893be64d3c47503ee0ad8030c997f`  
		Last Modified: Tue, 04 Jul 2023 17:22:23 GMT  
		Size: 115.8 MB (115753701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:ab9c060c7ff61a54b35a7b38fc09f4cb143f210c2c7711c04d19802b0b97f10f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337110137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2aa94390a4d91363d5896f5f9c83921b57d038fa1fefc849bf32f4c662ab5d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:33 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:34:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:34:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:34:48 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:34:49 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:34:49 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:34:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:34:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31bbf0eb561b1650f22e928cbeccb17872671effa64cad96c568923c773c5e1`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7602e07641dac1311b8a2427efdb849b9749894a1a9ed64979931ed3d6f03bdc`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925b08e9954cc34ec2861c0b6ea5ade09ae1a9361db08e6c22d2c5eba5010b65`  
		Last Modified: Tue, 04 Jul 2023 06:36:23 GMT  
		Size: 115.6 MB (115646236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:6b96a248881100cc1933ed1e2f876ca17ac8138028950815824834afab757599
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ea1c4453a2053b97b8cb06ad56df3c30d9180661156fed9e14bcea4bbc2418ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.7 MB (617745671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e5444ff1b29cf9fefef7604273556c2d43cb3354fbbff37cd7f0abc235e60f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:21:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=978819870e976f903ecfb68a8e22ee5ea498779ee14a0c4d9f0f98fc29230ccb NEO4J_TARBALL=neo4j-enterprise-5.9.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:21:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:21:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:21:01 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:21:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:21:19 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:21:19 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:21:19 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:21:19 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:21:20 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:21:20 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18d4eb232eb5306440a582c9f2d9610be6c51d5518cd4d1c3472e1cc0de40c`  
		Last Modified: Tue, 04 Jul 2023 17:22:43 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947e093535bfa8b8393da45080bde93dc7cb2ffa768b256e5bd081bf7436a20`  
		Last Modified: Tue, 04 Jul 2023 17:22:43 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3943ee1048805605e62569fb57f45ee82a4907e06b48e47b6066e7f02c46449`  
		Last Modified: Tue, 04 Jul 2023 17:22:59 GMT  
		Size: 393.7 MB (393734749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:34ccc1bd75af18944b35db27f14a3747b099d89c062ebbae6d1ce13b4c3afd1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **615.1 MB (615092882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a0584d04469afc9b6f9b5dabf6d8c470fa180ae3aeb3b7a28fd24a8ae6e59e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=978819870e976f903ecfb68a8e22ee5ea498779ee14a0c4d9f0f98fc29230ccb NEO4J_TARBALL=neo4j-enterprise-5.9.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:53 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:54 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:35:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:35:13 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:35:13 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:35:13 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:35:14 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:35:14 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:35:14 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd0804164ff5a7a8bac70caaa09e39349c9e0dbb8baef6d0ff03058ca910cac`  
		Last Modified: Tue, 04 Jul 2023 06:36:48 GMT  
		Size: 3.9 KB (3892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a8710006fb7822fddd6ed807ef02ffd3ec563cea959c37a3bf53fca4f7d956`  
		Last Modified: Tue, 04 Jul 2023 06:36:49 GMT  
		Size: 9.4 KB (9370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38a745a710edaf1eadcb2d76e64bd6030fb941963f87a919d7e899aaee490fa`  
		Last Modified: Tue, 04 Jul 2023 06:37:02 GMT  
		Size: 393.6 MB (393628976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:93684114e9961735c1312802d88b6295a75b425a2f5826cb8248529b8f06921f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:56ceb318b79315af073cad11c39446c99530c1b051e7006e18a4ca805383cc52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339764620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6225dd46452249271ff53463cd4c962b7f5645214423fec46a4162295a8bf435`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 04:06:23 GMT
COPY dir:bd419ef2141504aa2f648c196bb8bfe0688018838c9b92d958b5908207ce1f25 in /opt/java/openjdk 
# Tue, 04 Jul 2023 17:20:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 17:20:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 17:20:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 17:20:44 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 17:20:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:20:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:20:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 17:20:57 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 17:20:57 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 17:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 17:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22f472fa461196b4d0768628e3eee647b25cc27072e8bad3c89810bdd847134`  
		Last Modified: Tue, 04 Jul 2023 04:15:28 GMT  
		Size: 192.6 MB (192580306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afa9b3f536783089b8230b0cd2bc0eb9727b192b071a19f0fbe7c91dcf940bb`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacc8baa2aac9c647538ceb39c1e59c611d6e43b9215dfcc30fcbbe64cc6eb0`  
		Last Modified: Tue, 04 Jul 2023 17:22:18 GMT  
		Size: 9.4 KB (9368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6c0fb808423cc74fd89f637d31c471ef2893be64d3c47503ee0ad8030c997f`  
		Last Modified: Tue, 04 Jul 2023 17:22:23 GMT  
		Size: 115.8 MB (115753701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:ab9c060c7ff61a54b35a7b38fc09f4cb143f210c2c7711c04d19802b0b97f10f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337110137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2aa94390a4d91363d5896f5f9c83921b57d038fa1fefc849bf32f4c662ab5d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 06:34:28 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Tue, 04 Jul 2023 06:34:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5c8774afac24e8a43d1de94d7b200ed6ad27f51b6ab7802bc325f5d27992930a NEO4J_TARBALL=neo4j-community-5.9.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 04 Jul 2023 06:34:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
# Tue, 04 Jul 2023 06:34:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 04 Jul 2023 06:34:33 GMT
COPY multi:5d29fd3ffa43989bd2f4a4674bb74cea0fc3d966076b29cc72e8b59442142704 in /startup/ 
# Tue, 04 Jul 2023 06:34:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.9.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:34:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:34:48 GMT
WORKDIR /var/lib/neo4j
# Tue, 04 Jul 2023 06:34:49 GMT
VOLUME [/data /logs]
# Tue, 04 Jul 2023 06:34:49 GMT
EXPOSE 7473 7474 7687
# Tue, 04 Jul 2023 06:34:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:34:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275827ff61a5cc842494b7c486dc8fd020f878ff693af5f57969cf5f7481a0d0`  
		Last Modified: Tue, 04 Jul 2023 06:36:29 GMT  
		Size: 191.4 MB (191387687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31bbf0eb561b1650f22e928cbeccb17872671effa64cad96c568923c773c5e1`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7602e07641dac1311b8a2427efdb849b9749894a1a9ed64979931ed3d6f03bdc`  
		Last Modified: Tue, 04 Jul 2023 06:36:18 GMT  
		Size: 9.4 KB (9371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925b08e9954cc34ec2861c0b6ea5ade09ae1a9361db08e6c22d2c5eba5010b65`  
		Last Modified: Tue, 04 Jul 2023 06:36:23 GMT  
		Size: 115.6 MB (115646236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
