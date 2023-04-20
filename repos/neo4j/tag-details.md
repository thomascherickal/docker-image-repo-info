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
$ docker pull neo4j@sha256:c2dfb91ebe161dd6b1674ec887f54243574e07f373480bd330980167a7bdbf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:233e40a451103a4eea525b9f05f1cf7e99c218498e29632f284d8556e4af3912
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.6 MB (349567274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3504dbdfa74967bf5945fdc1b24833d24b466fab830c949e6efc1ea59336ad3e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:14:00 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:28:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 08:28:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 08:28:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 08:28:13 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 08:28:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:28:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:28:24 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 08:28:24 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 08:28:24 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 08:28:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 08:28:24 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4791db44f1181a51939f7b21de0fda8d67e0a03b6a5393ac49f8d64eadc56`  
		Last Modified: Wed, 12 Apr 2023 08:23:18 GMT  
		Size: 198.5 MB (198475991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5b333302b9ab5809f19218cd380df91f9a27f10b5d28432c248accad3b2e0d`  
		Last Modified: Wed, 12 Apr 2023 08:29:44 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc619c949cadf2a283ec47987f96965d00f0b355e8dd1e3b91e3fd30b582577`  
		Last Modified: Wed, 12 Apr 2023 08:29:44 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b306b912272817594d9ba4e4515ff2c94db58be29fb05f62248de4ef615b1db0`  
		Last Modified: Wed, 12 Apr 2023 08:29:49 GMT  
		Size: 119.7 MB (119660626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5cd4a30938ea03d4ccb7da402113e996faf548045ad441344c8c598d2eb5fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.8 MB (344836993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865938353751632763ef13e1ee47f440ee78564b9400c8a09e8f9d5246ff3bf6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:21:10 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 04:19:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 04:19:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 04:19:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 04:19:26 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 04:19:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:19:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 04:19:36 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 04:19:37 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 04:19:37 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 04:19:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 04:19:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2a925b22c34d676c0f7dfea6c5e40dae89a2cd334554f1387adb3b0d65cee9`  
		Last Modified: Wed, 12 Apr 2023 01:29:42 GMT  
		Size: 195.2 MB (195242534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f4f0923ceb9a6b28985a53c91321754176486b20e26dbc7de37a4ab5b0b5d6`  
		Last Modified: Wed, 12 Apr 2023 04:20:59 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d9a312c1147b08b3200688361c11243b3c745f4ac478a03bb5ba66dee4bb16`  
		Last Modified: Wed, 12 Apr 2023 04:20:59 GMT  
		Size: 8.6 KB (8564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4022f1ec6edafb91be2d6d1642fb2a29af80e257add97f68193884477bdec250`  
		Last Modified: Wed, 12 Apr 2023 04:21:04 GMT  
		Size: 119.5 MB (119518182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:c2dfb91ebe161dd6b1674ec887f54243574e07f373480bd330980167a7bdbf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:233e40a451103a4eea525b9f05f1cf7e99c218498e29632f284d8556e4af3912
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.6 MB (349567274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3504dbdfa74967bf5945fdc1b24833d24b466fab830c949e6efc1ea59336ad3e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:14:00 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:28:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 08:28:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 08:28:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 08:28:13 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 08:28:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:28:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:28:24 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 08:28:24 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 08:28:24 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 08:28:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 08:28:24 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4791db44f1181a51939f7b21de0fda8d67e0a03b6a5393ac49f8d64eadc56`  
		Last Modified: Wed, 12 Apr 2023 08:23:18 GMT  
		Size: 198.5 MB (198475991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5b333302b9ab5809f19218cd380df91f9a27f10b5d28432c248accad3b2e0d`  
		Last Modified: Wed, 12 Apr 2023 08:29:44 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc619c949cadf2a283ec47987f96965d00f0b355e8dd1e3b91e3fd30b582577`  
		Last Modified: Wed, 12 Apr 2023 08:29:44 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b306b912272817594d9ba4e4515ff2c94db58be29fb05f62248de4ef615b1db0`  
		Last Modified: Wed, 12 Apr 2023 08:29:49 GMT  
		Size: 119.7 MB (119660626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5cd4a30938ea03d4ccb7da402113e996faf548045ad441344c8c598d2eb5fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.8 MB (344836993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865938353751632763ef13e1ee47f440ee78564b9400c8a09e8f9d5246ff3bf6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:21:10 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 04:19:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 04:19:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 04:19:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 04:19:26 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 04:19:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:19:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 04:19:36 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 04:19:37 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 04:19:37 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 04:19:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 04:19:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2a925b22c34d676c0f7dfea6c5e40dae89a2cd334554f1387adb3b0d65cee9`  
		Last Modified: Wed, 12 Apr 2023 01:29:42 GMT  
		Size: 195.2 MB (195242534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f4f0923ceb9a6b28985a53c91321754176486b20e26dbc7de37a4ab5b0b5d6`  
		Last Modified: Wed, 12 Apr 2023 04:20:59 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d9a312c1147b08b3200688361c11243b3c745f4ac478a03bb5ba66dee4bb16`  
		Last Modified: Wed, 12 Apr 2023 04:20:59 GMT  
		Size: 8.6 KB (8564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4022f1ec6edafb91be2d6d1642fb2a29af80e257add97f68193884477bdec250`  
		Last Modified: Wed, 12 Apr 2023 04:21:04 GMT  
		Size: 119.5 MB (119518182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:80123d1fce7761a99fa0109f6876c454c900209d33a7fb9373fec1fe0207a6ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:8b22aba3f4da2780f2b8b4775060b2cabe54474bb04c9fe0642dfd762316c0fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.3 MB (446334882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d212280b19a45fbb4d43dc735aa85d9d6c00887a343df1e380adc69a72f751d7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:14:00 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:28:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e9ecf2706abff535c4ac9e902ca36257ab23af96be3386ea54f0ec17dcb7cf8e NEO4J_TARBALL=neo4j-enterprise-4.4.19-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 08:28:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 08:28:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 08:28:29 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 08:28:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:28:42 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:28:43 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 08:28:43 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 08:28:43 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 08:28:43 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 08:28:43 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4791db44f1181a51939f7b21de0fda8d67e0a03b6a5393ac49f8d64eadc56`  
		Last Modified: Wed, 12 Apr 2023 08:23:18 GMT  
		Size: 198.5 MB (198475991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a1c32c48cc8b1243a4498a5c9f69ed7d8c7851d0beb170d8eb53724bf7c768`  
		Last Modified: Wed, 12 Apr 2023 08:30:01 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e988b2bb0eefe1fefdbb27f9df55ca19dafbd364a06a1fc4d2cabb69b6984b9a`  
		Last Modified: Wed, 12 Apr 2023 08:30:01 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8975ceb99e32eb8d44924a3d020d3a89c1cc42e17ff9f7c499c05d5e05709ed1`  
		Last Modified: Wed, 12 Apr 2023 08:30:10 GMT  
		Size: 216.4 MB (216428239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4f93208dbcfab14e87ec86def2918a858bc1862c1b56200188e258422f79d38c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.6 MB (441604971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e52bcf7f636a84cd72afb3311c7b6dac17c474687142adbfe0f165e22c0a2ed`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:21:10 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 04:19:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e9ecf2706abff535c4ac9e902ca36257ab23af96be3386ea54f0ec17dcb7cf8e NEO4J_TARBALL=neo4j-enterprise-4.4.19-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 04:19:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 04:19:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 04:19:40 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 04:19:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:19:59 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 04:19:59 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 04:19:59 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 04:19:59 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 04:19:59 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 04:19:59 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2a925b22c34d676c0f7dfea6c5e40dae89a2cd334554f1387adb3b0d65cee9`  
		Last Modified: Wed, 12 Apr 2023 01:29:42 GMT  
		Size: 195.2 MB (195242534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bb05aa0bc57ddafcd0544e72a5249b71194450c0ed5c0313d53a5265289a5b`  
		Last Modified: Wed, 12 Apr 2023 04:21:15 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0eaec0edabda472a78212330a9a1048a704a6f7ccf77cfdf70ddf1a3b5382d3`  
		Last Modified: Wed, 12 Apr 2023 04:21:15 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d9cb15aaf269aad791dbd64d8c69f932d284df8abf61e52f2f61167845275`  
		Last Modified: Wed, 12 Apr 2023 04:21:24 GMT  
		Size: 216.3 MB (216286159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.19`

```console
$ docker pull neo4j@sha256:c2dfb91ebe161dd6b1674ec887f54243574e07f373480bd330980167a7bdbf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.19` - linux; amd64

```console
$ docker pull neo4j@sha256:233e40a451103a4eea525b9f05f1cf7e99c218498e29632f284d8556e4af3912
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.6 MB (349567274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3504dbdfa74967bf5945fdc1b24833d24b466fab830c949e6efc1ea59336ad3e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:14:00 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:28:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 08:28:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 08:28:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 08:28:13 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 08:28:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:28:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:28:24 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 08:28:24 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 08:28:24 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 08:28:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 08:28:24 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4791db44f1181a51939f7b21de0fda8d67e0a03b6a5393ac49f8d64eadc56`  
		Last Modified: Wed, 12 Apr 2023 08:23:18 GMT  
		Size: 198.5 MB (198475991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5b333302b9ab5809f19218cd380df91f9a27f10b5d28432c248accad3b2e0d`  
		Last Modified: Wed, 12 Apr 2023 08:29:44 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc619c949cadf2a283ec47987f96965d00f0b355e8dd1e3b91e3fd30b582577`  
		Last Modified: Wed, 12 Apr 2023 08:29:44 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b306b912272817594d9ba4e4515ff2c94db58be29fb05f62248de4ef615b1db0`  
		Last Modified: Wed, 12 Apr 2023 08:29:49 GMT  
		Size: 119.7 MB (119660626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.19` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5cd4a30938ea03d4ccb7da402113e996faf548045ad441344c8c598d2eb5fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.8 MB (344836993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865938353751632763ef13e1ee47f440ee78564b9400c8a09e8f9d5246ff3bf6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:21:10 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 04:19:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 04:19:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 04:19:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 04:19:26 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 04:19:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:19:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 04:19:36 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 04:19:37 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 04:19:37 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 04:19:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 04:19:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2a925b22c34d676c0f7dfea6c5e40dae89a2cd334554f1387adb3b0d65cee9`  
		Last Modified: Wed, 12 Apr 2023 01:29:42 GMT  
		Size: 195.2 MB (195242534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f4f0923ceb9a6b28985a53c91321754176486b20e26dbc7de37a4ab5b0b5d6`  
		Last Modified: Wed, 12 Apr 2023 04:20:59 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d9a312c1147b08b3200688361c11243b3c745f4ac478a03bb5ba66dee4bb16`  
		Last Modified: Wed, 12 Apr 2023 04:20:59 GMT  
		Size: 8.6 KB (8564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4022f1ec6edafb91be2d6d1642fb2a29af80e257add97f68193884477bdec250`  
		Last Modified: Wed, 12 Apr 2023 04:21:04 GMT  
		Size: 119.5 MB (119518182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.19-community`

```console
$ docker pull neo4j@sha256:c2dfb91ebe161dd6b1674ec887f54243574e07f373480bd330980167a7bdbf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.19-community` - linux; amd64

```console
$ docker pull neo4j@sha256:233e40a451103a4eea525b9f05f1cf7e99c218498e29632f284d8556e4af3912
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.6 MB (349567274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3504dbdfa74967bf5945fdc1b24833d24b466fab830c949e6efc1ea59336ad3e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:14:00 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:28:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 08:28:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 08:28:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 08:28:13 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 08:28:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:28:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:28:24 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 08:28:24 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 08:28:24 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 08:28:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 08:28:24 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4791db44f1181a51939f7b21de0fda8d67e0a03b6a5393ac49f8d64eadc56`  
		Last Modified: Wed, 12 Apr 2023 08:23:18 GMT  
		Size: 198.5 MB (198475991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5b333302b9ab5809f19218cd380df91f9a27f10b5d28432c248accad3b2e0d`  
		Last Modified: Wed, 12 Apr 2023 08:29:44 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc619c949cadf2a283ec47987f96965d00f0b355e8dd1e3b91e3fd30b582577`  
		Last Modified: Wed, 12 Apr 2023 08:29:44 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b306b912272817594d9ba4e4515ff2c94db58be29fb05f62248de4ef615b1db0`  
		Last Modified: Wed, 12 Apr 2023 08:29:49 GMT  
		Size: 119.7 MB (119660626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.19-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5cd4a30938ea03d4ccb7da402113e996faf548045ad441344c8c598d2eb5fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.8 MB (344836993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865938353751632763ef13e1ee47f440ee78564b9400c8a09e8f9d5246ff3bf6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:21:10 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 04:19:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e101ff8ad46b1244223fefb2508e4d83c40a717028e004aba66b9cc70945cecb NEO4J_TARBALL=neo4j-community-4.4.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 04:19:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 04:19:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 04:19:26 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 04:19:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:19:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 04:19:36 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 04:19:37 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 04:19:37 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 04:19:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 04:19:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2a925b22c34d676c0f7dfea6c5e40dae89a2cd334554f1387adb3b0d65cee9`  
		Last Modified: Wed, 12 Apr 2023 01:29:42 GMT  
		Size: 195.2 MB (195242534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f4f0923ceb9a6b28985a53c91321754176486b20e26dbc7de37a4ab5b0b5d6`  
		Last Modified: Wed, 12 Apr 2023 04:20:59 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d9a312c1147b08b3200688361c11243b3c745f4ac478a03bb5ba66dee4bb16`  
		Last Modified: Wed, 12 Apr 2023 04:20:59 GMT  
		Size: 8.6 KB (8564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4022f1ec6edafb91be2d6d1642fb2a29af80e257add97f68193884477bdec250`  
		Last Modified: Wed, 12 Apr 2023 04:21:04 GMT  
		Size: 119.5 MB (119518182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.19-enterprise`

```console
$ docker pull neo4j@sha256:80123d1fce7761a99fa0109f6876c454c900209d33a7fb9373fec1fe0207a6ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.19-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:8b22aba3f4da2780f2b8b4775060b2cabe54474bb04c9fe0642dfd762316c0fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.3 MB (446334882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d212280b19a45fbb4d43dc735aa85d9d6c00887a343df1e380adc69a72f751d7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:14:00 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:28:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e9ecf2706abff535c4ac9e902ca36257ab23af96be3386ea54f0ec17dcb7cf8e NEO4J_TARBALL=neo4j-enterprise-4.4.19-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 08:28:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 08:28:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 08:28:29 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 08:28:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:28:42 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:28:43 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 08:28:43 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 08:28:43 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 08:28:43 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 08:28:43 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4791db44f1181a51939f7b21de0fda8d67e0a03b6a5393ac49f8d64eadc56`  
		Last Modified: Wed, 12 Apr 2023 08:23:18 GMT  
		Size: 198.5 MB (198475991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a1c32c48cc8b1243a4498a5c9f69ed7d8c7851d0beb170d8eb53724bf7c768`  
		Last Modified: Wed, 12 Apr 2023 08:30:01 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e988b2bb0eefe1fefdbb27f9df55ca19dafbd364a06a1fc4d2cabb69b6984b9a`  
		Last Modified: Wed, 12 Apr 2023 08:30:01 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8975ceb99e32eb8d44924a3d020d3a89c1cc42e17ff9f7c499c05d5e05709ed1`  
		Last Modified: Wed, 12 Apr 2023 08:30:10 GMT  
		Size: 216.4 MB (216428239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.19-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4f93208dbcfab14e87ec86def2918a858bc1862c1b56200188e258422f79d38c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.6 MB (441604971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e52bcf7f636a84cd72afb3311c7b6dac17c474687142adbfe0f165e22c0a2ed`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:21:10 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 04:19:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e9ecf2706abff535c4ac9e902ca36257ab23af96be3386ea54f0ec17dcb7cf8e NEO4J_TARBALL=neo4j-enterprise-4.4.19-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 12 Apr 2023 04:19:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
# Wed, 12 Apr 2023 04:19:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 12 Apr 2023 04:19:40 GMT
COPY multi:aaaef3312b424e9587435ac8f800bbbd3d3459429e38edf4429492cb6a753a4b in /startup/ 
# Wed, 12 Apr 2023 04:19:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:19:59 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 04:19:59 GMT
WORKDIR /var/lib/neo4j
# Wed, 12 Apr 2023 04:19:59 GMT
VOLUME [/data /logs]
# Wed, 12 Apr 2023 04:19:59 GMT
EXPOSE 7473 7474 7687
# Wed, 12 Apr 2023 04:19:59 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 04:19:59 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2a925b22c34d676c0f7dfea6c5e40dae89a2cd334554f1387adb3b0d65cee9`  
		Last Modified: Wed, 12 Apr 2023 01:29:42 GMT  
		Size: 195.2 MB (195242534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bb05aa0bc57ddafcd0544e72a5249b71194450c0ed5c0313d53a5265289a5b`  
		Last Modified: Wed, 12 Apr 2023 04:21:15 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0eaec0edabda472a78212330a9a1048a704a6f7ccf77cfdf70ddf1a3b5382d3`  
		Last Modified: Wed, 12 Apr 2023 04:21:15 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d9cb15aaf269aad791dbd64d8c69f932d284df8abf61e52f2f61167845275`  
		Last Modified: Wed, 12 Apr 2023 04:21:24 GMT  
		Size: 216.3 MB (216286159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:b62813c502a696707b4f890b33e236d1f8c41df4e4335858c8cf21d3d7d6caab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:3fc78efa9bb96b507334dc70d10cce85f6bf81b679cf94b514ca9495969e3588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339542656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbff370c391789b65d526822bf5da5c3ca91ecf3f74d54eedf570afe6cd34f85`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:05 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:18 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977d0170423a85c4eb0e4bc45a4fba37797676f8b8d77d69c1f078a94c74a7a3`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe92c924f0dee66d71f30d6237be37518a2a75ef2cf80581fa47648ec4e1de5`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf4747a6e7a3ecc8826836e973d00590e58f301cbc96992d285c2b20e5e711e`  
		Last Modified: Thu, 20 Apr 2023 19:39:17 GMT  
		Size: 115.7 MB (115673535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4fa2dbc6e2a3afc653bdac75577919ed79b051ee9570d57c4ce3ad086297e2e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336865467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47bdd53f565cf5edf4224dd2d4ebb78943d9acec647afa7cedd748248e3c6c2`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:39:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:39:41 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:39:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:39:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:39:55 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:39:55 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:39:55 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:39:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:39:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e945c1ebf0badf10ab03f2eff8dbee4ad5847f79bfcf9ac476fd6b4f08f64bb9`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e653fe60014f6ae8c9352c39801c8e22fb52250d0917b477748fc27943cb242`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52481b4cf4323cb463feb079e8b265907f0fba629dde9d369e5d18f0ef4088`  
		Last Modified: Thu, 20 Apr 2023 19:40:41 GMT  
		Size: 115.5 MB (115528544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:b62813c502a696707b4f890b33e236d1f8c41df4e4335858c8cf21d3d7d6caab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:3fc78efa9bb96b507334dc70d10cce85f6bf81b679cf94b514ca9495969e3588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339542656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbff370c391789b65d526822bf5da5c3ca91ecf3f74d54eedf570afe6cd34f85`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:05 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:18 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977d0170423a85c4eb0e4bc45a4fba37797676f8b8d77d69c1f078a94c74a7a3`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe92c924f0dee66d71f30d6237be37518a2a75ef2cf80581fa47648ec4e1de5`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf4747a6e7a3ecc8826836e973d00590e58f301cbc96992d285c2b20e5e711e`  
		Last Modified: Thu, 20 Apr 2023 19:39:17 GMT  
		Size: 115.7 MB (115673535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4fa2dbc6e2a3afc653bdac75577919ed79b051ee9570d57c4ce3ad086297e2e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336865467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47bdd53f565cf5edf4224dd2d4ebb78943d9acec647afa7cedd748248e3c6c2`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:39:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:39:41 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:39:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:39:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:39:55 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:39:55 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:39:55 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:39:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:39:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e945c1ebf0badf10ab03f2eff8dbee4ad5847f79bfcf9ac476fd6b4f08f64bb9`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e653fe60014f6ae8c9352c39801c8e22fb52250d0917b477748fc27943cb242`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52481b4cf4323cb463feb079e8b265907f0fba629dde9d369e5d18f0ef4088`  
		Last Modified: Thu, 20 Apr 2023 19:40:41 GMT  
		Size: 115.5 MB (115528544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:6fa3dd5902b8143c375bbd85aed61563c147ae4849601c92e5074d85a677eec1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ccf9321a790fa0865a4a2005716734ab72aa65070cf7dd9c99c4b5e031374678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **604.0 MB (604008274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac749bb430d0332d8eb75e2d0c9d308530ae152788bb5b63cb4bb5958b75601`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:24 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:25 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:53 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:53 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:53 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a586f824faf837de491bb42598a1553dac740a520a98b56af256955c62d51706`  
		Last Modified: Thu, 20 Apr 2023 19:39:37 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471f065013b8d9986b122da7ee9816ba1f3325f9d1da9393b15f932eca4964fa`  
		Last Modified: Thu, 20 Apr 2023 19:39:37 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9889380e5de072b80f86b53c54a51993ec73e70a79bd173c1787f1f6d45a28b8`  
		Last Modified: Thu, 20 Apr 2023 19:39:52 GMT  
		Size: 380.1 MB (380139153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:badf2a5dffa3e3da5c416234227a79a81594dfb5e4b8e2e9e83311f39d7dfe3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.3 MB (601333285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcfb868dfdf7858e5de016c20b4c12feaf35bfab8e9febd44a9798930d042bf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:40:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:40:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:40:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:40:19 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:40:19 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:40:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:40:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:40:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:40:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68a5571919a3ffa681606c8e457424e9c6ac46b61c8576461462d3a45183fc`  
		Last Modified: Thu, 20 Apr 2023 19:41:00 GMT  
		Size: 3.9 KB (3895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2b43bfc59c1e32ca976434bfcd332dc9b0fcd701cc2f471cc25763b9acf082`  
		Last Modified: Thu, 20 Apr 2023 19:41:00 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b0d39b9df8fd2e54bcd71b738744dde00b25f28d21d960247be2989b5d35e0`  
		Last Modified: Thu, 20 Apr 2023 19:41:13 GMT  
		Size: 380.0 MB (379996362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7`

```console
$ docker pull neo4j@sha256:b62813c502a696707b4f890b33e236d1f8c41df4e4335858c8cf21d3d7d6caab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7` - linux; amd64

```console
$ docker pull neo4j@sha256:3fc78efa9bb96b507334dc70d10cce85f6bf81b679cf94b514ca9495969e3588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339542656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbff370c391789b65d526822bf5da5c3ca91ecf3f74d54eedf570afe6cd34f85`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:05 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:18 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977d0170423a85c4eb0e4bc45a4fba37797676f8b8d77d69c1f078a94c74a7a3`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe92c924f0dee66d71f30d6237be37518a2a75ef2cf80581fa47648ec4e1de5`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf4747a6e7a3ecc8826836e973d00590e58f301cbc96992d285c2b20e5e711e`  
		Last Modified: Thu, 20 Apr 2023 19:39:17 GMT  
		Size: 115.7 MB (115673535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4fa2dbc6e2a3afc653bdac75577919ed79b051ee9570d57c4ce3ad086297e2e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336865467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47bdd53f565cf5edf4224dd2d4ebb78943d9acec647afa7cedd748248e3c6c2`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:39:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:39:41 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:39:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:39:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:39:55 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:39:55 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:39:55 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:39:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:39:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e945c1ebf0badf10ab03f2eff8dbee4ad5847f79bfcf9ac476fd6b4f08f64bb9`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e653fe60014f6ae8c9352c39801c8e22fb52250d0917b477748fc27943cb242`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52481b4cf4323cb463feb079e8b265907f0fba629dde9d369e5d18f0ef4088`  
		Last Modified: Thu, 20 Apr 2023 19:40:41 GMT  
		Size: 115.5 MB (115528544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7-community`

```console
$ docker pull neo4j@sha256:b62813c502a696707b4f890b33e236d1f8c41df4e4335858c8cf21d3d7d6caab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7-community` - linux; amd64

```console
$ docker pull neo4j@sha256:3fc78efa9bb96b507334dc70d10cce85f6bf81b679cf94b514ca9495969e3588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339542656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbff370c391789b65d526822bf5da5c3ca91ecf3f74d54eedf570afe6cd34f85`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:05 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:18 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977d0170423a85c4eb0e4bc45a4fba37797676f8b8d77d69c1f078a94c74a7a3`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe92c924f0dee66d71f30d6237be37518a2a75ef2cf80581fa47648ec4e1de5`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf4747a6e7a3ecc8826836e973d00590e58f301cbc96992d285c2b20e5e711e`  
		Last Modified: Thu, 20 Apr 2023 19:39:17 GMT  
		Size: 115.7 MB (115673535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4fa2dbc6e2a3afc653bdac75577919ed79b051ee9570d57c4ce3ad086297e2e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336865467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47bdd53f565cf5edf4224dd2d4ebb78943d9acec647afa7cedd748248e3c6c2`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:39:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:39:41 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:39:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:39:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:39:55 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:39:55 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:39:55 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:39:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:39:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e945c1ebf0badf10ab03f2eff8dbee4ad5847f79bfcf9ac476fd6b4f08f64bb9`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e653fe60014f6ae8c9352c39801c8e22fb52250d0917b477748fc27943cb242`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52481b4cf4323cb463feb079e8b265907f0fba629dde9d369e5d18f0ef4088`  
		Last Modified: Thu, 20 Apr 2023 19:40:41 GMT  
		Size: 115.5 MB (115528544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7-enterprise`

```console
$ docker pull neo4j@sha256:6fa3dd5902b8143c375bbd85aed61563c147ae4849601c92e5074d85a677eec1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ccf9321a790fa0865a4a2005716734ab72aa65070cf7dd9c99c4b5e031374678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **604.0 MB (604008274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac749bb430d0332d8eb75e2d0c9d308530ae152788bb5b63cb4bb5958b75601`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:24 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:25 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:53 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:53 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:53 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a586f824faf837de491bb42598a1553dac740a520a98b56af256955c62d51706`  
		Last Modified: Thu, 20 Apr 2023 19:39:37 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471f065013b8d9986b122da7ee9816ba1f3325f9d1da9393b15f932eca4964fa`  
		Last Modified: Thu, 20 Apr 2023 19:39:37 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9889380e5de072b80f86b53c54a51993ec73e70a79bd173c1787f1f6d45a28b8`  
		Last Modified: Thu, 20 Apr 2023 19:39:52 GMT  
		Size: 380.1 MB (380139153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:badf2a5dffa3e3da5c416234227a79a81594dfb5e4b8e2e9e83311f39d7dfe3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.3 MB (601333285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcfb868dfdf7858e5de016c20b4c12feaf35bfab8e9febd44a9798930d042bf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:40:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:40:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:40:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:40:19 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:40:19 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:40:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:40:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:40:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:40:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68a5571919a3ffa681606c8e457424e9c6ac46b61c8576461462d3a45183fc`  
		Last Modified: Thu, 20 Apr 2023 19:41:00 GMT  
		Size: 3.9 KB (3895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2b43bfc59c1e32ca976434bfcd332dc9b0fcd701cc2f471cc25763b9acf082`  
		Last Modified: Thu, 20 Apr 2023 19:41:00 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b0d39b9df8fd2e54bcd71b738744dde00b25f28d21d960247be2989b5d35e0`  
		Last Modified: Thu, 20 Apr 2023 19:41:13 GMT  
		Size: 380.0 MB (379996362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7.0`

```console
$ docker pull neo4j@sha256:b62813c502a696707b4f890b33e236d1f8c41df4e4335858c8cf21d3d7d6caab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7.0` - linux; amd64

```console
$ docker pull neo4j@sha256:3fc78efa9bb96b507334dc70d10cce85f6bf81b679cf94b514ca9495969e3588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339542656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbff370c391789b65d526822bf5da5c3ca91ecf3f74d54eedf570afe6cd34f85`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:05 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:18 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977d0170423a85c4eb0e4bc45a4fba37797676f8b8d77d69c1f078a94c74a7a3`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe92c924f0dee66d71f30d6237be37518a2a75ef2cf80581fa47648ec4e1de5`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf4747a6e7a3ecc8826836e973d00590e58f301cbc96992d285c2b20e5e711e`  
		Last Modified: Thu, 20 Apr 2023 19:39:17 GMT  
		Size: 115.7 MB (115673535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4fa2dbc6e2a3afc653bdac75577919ed79b051ee9570d57c4ce3ad086297e2e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336865467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47bdd53f565cf5edf4224dd2d4ebb78943d9acec647afa7cedd748248e3c6c2`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:39:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:39:41 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:39:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:39:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:39:55 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:39:55 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:39:55 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:39:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:39:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e945c1ebf0badf10ab03f2eff8dbee4ad5847f79bfcf9ac476fd6b4f08f64bb9`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e653fe60014f6ae8c9352c39801c8e22fb52250d0917b477748fc27943cb242`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52481b4cf4323cb463feb079e8b265907f0fba629dde9d369e5d18f0ef4088`  
		Last Modified: Thu, 20 Apr 2023 19:40:41 GMT  
		Size: 115.5 MB (115528544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7.0-community`

```console
$ docker pull neo4j@sha256:b62813c502a696707b4f890b33e236d1f8c41df4e4335858c8cf21d3d7d6caab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:3fc78efa9bb96b507334dc70d10cce85f6bf81b679cf94b514ca9495969e3588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339542656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbff370c391789b65d526822bf5da5c3ca91ecf3f74d54eedf570afe6cd34f85`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:05 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:18 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977d0170423a85c4eb0e4bc45a4fba37797676f8b8d77d69c1f078a94c74a7a3`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe92c924f0dee66d71f30d6237be37518a2a75ef2cf80581fa47648ec4e1de5`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf4747a6e7a3ecc8826836e973d00590e58f301cbc96992d285c2b20e5e711e`  
		Last Modified: Thu, 20 Apr 2023 19:39:17 GMT  
		Size: 115.7 MB (115673535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4fa2dbc6e2a3afc653bdac75577919ed79b051ee9570d57c4ce3ad086297e2e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336865467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47bdd53f565cf5edf4224dd2d4ebb78943d9acec647afa7cedd748248e3c6c2`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:39:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:39:41 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:39:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:39:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:39:55 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:39:55 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:39:55 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:39:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:39:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e945c1ebf0badf10ab03f2eff8dbee4ad5847f79bfcf9ac476fd6b4f08f64bb9`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e653fe60014f6ae8c9352c39801c8e22fb52250d0917b477748fc27943cb242`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52481b4cf4323cb463feb079e8b265907f0fba629dde9d369e5d18f0ef4088`  
		Last Modified: Thu, 20 Apr 2023 19:40:41 GMT  
		Size: 115.5 MB (115528544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.7.0-enterprise`

```console
$ docker pull neo4j@sha256:6fa3dd5902b8143c375bbd85aed61563c147ae4849601c92e5074d85a677eec1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.7.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ccf9321a790fa0865a4a2005716734ab72aa65070cf7dd9c99c4b5e031374678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **604.0 MB (604008274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac749bb430d0332d8eb75e2d0c9d308530ae152788bb5b63cb4bb5958b75601`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:24 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:25 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:53 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:53 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:53 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a586f824faf837de491bb42598a1553dac740a520a98b56af256955c62d51706`  
		Last Modified: Thu, 20 Apr 2023 19:39:37 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471f065013b8d9986b122da7ee9816ba1f3325f9d1da9393b15f932eca4964fa`  
		Last Modified: Thu, 20 Apr 2023 19:39:37 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9889380e5de072b80f86b53c54a51993ec73e70a79bd173c1787f1f6d45a28b8`  
		Last Modified: Thu, 20 Apr 2023 19:39:52 GMT  
		Size: 380.1 MB (380139153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.7.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:badf2a5dffa3e3da5c416234227a79a81594dfb5e4b8e2e9e83311f39d7dfe3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.3 MB (601333285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcfb868dfdf7858e5de016c20b4c12feaf35bfab8e9febd44a9798930d042bf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:40:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:40:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:40:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:40:19 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:40:19 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:40:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:40:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:40:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:40:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68a5571919a3ffa681606c8e457424e9c6ac46b61c8576461462d3a45183fc`  
		Last Modified: Thu, 20 Apr 2023 19:41:00 GMT  
		Size: 3.9 KB (3895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2b43bfc59c1e32ca976434bfcd332dc9b0fcd701cc2f471cc25763b9acf082`  
		Last Modified: Thu, 20 Apr 2023 19:41:00 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b0d39b9df8fd2e54bcd71b738744dde00b25f28d21d960247be2989b5d35e0`  
		Last Modified: Thu, 20 Apr 2023 19:41:13 GMT  
		Size: 380.0 MB (379996362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:b62813c502a696707b4f890b33e236d1f8c41df4e4335858c8cf21d3d7d6caab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:3fc78efa9bb96b507334dc70d10cce85f6bf81b679cf94b514ca9495969e3588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339542656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbff370c391789b65d526822bf5da5c3ca91ecf3f74d54eedf570afe6cd34f85`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:05 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:18 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977d0170423a85c4eb0e4bc45a4fba37797676f8b8d77d69c1f078a94c74a7a3`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe92c924f0dee66d71f30d6237be37518a2a75ef2cf80581fa47648ec4e1de5`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf4747a6e7a3ecc8826836e973d00590e58f301cbc96992d285c2b20e5e711e`  
		Last Modified: Thu, 20 Apr 2023 19:39:17 GMT  
		Size: 115.7 MB (115673535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4fa2dbc6e2a3afc653bdac75577919ed79b051ee9570d57c4ce3ad086297e2e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336865467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47bdd53f565cf5edf4224dd2d4ebb78943d9acec647afa7cedd748248e3c6c2`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:39:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:39:41 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:39:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:39:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:39:55 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:39:55 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:39:55 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:39:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:39:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e945c1ebf0badf10ab03f2eff8dbee4ad5847f79bfcf9ac476fd6b4f08f64bb9`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e653fe60014f6ae8c9352c39801c8e22fb52250d0917b477748fc27943cb242`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52481b4cf4323cb463feb079e8b265907f0fba629dde9d369e5d18f0ef4088`  
		Last Modified: Thu, 20 Apr 2023 19:40:41 GMT  
		Size: 115.5 MB (115528544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:6fa3dd5902b8143c375bbd85aed61563c147ae4849601c92e5074d85a677eec1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ccf9321a790fa0865a4a2005716734ab72aa65070cf7dd9c99c4b5e031374678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **604.0 MB (604008274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac749bb430d0332d8eb75e2d0c9d308530ae152788bb5b63cb4bb5958b75601`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:24 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:25 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:53 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:53 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:53 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a586f824faf837de491bb42598a1553dac740a520a98b56af256955c62d51706`  
		Last Modified: Thu, 20 Apr 2023 19:39:37 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471f065013b8d9986b122da7ee9816ba1f3325f9d1da9393b15f932eca4964fa`  
		Last Modified: Thu, 20 Apr 2023 19:39:37 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9889380e5de072b80f86b53c54a51993ec73e70a79bd173c1787f1f6d45a28b8`  
		Last Modified: Thu, 20 Apr 2023 19:39:52 GMT  
		Size: 380.1 MB (380139153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:badf2a5dffa3e3da5c416234227a79a81594dfb5e4b8e2e9e83311f39d7dfe3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.3 MB (601333285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcfb868dfdf7858e5de016c20b4c12feaf35bfab8e9febd44a9798930d042bf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ed2a757d3d52b0dd5d37566118e333c4a32568d8b551d47edb62222b37f9486a NEO4J_TARBALL=neo4j-enterprise-5.7.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:40:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:40:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:40:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:40:19 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:40:19 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:40:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:40:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:40:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:40:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68a5571919a3ffa681606c8e457424e9c6ac46b61c8576461462d3a45183fc`  
		Last Modified: Thu, 20 Apr 2023 19:41:00 GMT  
		Size: 3.9 KB (3895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2b43bfc59c1e32ca976434bfcd332dc9b0fcd701cc2f471cc25763b9acf082`  
		Last Modified: Thu, 20 Apr 2023 19:41:00 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b0d39b9df8fd2e54bcd71b738744dde00b25f28d21d960247be2989b5d35e0`  
		Last Modified: Thu, 20 Apr 2023 19:41:13 GMT  
		Size: 380.0 MB (379996362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:b62813c502a696707b4f890b33e236d1f8c41df4e4335858c8cf21d3d7d6caab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:3fc78efa9bb96b507334dc70d10cce85f6bf81b679cf94b514ca9495969e3588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339542656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbff370c391789b65d526822bf5da5c3ca91ecf3f74d54eedf570afe6cd34f85`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:38:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:38:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:38:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:38:05 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:38:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:38:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:38:18 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:38:19 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:38:19 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:38:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:38:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977d0170423a85c4eb0e4bc45a4fba37797676f8b8d77d69c1f078a94c74a7a3`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe92c924f0dee66d71f30d6237be37518a2a75ef2cf80581fa47648ec4e1de5`  
		Last Modified: Thu, 20 Apr 2023 19:39:12 GMT  
		Size: 8.8 KB (8771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf4747a6e7a3ecc8826836e973d00590e58f301cbc96992d285c2b20e5e711e`  
		Last Modified: Thu, 20 Apr 2023 19:39:17 GMT  
		Size: 115.7 MB (115673535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4fa2dbc6e2a3afc653bdac75577919ed79b051ee9570d57c4ce3ad086297e2e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336865467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47bdd53f565cf5edf4224dd2d4ebb78943d9acec647afa7cedd748248e3c6c2`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 20 Apr 2023 19:39:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 20 Apr 2023 19:39:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 20 Apr 2023 19:39:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 20 Apr 2023 19:39:41 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 20 Apr 2023 19:39:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 19:39:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 19:39:55 GMT
WORKDIR /var/lib/neo4j
# Thu, 20 Apr 2023 19:39:55 GMT
VOLUME [/data /logs]
# Thu, 20 Apr 2023 19:39:55 GMT
EXPOSE 7473 7474 7687
# Thu, 20 Apr 2023 19:39:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 20 Apr 2023 19:39:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e945c1ebf0badf10ab03f2eff8dbee4ad5847f79bfcf9ac476fd6b4f08f64bb9`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e653fe60014f6ae8c9352c39801c8e22fb52250d0917b477748fc27943cb242`  
		Last Modified: Thu, 20 Apr 2023 19:40:36 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52481b4cf4323cb463feb079e8b265907f0fba629dde9d369e5d18f0ef4088`  
		Last Modified: Thu, 20 Apr 2023 19:40:41 GMT  
		Size: 115.5 MB (115528544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
