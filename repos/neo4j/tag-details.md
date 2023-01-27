<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.16`](#neo4j4416)
-	[`neo4j:4.4.16-community`](#neo4j4416-community)
-	[`neo4j:4.4.16-enterprise`](#neo4j4416-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5.4`](#neo4j54)
-	[`neo4j:5.4-enterprise`](#neo4j54-enterprise)
-	[`neo4j:5.4.0`](#neo4j540)
-	[`neo4j:5.4.0-community`](#neo4j540-community)
-	[`neo4j:5.4.0-enterprise`](#neo4j540-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:0ee890b73a6f61cbcbfc10d0e38eedb207866b3d0c8209ae7fb0dac6259c2908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:1a77c6d92542a6cd8ea4a79e03db440e730fddc21605c8f1bed187410a441d74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366768251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce58fe5a8143c8a0846eed58e90fbb63bc9a1ae19c9d0164e173fa7dd0a587d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:39:28 GMT
COPY dir:7c6c6be58d44c17cd09173c77ba1f0d96ed42a5b7ef2235235262bdd0141924b in /opt/java/openjdk 
# Wed, 25 Jan 2023 01:07:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 25 Jan 2023 01:07:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Wed, 25 Jan 2023 01:07:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 25 Jan 2023 01:07:13 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Wed, 25 Jan 2023 01:07:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Jan 2023 01:07:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 01:07:25 GMT
WORKDIR /var/lib/neo4j
# Wed, 25 Jan 2023 01:07:25 GMT
VOLUME [/data /logs]
# Wed, 25 Jan 2023 01:07:26 GMT
EXPOSE 7473 7474 7687
# Wed, 25 Jan 2023 01:07:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 25 Jan 2023 01:07:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a47d09ee4791f80acce6e1c0ec8e323c79df787142099f3b440887c41fbeeaf`  
		Last Modified: Wed, 25 Jan 2023 00:54:33 GMT  
		Size: 198.5 MB (198475706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6389abf0a877313b2cd386d6e0a79b69e1f2991846abf96ed7338252e7b748`  
		Last Modified: Wed, 25 Jan 2023 01:09:47 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7443393411952dbce54fd972a76a199da113cb95e38d016e9a4d7d0762ecd73`  
		Last Modified: Wed, 25 Jan 2023 01:09:47 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f18c11095f94baffd79664a230414f6590241d5c6b793b782085c4db53080a`  
		Last Modified: Wed, 25 Jan 2023 01:09:54 GMT  
		Size: 136.9 MB (136883542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8da5083a3f14e43acd769e664938116a73f38b31f88bd58e5746ea09e01471da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (362037380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3a125530376e46b806b5d3f5a7a7d1151dd8efcf4d1030185bac0c491db011`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 20:59:22 GMT
COPY dir:b5081ac7f31ec5da21215ff6126fdb71f9fa63a8c9b5dc5e3f45f611c1765726 in /opt/java/openjdk 
# Tue, 24 Jan 2023 21:23:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 24 Jan 2023 21:23:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Tue, 24 Jan 2023 21:23:27 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 24 Jan 2023 21:23:27 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 24 Jan 2023 21:23:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 24 Jan 2023 21:23:41 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:23:42 GMT
WORKDIR /var/lib/neo4j
# Tue, 24 Jan 2023 21:23:42 GMT
VOLUME [/data /logs]
# Tue, 24 Jan 2023 21:23:42 GMT
EXPOSE 7473 7474 7687
# Tue, 24 Jan 2023 21:23:42 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 24 Jan 2023 21:23:42 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8fec50bc484d6341eb4f90d4749394a389a13ec00c2b3ab78c9140d9d4cda0`  
		Last Modified: Tue, 24 Jan 2023 21:11:01 GMT  
		Size: 195.2 MB (195239953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b52c77927d8d2e485192a8d752f867d8024b262943748c71854ecdd831b3b`  
		Last Modified: Tue, 24 Jan 2023 21:25:21 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b0cb9ba3614914e8bbd97d58661197655cbc02d0b99cd70fccf61dd1e76b7f`  
		Last Modified: Tue, 24 Jan 2023 21:25:21 GMT  
		Size: 8.2 KB (8169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aabba8a30d8f3a58d58599d6f9643cd5fa04b27cec324e1acac4cce3dfea88e`  
		Last Modified: Tue, 24 Jan 2023 21:25:27 GMT  
		Size: 136.7 MB (136740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:0ee890b73a6f61cbcbfc10d0e38eedb207866b3d0c8209ae7fb0dac6259c2908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:1a77c6d92542a6cd8ea4a79e03db440e730fddc21605c8f1bed187410a441d74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366768251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce58fe5a8143c8a0846eed58e90fbb63bc9a1ae19c9d0164e173fa7dd0a587d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:39:28 GMT
COPY dir:7c6c6be58d44c17cd09173c77ba1f0d96ed42a5b7ef2235235262bdd0141924b in /opt/java/openjdk 
# Wed, 25 Jan 2023 01:07:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 25 Jan 2023 01:07:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Wed, 25 Jan 2023 01:07:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 25 Jan 2023 01:07:13 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Wed, 25 Jan 2023 01:07:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Jan 2023 01:07:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 01:07:25 GMT
WORKDIR /var/lib/neo4j
# Wed, 25 Jan 2023 01:07:25 GMT
VOLUME [/data /logs]
# Wed, 25 Jan 2023 01:07:26 GMT
EXPOSE 7473 7474 7687
# Wed, 25 Jan 2023 01:07:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 25 Jan 2023 01:07:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a47d09ee4791f80acce6e1c0ec8e323c79df787142099f3b440887c41fbeeaf`  
		Last Modified: Wed, 25 Jan 2023 00:54:33 GMT  
		Size: 198.5 MB (198475706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6389abf0a877313b2cd386d6e0a79b69e1f2991846abf96ed7338252e7b748`  
		Last Modified: Wed, 25 Jan 2023 01:09:47 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7443393411952dbce54fd972a76a199da113cb95e38d016e9a4d7d0762ecd73`  
		Last Modified: Wed, 25 Jan 2023 01:09:47 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f18c11095f94baffd79664a230414f6590241d5c6b793b782085c4db53080a`  
		Last Modified: Wed, 25 Jan 2023 01:09:54 GMT  
		Size: 136.9 MB (136883542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8da5083a3f14e43acd769e664938116a73f38b31f88bd58e5746ea09e01471da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (362037380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3a125530376e46b806b5d3f5a7a7d1151dd8efcf4d1030185bac0c491db011`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 20:59:22 GMT
COPY dir:b5081ac7f31ec5da21215ff6126fdb71f9fa63a8c9b5dc5e3f45f611c1765726 in /opt/java/openjdk 
# Tue, 24 Jan 2023 21:23:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 24 Jan 2023 21:23:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Tue, 24 Jan 2023 21:23:27 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 24 Jan 2023 21:23:27 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 24 Jan 2023 21:23:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 24 Jan 2023 21:23:41 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:23:42 GMT
WORKDIR /var/lib/neo4j
# Tue, 24 Jan 2023 21:23:42 GMT
VOLUME [/data /logs]
# Tue, 24 Jan 2023 21:23:42 GMT
EXPOSE 7473 7474 7687
# Tue, 24 Jan 2023 21:23:42 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 24 Jan 2023 21:23:42 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8fec50bc484d6341eb4f90d4749394a389a13ec00c2b3ab78c9140d9d4cda0`  
		Last Modified: Tue, 24 Jan 2023 21:11:01 GMT  
		Size: 195.2 MB (195239953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b52c77927d8d2e485192a8d752f867d8024b262943748c71854ecdd831b3b`  
		Last Modified: Tue, 24 Jan 2023 21:25:21 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b0cb9ba3614914e8bbd97d58661197655cbc02d0b99cd70fccf61dd1e76b7f`  
		Last Modified: Tue, 24 Jan 2023 21:25:21 GMT  
		Size: 8.2 KB (8169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aabba8a30d8f3a58d58599d6f9643cd5fa04b27cec324e1acac4cce3dfea88e`  
		Last Modified: Tue, 24 Jan 2023 21:25:27 GMT  
		Size: 136.7 MB (136740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:26d98d8d81282bb6f7b4249d12dc6ea640d515d7ddc196c37815ced2447f7614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:11fc6631fc5bdd868f5a5d786a2b7865ee766becdac8c89ba08d20c909da7b4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.1 MB (463095083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b33c60315de60ce15bb74deffa48381e71cd194928fafecba5ba730ca96e083`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:39:28 GMT
COPY dir:7c6c6be58d44c17cd09173c77ba1f0d96ed42a5b7ef2235235262bdd0141924b in /opt/java/openjdk 
# Wed, 25 Jan 2023 01:07:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c4db0c4625e4c56a74140560601524bd6dd44e00de9b61b6c23cda71aaaf18c3 NEO4J_TARBALL=neo4j-enterprise-4.4.16-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 25 Jan 2023 01:07:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
# Wed, 25 Jan 2023 01:07:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 25 Jan 2023 01:07:30 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Wed, 25 Jan 2023 01:07:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Jan 2023 01:07:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 01:07:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 25 Jan 2023 01:07:45 GMT
VOLUME [/data /logs]
# Wed, 25 Jan 2023 01:07:45 GMT
EXPOSE 7473 7474 7687
# Wed, 25 Jan 2023 01:07:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 25 Jan 2023 01:07:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a47d09ee4791f80acce6e1c0ec8e323c79df787142099f3b440887c41fbeeaf`  
		Last Modified: Wed, 25 Jan 2023 00:54:33 GMT  
		Size: 198.5 MB (198475706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf0e9e30357b6414a7f6c6a47fc44f66d81619215868cb6923224c0423b2ad0`  
		Last Modified: Wed, 25 Jan 2023 01:10:07 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e34e3d6e8a2298b473ca684635895d41db65c8c3ef7b7d56527ce2082e358c`  
		Last Modified: Wed, 25 Jan 2023 01:10:06 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87574904e3acd4c8b1c690a8b4db6442a3060af184a4230fe0086db3067d3f1b`  
		Last Modified: Wed, 25 Jan 2023 01:10:18 GMT  
		Size: 233.2 MB (233210366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:51d2d753a1f45e26281bdc355f10a668db8a26acfb731e96e94e8dec3ccfd3d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458364158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e48f2301f51e0c1f2ac87f64e24d9556c0624dd208caf06ac94495f118a7a48e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 20:59:22 GMT
COPY dir:b5081ac7f31ec5da21215ff6126fdb71f9fa63a8c9b5dc5e3f45f611c1765726 in /opt/java/openjdk 
# Tue, 24 Jan 2023 21:23:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c4db0c4625e4c56a74140560601524bd6dd44e00de9b61b6c23cda71aaaf18c3 NEO4J_TARBALL=neo4j-enterprise-4.4.16-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 24 Jan 2023 21:23:46 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
# Tue, 24 Jan 2023 21:23:47 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 24 Jan 2023 21:23:47 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 24 Jan 2023 21:24:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 24 Jan 2023 21:24:08 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:24:08 GMT
WORKDIR /var/lib/neo4j
# Tue, 24 Jan 2023 21:24:08 GMT
VOLUME [/data /logs]
# Tue, 24 Jan 2023 21:24:08 GMT
EXPOSE 7473 7474 7687
# Tue, 24 Jan 2023 21:24:08 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 24 Jan 2023 21:24:08 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8fec50bc484d6341eb4f90d4749394a389a13ec00c2b3ab78c9140d9d4cda0`  
		Last Modified: Tue, 24 Jan 2023 21:11:01 GMT  
		Size: 195.2 MB (195239953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bf483f53dbf1548e92dcc5790c02a84724ff0c256c4ca5a3949d562c28656b`  
		Last Modified: Tue, 24 Jan 2023 21:25:39 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de0a2069d0c0481d1bdc6839a70cefc1d063cd2ec5d548ca666e7736172319d`  
		Last Modified: Tue, 24 Jan 2023 21:25:39 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1602de26e151043b7887f949b827eff8c4c1a3f657da8901942ee931b17c35b1`  
		Last Modified: Tue, 24 Jan 2023 21:25:49 GMT  
		Size: 233.1 MB (233067332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.16`

```console
$ docker pull neo4j@sha256:0ee890b73a6f61cbcbfc10d0e38eedb207866b3d0c8209ae7fb0dac6259c2908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.16` - linux; amd64

```console
$ docker pull neo4j@sha256:1a77c6d92542a6cd8ea4a79e03db440e730fddc21605c8f1bed187410a441d74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366768251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce58fe5a8143c8a0846eed58e90fbb63bc9a1ae19c9d0164e173fa7dd0a587d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:39:28 GMT
COPY dir:7c6c6be58d44c17cd09173c77ba1f0d96ed42a5b7ef2235235262bdd0141924b in /opt/java/openjdk 
# Wed, 25 Jan 2023 01:07:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 25 Jan 2023 01:07:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Wed, 25 Jan 2023 01:07:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 25 Jan 2023 01:07:13 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Wed, 25 Jan 2023 01:07:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Jan 2023 01:07:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 01:07:25 GMT
WORKDIR /var/lib/neo4j
# Wed, 25 Jan 2023 01:07:25 GMT
VOLUME [/data /logs]
# Wed, 25 Jan 2023 01:07:26 GMT
EXPOSE 7473 7474 7687
# Wed, 25 Jan 2023 01:07:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 25 Jan 2023 01:07:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a47d09ee4791f80acce6e1c0ec8e323c79df787142099f3b440887c41fbeeaf`  
		Last Modified: Wed, 25 Jan 2023 00:54:33 GMT  
		Size: 198.5 MB (198475706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6389abf0a877313b2cd386d6e0a79b69e1f2991846abf96ed7338252e7b748`  
		Last Modified: Wed, 25 Jan 2023 01:09:47 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7443393411952dbce54fd972a76a199da113cb95e38d016e9a4d7d0762ecd73`  
		Last Modified: Wed, 25 Jan 2023 01:09:47 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f18c11095f94baffd79664a230414f6590241d5c6b793b782085c4db53080a`  
		Last Modified: Wed, 25 Jan 2023 01:09:54 GMT  
		Size: 136.9 MB (136883542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.16` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8da5083a3f14e43acd769e664938116a73f38b31f88bd58e5746ea09e01471da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (362037380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3a125530376e46b806b5d3f5a7a7d1151dd8efcf4d1030185bac0c491db011`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 20:59:22 GMT
COPY dir:b5081ac7f31ec5da21215ff6126fdb71f9fa63a8c9b5dc5e3f45f611c1765726 in /opt/java/openjdk 
# Tue, 24 Jan 2023 21:23:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 24 Jan 2023 21:23:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Tue, 24 Jan 2023 21:23:27 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 24 Jan 2023 21:23:27 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 24 Jan 2023 21:23:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 24 Jan 2023 21:23:41 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:23:42 GMT
WORKDIR /var/lib/neo4j
# Tue, 24 Jan 2023 21:23:42 GMT
VOLUME [/data /logs]
# Tue, 24 Jan 2023 21:23:42 GMT
EXPOSE 7473 7474 7687
# Tue, 24 Jan 2023 21:23:42 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 24 Jan 2023 21:23:42 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8fec50bc484d6341eb4f90d4749394a389a13ec00c2b3ab78c9140d9d4cda0`  
		Last Modified: Tue, 24 Jan 2023 21:11:01 GMT  
		Size: 195.2 MB (195239953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b52c77927d8d2e485192a8d752f867d8024b262943748c71854ecdd831b3b`  
		Last Modified: Tue, 24 Jan 2023 21:25:21 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b0cb9ba3614914e8bbd97d58661197655cbc02d0b99cd70fccf61dd1e76b7f`  
		Last Modified: Tue, 24 Jan 2023 21:25:21 GMT  
		Size: 8.2 KB (8169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aabba8a30d8f3a58d58599d6f9643cd5fa04b27cec324e1acac4cce3dfea88e`  
		Last Modified: Tue, 24 Jan 2023 21:25:27 GMT  
		Size: 136.7 MB (136740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.16-community`

```console
$ docker pull neo4j@sha256:0ee890b73a6f61cbcbfc10d0e38eedb207866b3d0c8209ae7fb0dac6259c2908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.16-community` - linux; amd64

```console
$ docker pull neo4j@sha256:1a77c6d92542a6cd8ea4a79e03db440e730fddc21605c8f1bed187410a441d74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366768251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce58fe5a8143c8a0846eed58e90fbb63bc9a1ae19c9d0164e173fa7dd0a587d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:39:28 GMT
COPY dir:7c6c6be58d44c17cd09173c77ba1f0d96ed42a5b7ef2235235262bdd0141924b in /opt/java/openjdk 
# Wed, 25 Jan 2023 01:07:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 25 Jan 2023 01:07:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Wed, 25 Jan 2023 01:07:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 25 Jan 2023 01:07:13 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Wed, 25 Jan 2023 01:07:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Jan 2023 01:07:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 01:07:25 GMT
WORKDIR /var/lib/neo4j
# Wed, 25 Jan 2023 01:07:25 GMT
VOLUME [/data /logs]
# Wed, 25 Jan 2023 01:07:26 GMT
EXPOSE 7473 7474 7687
# Wed, 25 Jan 2023 01:07:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 25 Jan 2023 01:07:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a47d09ee4791f80acce6e1c0ec8e323c79df787142099f3b440887c41fbeeaf`  
		Last Modified: Wed, 25 Jan 2023 00:54:33 GMT  
		Size: 198.5 MB (198475706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6389abf0a877313b2cd386d6e0a79b69e1f2991846abf96ed7338252e7b748`  
		Last Modified: Wed, 25 Jan 2023 01:09:47 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7443393411952dbce54fd972a76a199da113cb95e38d016e9a4d7d0762ecd73`  
		Last Modified: Wed, 25 Jan 2023 01:09:47 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f18c11095f94baffd79664a230414f6590241d5c6b793b782085c4db53080a`  
		Last Modified: Wed, 25 Jan 2023 01:09:54 GMT  
		Size: 136.9 MB (136883542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.16-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8da5083a3f14e43acd769e664938116a73f38b31f88bd58e5746ea09e01471da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (362037380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3a125530376e46b806b5d3f5a7a7d1151dd8efcf4d1030185bac0c491db011`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 20:59:22 GMT
COPY dir:b5081ac7f31ec5da21215ff6126fdb71f9fa63a8c9b5dc5e3f45f611c1765726 in /opt/java/openjdk 
# Tue, 24 Jan 2023 21:23:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 24 Jan 2023 21:23:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Tue, 24 Jan 2023 21:23:27 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 24 Jan 2023 21:23:27 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 24 Jan 2023 21:23:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 24 Jan 2023 21:23:41 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:23:42 GMT
WORKDIR /var/lib/neo4j
# Tue, 24 Jan 2023 21:23:42 GMT
VOLUME [/data /logs]
# Tue, 24 Jan 2023 21:23:42 GMT
EXPOSE 7473 7474 7687
# Tue, 24 Jan 2023 21:23:42 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 24 Jan 2023 21:23:42 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8fec50bc484d6341eb4f90d4749394a389a13ec00c2b3ab78c9140d9d4cda0`  
		Last Modified: Tue, 24 Jan 2023 21:11:01 GMT  
		Size: 195.2 MB (195239953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b52c77927d8d2e485192a8d752f867d8024b262943748c71854ecdd831b3b`  
		Last Modified: Tue, 24 Jan 2023 21:25:21 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b0cb9ba3614914e8bbd97d58661197655cbc02d0b99cd70fccf61dd1e76b7f`  
		Last Modified: Tue, 24 Jan 2023 21:25:21 GMT  
		Size: 8.2 KB (8169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aabba8a30d8f3a58d58599d6f9643cd5fa04b27cec324e1acac4cce3dfea88e`  
		Last Modified: Tue, 24 Jan 2023 21:25:27 GMT  
		Size: 136.7 MB (136740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.16-enterprise`

```console
$ docker pull neo4j@sha256:26d98d8d81282bb6f7b4249d12dc6ea640d515d7ddc196c37815ced2447f7614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.16-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:11fc6631fc5bdd868f5a5d786a2b7865ee766becdac8c89ba08d20c909da7b4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.1 MB (463095083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b33c60315de60ce15bb74deffa48381e71cd194928fafecba5ba730ca96e083`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:39:28 GMT
COPY dir:7c6c6be58d44c17cd09173c77ba1f0d96ed42a5b7ef2235235262bdd0141924b in /opt/java/openjdk 
# Wed, 25 Jan 2023 01:07:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c4db0c4625e4c56a74140560601524bd6dd44e00de9b61b6c23cda71aaaf18c3 NEO4J_TARBALL=neo4j-enterprise-4.4.16-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 25 Jan 2023 01:07:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
# Wed, 25 Jan 2023 01:07:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 25 Jan 2023 01:07:30 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Wed, 25 Jan 2023 01:07:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Jan 2023 01:07:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 01:07:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 25 Jan 2023 01:07:45 GMT
VOLUME [/data /logs]
# Wed, 25 Jan 2023 01:07:45 GMT
EXPOSE 7473 7474 7687
# Wed, 25 Jan 2023 01:07:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 25 Jan 2023 01:07:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a47d09ee4791f80acce6e1c0ec8e323c79df787142099f3b440887c41fbeeaf`  
		Last Modified: Wed, 25 Jan 2023 00:54:33 GMT  
		Size: 198.5 MB (198475706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf0e9e30357b6414a7f6c6a47fc44f66d81619215868cb6923224c0423b2ad0`  
		Last Modified: Wed, 25 Jan 2023 01:10:07 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e34e3d6e8a2298b473ca684635895d41db65c8c3ef7b7d56527ce2082e358c`  
		Last Modified: Wed, 25 Jan 2023 01:10:06 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87574904e3acd4c8b1c690a8b4db6442a3060af184a4230fe0086db3067d3f1b`  
		Last Modified: Wed, 25 Jan 2023 01:10:18 GMT  
		Size: 233.2 MB (233210366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.16-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:51d2d753a1f45e26281bdc355f10a668db8a26acfb731e96e94e8dec3ccfd3d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458364158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e48f2301f51e0c1f2ac87f64e24d9556c0624dd208caf06ac94495f118a7a48e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 20:59:22 GMT
COPY dir:b5081ac7f31ec5da21215ff6126fdb71f9fa63a8c9b5dc5e3f45f611c1765726 in /opt/java/openjdk 
# Tue, 24 Jan 2023 21:23:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c4db0c4625e4c56a74140560601524bd6dd44e00de9b61b6c23cda71aaaf18c3 NEO4J_TARBALL=neo4j-enterprise-4.4.16-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 24 Jan 2023 21:23:46 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
# Tue, 24 Jan 2023 21:23:47 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 24 Jan 2023 21:23:47 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 24 Jan 2023 21:24:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 24 Jan 2023 21:24:08 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:24:08 GMT
WORKDIR /var/lib/neo4j
# Tue, 24 Jan 2023 21:24:08 GMT
VOLUME [/data /logs]
# Tue, 24 Jan 2023 21:24:08 GMT
EXPOSE 7473 7474 7687
# Tue, 24 Jan 2023 21:24:08 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 24 Jan 2023 21:24:08 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8fec50bc484d6341eb4f90d4749394a389a13ec00c2b3ab78c9140d9d4cda0`  
		Last Modified: Tue, 24 Jan 2023 21:11:01 GMT  
		Size: 195.2 MB (195239953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bf483f53dbf1548e92dcc5790c02a84724ff0c256c4ca5a3949d562c28656b`  
		Last Modified: Tue, 24 Jan 2023 21:25:39 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de0a2069d0c0481d1bdc6839a70cefc1d063cd2ec5d548ca666e7736172319d`  
		Last Modified: Tue, 24 Jan 2023 21:25:39 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1602de26e151043b7887f949b827eff8c4c1a3f657da8901942ee931b17c35b1`  
		Last Modified: Tue, 24 Jan 2023 21:25:49 GMT  
		Size: 233.1 MB (233067332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:4da73555d51ae5a40b698bc9654c9d629e3a972040be0bb7c22d4e04865c5342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:79c2a5802ac0684fbce0d85421d0cb994967f4f57c7b9d8152ee26890b45aa60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338568057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801d7a542ed2c02db9b9a2984cf97d5b2a298b56bf1b36e27735a380934afc83`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:19:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:19:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:19:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:19:52 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:06 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:06 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:06 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d46b5ccec1c38088acc371a620c831f87e7954f5274fe56194ad0fc35d51`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d912719189eb3a824e515e108b0e1eb5067c9ccc1b821183ec5aef7fe64db`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 8.3 KB (8338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beaef1edc03f7eca9434fbd08ebc846f5ebde22524306bd963c7390affea6a72`  
		Last Modified: Fri, 27 Jan 2023 20:21:00 GMT  
		Size: 114.7 MB (114720741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fa8d67f81f72551bf4f03be555e4ad3a2a262f33b1e3c31de06040b3e69d02a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7389ff6917629855abdeaa437e2becdc1b14b80af326e21533f40c4cb241a3bd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:10 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:21 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:21 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:21 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db6ad68d5043079adfe47bcd5eea82a6b923a893c3d56c82b7655371f544280`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398d73d2bf5d1dba7105ca31b65ad4d44e4c0bab7a6a627b4427d20e8dc5954d`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7bb5b9140f835f1d3638d645d54df4ce5f594068484b4d5ce7ff3474318ebb`  
		Last Modified: Fri, 27 Jan 2023 21:18:12 GMT  
		Size: 114.6 MB (114579133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:4da73555d51ae5a40b698bc9654c9d629e3a972040be0bb7c22d4e04865c5342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:79c2a5802ac0684fbce0d85421d0cb994967f4f57c7b9d8152ee26890b45aa60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338568057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801d7a542ed2c02db9b9a2984cf97d5b2a298b56bf1b36e27735a380934afc83`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:19:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:19:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:19:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:19:52 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:06 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:06 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:06 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d46b5ccec1c38088acc371a620c831f87e7954f5274fe56194ad0fc35d51`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d912719189eb3a824e515e108b0e1eb5067c9ccc1b821183ec5aef7fe64db`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 8.3 KB (8338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beaef1edc03f7eca9434fbd08ebc846f5ebde22524306bd963c7390affea6a72`  
		Last Modified: Fri, 27 Jan 2023 20:21:00 GMT  
		Size: 114.7 MB (114720741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fa8d67f81f72551bf4f03be555e4ad3a2a262f33b1e3c31de06040b3e69d02a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7389ff6917629855abdeaa437e2becdc1b14b80af326e21533f40c4cb241a3bd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:10 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:21 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:21 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:21 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db6ad68d5043079adfe47bcd5eea82a6b923a893c3d56c82b7655371f544280`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398d73d2bf5d1dba7105ca31b65ad4d44e4c0bab7a6a627b4427d20e8dc5954d`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7bb5b9140f835f1d3638d645d54df4ce5f594068484b4d5ce7ff3474318ebb`  
		Last Modified: Fri, 27 Jan 2023 21:18:12 GMT  
		Size: 114.6 MB (114579133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:5334b27b9faf870c74e394e00151db55b8fbadaf29a20d3d5a2a91b89ea1e61d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:09d06457fb046eb160f61aeb450484f4925752388debf7de3b9e0c1d05d468a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.2 MB (435231079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456927c0a42bf8702e91faada62e663c7acddc4f7e6cdb32e7192619d534f5ee`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:20:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:20:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:20:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:20:12 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:27 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:27 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:27 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:28 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05ec86513c46a7008e540f20832efaf9f73c252fe37f08cc42f963b0588fb18`  
		Last Modified: Fri, 27 Jan 2023 20:21:20 GMT  
		Size: 3.9 KB (3861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdc4b157743113125f0f33b6c196bf0d3e7b682e489d46f12d582c7aca5f6ed`  
		Last Modified: Fri, 27 Jan 2023 20:21:20 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55006d4afdf1fdf021a7414bf8ffbde47e23ad952a7a450249aa81ecffc1a0b6`  
		Last Modified: Fri, 27 Jan 2023 20:21:30 GMT  
		Size: 211.4 MB (211383759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:86a89bad9fb57937f16ba30a4947b85fdffeac074b3fcfa1857df152a9ab54d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292bc7a8cff1db20841e7def11fd2d472285eefdc2ed7877fa76a7b4c09c294`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:26 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:37 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:38 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:38 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:39 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167a2537c000981c0f5bee543f87848394744dd6f3a8e6d9c47bd49c8af6bc1f`  
		Last Modified: Fri, 27 Jan 2023 21:18:31 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cfd7e05443a755b252a2b77efbe931f20279a00c2b6fd25a1f9d24808ff36cf`  
		Last Modified: Fri, 27 Jan 2023 21:18:31 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e77e468dc817cb21ddcc704bbf32833a11836dbdf70286e63520041c54b63a4`  
		Last Modified: Fri, 27 Jan 2023 21:18:40 GMT  
		Size: 211.2 MB (211241012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4`

```console
$ docker pull neo4j@sha256:4da73555d51ae5a40b698bc9654c9d629e3a972040be0bb7c22d4e04865c5342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.4` - linux; amd64

```console
$ docker pull neo4j@sha256:79c2a5802ac0684fbce0d85421d0cb994967f4f57c7b9d8152ee26890b45aa60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338568057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801d7a542ed2c02db9b9a2984cf97d5b2a298b56bf1b36e27735a380934afc83`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:19:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:19:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:19:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:19:52 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:06 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:06 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:06 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d46b5ccec1c38088acc371a620c831f87e7954f5274fe56194ad0fc35d51`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d912719189eb3a824e515e108b0e1eb5067c9ccc1b821183ec5aef7fe64db`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 8.3 KB (8338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beaef1edc03f7eca9434fbd08ebc846f5ebde22524306bd963c7390affea6a72`  
		Last Modified: Fri, 27 Jan 2023 20:21:00 GMT  
		Size: 114.7 MB (114720741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fa8d67f81f72551bf4f03be555e4ad3a2a262f33b1e3c31de06040b3e69d02a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7389ff6917629855abdeaa437e2becdc1b14b80af326e21533f40c4cb241a3bd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:10 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:21 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:21 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:21 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db6ad68d5043079adfe47bcd5eea82a6b923a893c3d56c82b7655371f544280`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398d73d2bf5d1dba7105ca31b65ad4d44e4c0bab7a6a627b4427d20e8dc5954d`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7bb5b9140f835f1d3638d645d54df4ce5f594068484b4d5ce7ff3474318ebb`  
		Last Modified: Fri, 27 Jan 2023 21:18:12 GMT  
		Size: 114.6 MB (114579133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4-enterprise`

```console
$ docker pull neo4j@sha256:5334b27b9faf870c74e394e00151db55b8fbadaf29a20d3d5a2a91b89ea1e61d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:09d06457fb046eb160f61aeb450484f4925752388debf7de3b9e0c1d05d468a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.2 MB (435231079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456927c0a42bf8702e91faada62e663c7acddc4f7e6cdb32e7192619d534f5ee`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:20:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:20:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:20:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:20:12 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:27 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:27 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:27 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:28 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05ec86513c46a7008e540f20832efaf9f73c252fe37f08cc42f963b0588fb18`  
		Last Modified: Fri, 27 Jan 2023 20:21:20 GMT  
		Size: 3.9 KB (3861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdc4b157743113125f0f33b6c196bf0d3e7b682e489d46f12d582c7aca5f6ed`  
		Last Modified: Fri, 27 Jan 2023 20:21:20 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55006d4afdf1fdf021a7414bf8ffbde47e23ad952a7a450249aa81ecffc1a0b6`  
		Last Modified: Fri, 27 Jan 2023 20:21:30 GMT  
		Size: 211.4 MB (211383759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:86a89bad9fb57937f16ba30a4947b85fdffeac074b3fcfa1857df152a9ab54d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292bc7a8cff1db20841e7def11fd2d472285eefdc2ed7877fa76a7b4c09c294`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:26 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:37 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:38 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:38 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:39 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167a2537c000981c0f5bee543f87848394744dd6f3a8e6d9c47bd49c8af6bc1f`  
		Last Modified: Fri, 27 Jan 2023 21:18:31 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cfd7e05443a755b252a2b77efbe931f20279a00c2b6fd25a1f9d24808ff36cf`  
		Last Modified: Fri, 27 Jan 2023 21:18:31 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e77e468dc817cb21ddcc704bbf32833a11836dbdf70286e63520041c54b63a4`  
		Last Modified: Fri, 27 Jan 2023 21:18:40 GMT  
		Size: 211.2 MB (211241012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4.0`

```console
$ docker pull neo4j@sha256:4da73555d51ae5a40b698bc9654c9d629e3a972040be0bb7c22d4e04865c5342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.4.0` - linux; amd64

```console
$ docker pull neo4j@sha256:79c2a5802ac0684fbce0d85421d0cb994967f4f57c7b9d8152ee26890b45aa60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338568057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801d7a542ed2c02db9b9a2984cf97d5b2a298b56bf1b36e27735a380934afc83`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:19:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:19:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:19:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:19:52 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:06 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:06 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:06 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d46b5ccec1c38088acc371a620c831f87e7954f5274fe56194ad0fc35d51`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d912719189eb3a824e515e108b0e1eb5067c9ccc1b821183ec5aef7fe64db`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 8.3 KB (8338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beaef1edc03f7eca9434fbd08ebc846f5ebde22524306bd963c7390affea6a72`  
		Last Modified: Fri, 27 Jan 2023 20:21:00 GMT  
		Size: 114.7 MB (114720741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.4.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fa8d67f81f72551bf4f03be555e4ad3a2a262f33b1e3c31de06040b3e69d02a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7389ff6917629855abdeaa437e2becdc1b14b80af326e21533f40c4cb241a3bd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:10 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:21 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:21 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:21 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db6ad68d5043079adfe47bcd5eea82a6b923a893c3d56c82b7655371f544280`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398d73d2bf5d1dba7105ca31b65ad4d44e4c0bab7a6a627b4427d20e8dc5954d`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7bb5b9140f835f1d3638d645d54df4ce5f594068484b4d5ce7ff3474318ebb`  
		Last Modified: Fri, 27 Jan 2023 21:18:12 GMT  
		Size: 114.6 MB (114579133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4.0-community`

```console
$ docker pull neo4j@sha256:4da73555d51ae5a40b698bc9654c9d629e3a972040be0bb7c22d4e04865c5342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.4.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:79c2a5802ac0684fbce0d85421d0cb994967f4f57c7b9d8152ee26890b45aa60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338568057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801d7a542ed2c02db9b9a2984cf97d5b2a298b56bf1b36e27735a380934afc83`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:19:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:19:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:19:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:19:52 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:06 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:06 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:06 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d46b5ccec1c38088acc371a620c831f87e7954f5274fe56194ad0fc35d51`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d912719189eb3a824e515e108b0e1eb5067c9ccc1b821183ec5aef7fe64db`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 8.3 KB (8338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beaef1edc03f7eca9434fbd08ebc846f5ebde22524306bd963c7390affea6a72`  
		Last Modified: Fri, 27 Jan 2023 20:21:00 GMT  
		Size: 114.7 MB (114720741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.4.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fa8d67f81f72551bf4f03be555e4ad3a2a262f33b1e3c31de06040b3e69d02a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7389ff6917629855abdeaa437e2becdc1b14b80af326e21533f40c4cb241a3bd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:10 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:21 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:21 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:21 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db6ad68d5043079adfe47bcd5eea82a6b923a893c3d56c82b7655371f544280`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398d73d2bf5d1dba7105ca31b65ad4d44e4c0bab7a6a627b4427d20e8dc5954d`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7bb5b9140f835f1d3638d645d54df4ce5f594068484b4d5ce7ff3474318ebb`  
		Last Modified: Fri, 27 Jan 2023 21:18:12 GMT  
		Size: 114.6 MB (114579133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4.0-enterprise`

```console
$ docker pull neo4j@sha256:5334b27b9faf870c74e394e00151db55b8fbadaf29a20d3d5a2a91b89ea1e61d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.4.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:09d06457fb046eb160f61aeb450484f4925752388debf7de3b9e0c1d05d468a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.2 MB (435231079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456927c0a42bf8702e91faada62e663c7acddc4f7e6cdb32e7192619d534f5ee`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:20:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:20:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:20:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:20:12 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:27 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:27 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:27 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:28 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05ec86513c46a7008e540f20832efaf9f73c252fe37f08cc42f963b0588fb18`  
		Last Modified: Fri, 27 Jan 2023 20:21:20 GMT  
		Size: 3.9 KB (3861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdc4b157743113125f0f33b6c196bf0d3e7b682e489d46f12d582c7aca5f6ed`  
		Last Modified: Fri, 27 Jan 2023 20:21:20 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55006d4afdf1fdf021a7414bf8ffbde47e23ad952a7a450249aa81ecffc1a0b6`  
		Last Modified: Fri, 27 Jan 2023 20:21:30 GMT  
		Size: 211.4 MB (211383759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.4.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:86a89bad9fb57937f16ba30a4947b85fdffeac074b3fcfa1857df152a9ab54d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292bc7a8cff1db20841e7def11fd2d472285eefdc2ed7877fa76a7b4c09c294`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:26 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:37 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:38 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:38 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:39 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167a2537c000981c0f5bee543f87848394744dd6f3a8e6d9c47bd49c8af6bc1f`  
		Last Modified: Fri, 27 Jan 2023 21:18:31 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cfd7e05443a755b252a2b77efbe931f20279a00c2b6fd25a1f9d24808ff36cf`  
		Last Modified: Fri, 27 Jan 2023 21:18:31 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e77e468dc817cb21ddcc704bbf32833a11836dbdf70286e63520041c54b63a4`  
		Last Modified: Fri, 27 Jan 2023 21:18:40 GMT  
		Size: 211.2 MB (211241012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:4da73555d51ae5a40b698bc9654c9d629e3a972040be0bb7c22d4e04865c5342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:79c2a5802ac0684fbce0d85421d0cb994967f4f57c7b9d8152ee26890b45aa60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338568057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801d7a542ed2c02db9b9a2984cf97d5b2a298b56bf1b36e27735a380934afc83`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:19:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:19:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:19:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:19:52 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:06 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:06 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:06 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d46b5ccec1c38088acc371a620c831f87e7954f5274fe56194ad0fc35d51`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d912719189eb3a824e515e108b0e1eb5067c9ccc1b821183ec5aef7fe64db`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 8.3 KB (8338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beaef1edc03f7eca9434fbd08ebc846f5ebde22524306bd963c7390affea6a72`  
		Last Modified: Fri, 27 Jan 2023 20:21:00 GMT  
		Size: 114.7 MB (114720741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fa8d67f81f72551bf4f03be555e4ad3a2a262f33b1e3c31de06040b3e69d02a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7389ff6917629855abdeaa437e2becdc1b14b80af326e21533f40c4cb241a3bd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:10 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:21 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:21 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:21 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db6ad68d5043079adfe47bcd5eea82a6b923a893c3d56c82b7655371f544280`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398d73d2bf5d1dba7105ca31b65ad4d44e4c0bab7a6a627b4427d20e8dc5954d`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7bb5b9140f835f1d3638d645d54df4ce5f594068484b4d5ce7ff3474318ebb`  
		Last Modified: Fri, 27 Jan 2023 21:18:12 GMT  
		Size: 114.6 MB (114579133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:5334b27b9faf870c74e394e00151db55b8fbadaf29a20d3d5a2a91b89ea1e61d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:09d06457fb046eb160f61aeb450484f4925752388debf7de3b9e0c1d05d468a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.2 MB (435231079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456927c0a42bf8702e91faada62e663c7acddc4f7e6cdb32e7192619d534f5ee`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:20:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:20:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:20:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:20:12 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:27 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:27 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:27 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:28 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05ec86513c46a7008e540f20832efaf9f73c252fe37f08cc42f963b0588fb18`  
		Last Modified: Fri, 27 Jan 2023 20:21:20 GMT  
		Size: 3.9 KB (3861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdc4b157743113125f0f33b6c196bf0d3e7b682e489d46f12d582c7aca5f6ed`  
		Last Modified: Fri, 27 Jan 2023 20:21:20 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55006d4afdf1fdf021a7414bf8ffbde47e23ad952a7a450249aa81ecffc1a0b6`  
		Last Modified: Fri, 27 Jan 2023 20:21:30 GMT  
		Size: 211.4 MB (211383759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:86a89bad9fb57937f16ba30a4947b85fdffeac074b3fcfa1857df152a9ab54d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292bc7a8cff1db20841e7def11fd2d472285eefdc2ed7877fa76a7b4c09c294`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:26 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:37 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:38 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:38 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:39 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167a2537c000981c0f5bee543f87848394744dd6f3a8e6d9c47bd49c8af6bc1f`  
		Last Modified: Fri, 27 Jan 2023 21:18:31 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cfd7e05443a755b252a2b77efbe931f20279a00c2b6fd25a1f9d24808ff36cf`  
		Last Modified: Fri, 27 Jan 2023 21:18:31 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e77e468dc817cb21ddcc704bbf32833a11836dbdf70286e63520041c54b63a4`  
		Last Modified: Fri, 27 Jan 2023 21:18:40 GMT  
		Size: 211.2 MB (211241012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:4da73555d51ae5a40b698bc9654c9d629e3a972040be0bb7c22d4e04865c5342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:79c2a5802ac0684fbce0d85421d0cb994967f4f57c7b9d8152ee26890b45aa60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338568057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801d7a542ed2c02db9b9a2984cf97d5b2a298b56bf1b36e27735a380934afc83`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:19:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:19:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:19:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:19:52 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:06 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:06 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:06 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d46b5ccec1c38088acc371a620c831f87e7954f5274fe56194ad0fc35d51`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d912719189eb3a824e515e108b0e1eb5067c9ccc1b821183ec5aef7fe64db`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 8.3 KB (8338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beaef1edc03f7eca9434fbd08ebc846f5ebde22524306bd963c7390affea6a72`  
		Last Modified: Fri, 27 Jan 2023 20:21:00 GMT  
		Size: 114.7 MB (114720741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fa8d67f81f72551bf4f03be555e4ad3a2a262f33b1e3c31de06040b3e69d02a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7389ff6917629855abdeaa437e2becdc1b14b80af326e21533f40c4cb241a3bd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:10 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:21 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:21 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:21 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db6ad68d5043079adfe47bcd5eea82a6b923a893c3d56c82b7655371f544280`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398d73d2bf5d1dba7105ca31b65ad4d44e4c0bab7a6a627b4427d20e8dc5954d`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7bb5b9140f835f1d3638d645d54df4ce5f594068484b4d5ce7ff3474318ebb`  
		Last Modified: Fri, 27 Jan 2023 21:18:12 GMT  
		Size: 114.6 MB (114579133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
