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
$ docker pull neo4j@sha256:0af0b4325a680e742ad3809133ff5de01ea9d9ea9c08f7599bf6c0b5cefc8ffd
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
$ docker pull neo4j@sha256:0df20d450c0ec047201e6fbbb3cab12ec6fb7f1a9c5c280e23e9e1c345feefec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (362037825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f9d80ebc3071c067c7ad87f946d5c01418c49f8f899bee1ebe23c099a07f43`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:50:12 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:58:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:58:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Tue, 31 Jan 2023 21:58:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:58:11 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 31 Jan 2023 21:58:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:58:26 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:58:26 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:58:26 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:58:26 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:58:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:58:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5842b36268c5c5b9539a446d9eba4513a75b1955de0b698663ccf059458ac527`  
		Last Modified: Tue, 31 Jan 2023 21:04:34 GMT  
		Size: 195.2 MB (195240302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19061b4a9343921b04c67bfa4acd4d5710118cb35a25917c8956a8fc9f08253b`  
		Last Modified: Tue, 31 Jan 2023 21:59:54 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b45f0309ac4d360da743e7977656ac584ec56a0e28e02c346e6f4e3ed0dd9`  
		Last Modified: Tue, 31 Jan 2023 21:59:54 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e73f539c975416ebb24c1076d06474b54d0e0fae2b4ae44b50a8b4d94878137`  
		Last Modified: Tue, 31 Jan 2023 22:00:00 GMT  
		Size: 136.7 MB (136740647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:0af0b4325a680e742ad3809133ff5de01ea9d9ea9c08f7599bf6c0b5cefc8ffd
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
$ docker pull neo4j@sha256:0df20d450c0ec047201e6fbbb3cab12ec6fb7f1a9c5c280e23e9e1c345feefec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (362037825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f9d80ebc3071c067c7ad87f946d5c01418c49f8f899bee1ebe23c099a07f43`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:50:12 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:58:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:58:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Tue, 31 Jan 2023 21:58:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:58:11 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 31 Jan 2023 21:58:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:58:26 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:58:26 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:58:26 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:58:26 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:58:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:58:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5842b36268c5c5b9539a446d9eba4513a75b1955de0b698663ccf059458ac527`  
		Last Modified: Tue, 31 Jan 2023 21:04:34 GMT  
		Size: 195.2 MB (195240302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19061b4a9343921b04c67bfa4acd4d5710118cb35a25917c8956a8fc9f08253b`  
		Last Modified: Tue, 31 Jan 2023 21:59:54 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b45f0309ac4d360da743e7977656ac584ec56a0e28e02c346e6f4e3ed0dd9`  
		Last Modified: Tue, 31 Jan 2023 21:59:54 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e73f539c975416ebb24c1076d06474b54d0e0fae2b4ae44b50a8b4d94878137`  
		Last Modified: Tue, 31 Jan 2023 22:00:00 GMT  
		Size: 136.7 MB (136740647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:b998af9d214c23489f4acd19f866a91429dd746eaee3caafa86b23a61c301649
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
$ docker pull neo4j@sha256:bd9abfbda2cd35d0a1b4dd23559acd8a2915869fb4170188043b74770cd5879d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458364702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f6e10d836f69d07e0451628908f980b9eb958045bf94d3d1be26bc38efdf5ca`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:50:12 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:58:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c4db0c4625e4c56a74140560601524bd6dd44e00de9b61b6c23cda71aaaf18c3 NEO4J_TARBALL=neo4j-enterprise-4.4.16-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:58:31 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
# Tue, 31 Jan 2023 21:58:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:58:31 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 31 Jan 2023 21:58:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:58:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:58:45 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:58:45 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:58:45 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:58:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:58:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5842b36268c5c5b9539a446d9eba4513a75b1955de0b698663ccf059458ac527`  
		Last Modified: Tue, 31 Jan 2023 21:04:34 GMT  
		Size: 195.2 MB (195240302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3637bc047e35e88acc4a5de1f154aeac23285edd003d383878c0ed71c7c64ca`  
		Last Modified: Tue, 31 Jan 2023 22:00:16 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ded26bcf84143d3fe4f5a759df9594ad65ecf8d062089f45dab61a22948aae`  
		Last Modified: Tue, 31 Jan 2023 22:00:16 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269f3048c469729b05b4ae29241292c26c8fe95e3f06f1f5388e537b58a97103`  
		Last Modified: Tue, 31 Jan 2023 22:00:26 GMT  
		Size: 233.1 MB (233067523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.16`

```console
$ docker pull neo4j@sha256:0af0b4325a680e742ad3809133ff5de01ea9d9ea9c08f7599bf6c0b5cefc8ffd
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
$ docker pull neo4j@sha256:0df20d450c0ec047201e6fbbb3cab12ec6fb7f1a9c5c280e23e9e1c345feefec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (362037825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f9d80ebc3071c067c7ad87f946d5c01418c49f8f899bee1ebe23c099a07f43`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:50:12 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:58:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:58:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Tue, 31 Jan 2023 21:58:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:58:11 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 31 Jan 2023 21:58:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:58:26 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:58:26 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:58:26 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:58:26 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:58:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:58:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5842b36268c5c5b9539a446d9eba4513a75b1955de0b698663ccf059458ac527`  
		Last Modified: Tue, 31 Jan 2023 21:04:34 GMT  
		Size: 195.2 MB (195240302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19061b4a9343921b04c67bfa4acd4d5710118cb35a25917c8956a8fc9f08253b`  
		Last Modified: Tue, 31 Jan 2023 21:59:54 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b45f0309ac4d360da743e7977656ac584ec56a0e28e02c346e6f4e3ed0dd9`  
		Last Modified: Tue, 31 Jan 2023 21:59:54 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e73f539c975416ebb24c1076d06474b54d0e0fae2b4ae44b50a8b4d94878137`  
		Last Modified: Tue, 31 Jan 2023 22:00:00 GMT  
		Size: 136.7 MB (136740647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.16-community`

```console
$ docker pull neo4j@sha256:0af0b4325a680e742ad3809133ff5de01ea9d9ea9c08f7599bf6c0b5cefc8ffd
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
$ docker pull neo4j@sha256:0df20d450c0ec047201e6fbbb3cab12ec6fb7f1a9c5c280e23e9e1c345feefec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (362037825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f9d80ebc3071c067c7ad87f946d5c01418c49f8f899bee1ebe23c099a07f43`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:50:12 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:58:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9e4ae513dc1a297dc2cbf4f07af5ced366038055385de9c9d598df1b4aceed91 NEO4J_TARBALL=neo4j-community-4.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:58:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
# Tue, 31 Jan 2023 21:58:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:58:11 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 31 Jan 2023 21:58:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:58:26 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:58:26 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:58:26 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:58:26 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:58:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:58:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5842b36268c5c5b9539a446d9eba4513a75b1955de0b698663ccf059458ac527`  
		Last Modified: Tue, 31 Jan 2023 21:04:34 GMT  
		Size: 195.2 MB (195240302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19061b4a9343921b04c67bfa4acd4d5710118cb35a25917c8956a8fc9f08253b`  
		Last Modified: Tue, 31 Jan 2023 21:59:54 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b45f0309ac4d360da743e7977656ac584ec56a0e28e02c346e6f4e3ed0dd9`  
		Last Modified: Tue, 31 Jan 2023 21:59:54 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e73f539c975416ebb24c1076d06474b54d0e0fae2b4ae44b50a8b4d94878137`  
		Last Modified: Tue, 31 Jan 2023 22:00:00 GMT  
		Size: 136.7 MB (136740647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.16-enterprise`

```console
$ docker pull neo4j@sha256:b998af9d214c23489f4acd19f866a91429dd746eaee3caafa86b23a61c301649
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
$ docker pull neo4j@sha256:bd9abfbda2cd35d0a1b4dd23559acd8a2915869fb4170188043b74770cd5879d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458364702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f6e10d836f69d07e0451628908f980b9eb958045bf94d3d1be26bc38efdf5ca`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:50:12 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:58:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c4db0c4625e4c56a74140560601524bd6dd44e00de9b61b6c23cda71aaaf18c3 NEO4J_TARBALL=neo4j-enterprise-4.4.16-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:58:31 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
# Tue, 31 Jan 2023 21:58:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:58:31 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Tue, 31 Jan 2023 21:58:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:58:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:58:45 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:58:45 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:58:45 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:58:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:58:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5842b36268c5c5b9539a446d9eba4513a75b1955de0b698663ccf059458ac527`  
		Last Modified: Tue, 31 Jan 2023 21:04:34 GMT  
		Size: 195.2 MB (195240302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3637bc047e35e88acc4a5de1f154aeac23285edd003d383878c0ed71c7c64ca`  
		Last Modified: Tue, 31 Jan 2023 22:00:16 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ded26bcf84143d3fe4f5a759df9594ad65ecf8d062089f45dab61a22948aae`  
		Last Modified: Tue, 31 Jan 2023 22:00:16 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269f3048c469729b05b4ae29241292c26c8fe95e3f06f1f5388e537b58a97103`  
		Last Modified: Tue, 31 Jan 2023 22:00:26 GMT  
		Size: 233.1 MB (233067523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:67e9d04d3f796071778d301b6371cf89940a079e5db203afc969f830500303b8
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
$ docker pull neo4j@sha256:bf1d85b1081fd556288f0c204756b4db616740b5c4e88badcf1d443ca4d298ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da0dd68954d57ef80e0675d9a718b3246fb314e948876f4fef7943b654cb1cf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:57:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:57:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:57:50 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:57:50 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:57:50 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:57:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:57:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a5c4e04f9bcf426624cdddd72be1ee3b881e3343b3b4fdba019406e3e19c4`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b40a34bc69773588a218a7f59e57a44423c30b870271af697637e0b998a823`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7e2b8dcc69dc7857585c0a42bb279013e506142b19e3dcb30ca055674272b`  
		Last Modified: Tue, 31 Jan 2023 21:59:15 GMT  
		Size: 114.6 MB (114578996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:67e9d04d3f796071778d301b6371cf89940a079e5db203afc969f830500303b8
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
$ docker pull neo4j@sha256:bf1d85b1081fd556288f0c204756b4db616740b5c4e88badcf1d443ca4d298ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da0dd68954d57ef80e0675d9a718b3246fb314e948876f4fef7943b654cb1cf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:57:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:57:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:57:50 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:57:50 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:57:50 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:57:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:57:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a5c4e04f9bcf426624cdddd72be1ee3b881e3343b3b4fdba019406e3e19c4`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b40a34bc69773588a218a7f59e57a44423c30b870271af697637e0b998a823`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7e2b8dcc69dc7857585c0a42bb279013e506142b19e3dcb30ca055674272b`  
		Last Modified: Tue, 31 Jan 2023 21:59:15 GMT  
		Size: 114.6 MB (114578996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:f6958bb9e76b210c9599c9924e8aa91c1fb122cac5cbad5b1a18a1231bfdb0c8
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
$ docker pull neo4j@sha256:bfabb752fc0c628e37be06b1d26ef3534088afb7bfbba1adedb07645e87573bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06dd04bfe22073df40bd40c3852336e5c259200878ed779a35598c3ba4f268fe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:55 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:58:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:58:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:58:07 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:58:07 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:58:08 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:58:08 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:58:08 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483baeece87ea32f7b15e6242c8c556cd4580d42a4e2cf52d1e422cd79fff89a`  
		Last Modified: Tue, 31 Jan 2023 21:59:33 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90597eb3cb286c2822c1098bccfb8922aec2613e06c64fde55b43b429de94c9e`  
		Last Modified: Tue, 31 Jan 2023 21:59:33 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159934fd6a3375efa277859c7ea8d73ba4cdc2f1348518f23f2c8be09b264941`  
		Last Modified: Tue, 31 Jan 2023 21:59:41 GMT  
		Size: 211.2 MB (211241279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4`

```console
$ docker pull neo4j@sha256:67e9d04d3f796071778d301b6371cf89940a079e5db203afc969f830500303b8
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
$ docker pull neo4j@sha256:bf1d85b1081fd556288f0c204756b4db616740b5c4e88badcf1d443ca4d298ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da0dd68954d57ef80e0675d9a718b3246fb314e948876f4fef7943b654cb1cf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:57:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:57:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:57:50 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:57:50 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:57:50 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:57:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:57:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a5c4e04f9bcf426624cdddd72be1ee3b881e3343b3b4fdba019406e3e19c4`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b40a34bc69773588a218a7f59e57a44423c30b870271af697637e0b998a823`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7e2b8dcc69dc7857585c0a42bb279013e506142b19e3dcb30ca055674272b`  
		Last Modified: Tue, 31 Jan 2023 21:59:15 GMT  
		Size: 114.6 MB (114578996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4-enterprise`

```console
$ docker pull neo4j@sha256:f6958bb9e76b210c9599c9924e8aa91c1fb122cac5cbad5b1a18a1231bfdb0c8
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
$ docker pull neo4j@sha256:bfabb752fc0c628e37be06b1d26ef3534088afb7bfbba1adedb07645e87573bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06dd04bfe22073df40bd40c3852336e5c259200878ed779a35598c3ba4f268fe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:55 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:58:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:58:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:58:07 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:58:07 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:58:08 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:58:08 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:58:08 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483baeece87ea32f7b15e6242c8c556cd4580d42a4e2cf52d1e422cd79fff89a`  
		Last Modified: Tue, 31 Jan 2023 21:59:33 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90597eb3cb286c2822c1098bccfb8922aec2613e06c64fde55b43b429de94c9e`  
		Last Modified: Tue, 31 Jan 2023 21:59:33 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159934fd6a3375efa277859c7ea8d73ba4cdc2f1348518f23f2c8be09b264941`  
		Last Modified: Tue, 31 Jan 2023 21:59:41 GMT  
		Size: 211.2 MB (211241279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4.0`

```console
$ docker pull neo4j@sha256:67e9d04d3f796071778d301b6371cf89940a079e5db203afc969f830500303b8
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
$ docker pull neo4j@sha256:bf1d85b1081fd556288f0c204756b4db616740b5c4e88badcf1d443ca4d298ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da0dd68954d57ef80e0675d9a718b3246fb314e948876f4fef7943b654cb1cf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:57:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:57:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:57:50 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:57:50 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:57:50 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:57:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:57:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a5c4e04f9bcf426624cdddd72be1ee3b881e3343b3b4fdba019406e3e19c4`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b40a34bc69773588a218a7f59e57a44423c30b870271af697637e0b998a823`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7e2b8dcc69dc7857585c0a42bb279013e506142b19e3dcb30ca055674272b`  
		Last Modified: Tue, 31 Jan 2023 21:59:15 GMT  
		Size: 114.6 MB (114578996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4.0-community`

```console
$ docker pull neo4j@sha256:67e9d04d3f796071778d301b6371cf89940a079e5db203afc969f830500303b8
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
$ docker pull neo4j@sha256:bf1d85b1081fd556288f0c204756b4db616740b5c4e88badcf1d443ca4d298ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da0dd68954d57ef80e0675d9a718b3246fb314e948876f4fef7943b654cb1cf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:57:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:57:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:57:50 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:57:50 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:57:50 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:57:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:57:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a5c4e04f9bcf426624cdddd72be1ee3b881e3343b3b4fdba019406e3e19c4`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b40a34bc69773588a218a7f59e57a44423c30b870271af697637e0b998a823`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7e2b8dcc69dc7857585c0a42bb279013e506142b19e3dcb30ca055674272b`  
		Last Modified: Tue, 31 Jan 2023 21:59:15 GMT  
		Size: 114.6 MB (114578996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4.0-enterprise`

```console
$ docker pull neo4j@sha256:f6958bb9e76b210c9599c9924e8aa91c1fb122cac5cbad5b1a18a1231bfdb0c8
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
$ docker pull neo4j@sha256:bfabb752fc0c628e37be06b1d26ef3534088afb7bfbba1adedb07645e87573bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06dd04bfe22073df40bd40c3852336e5c259200878ed779a35598c3ba4f268fe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:55 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:58:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:58:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:58:07 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:58:07 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:58:08 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:58:08 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:58:08 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483baeece87ea32f7b15e6242c8c556cd4580d42a4e2cf52d1e422cd79fff89a`  
		Last Modified: Tue, 31 Jan 2023 21:59:33 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90597eb3cb286c2822c1098bccfb8922aec2613e06c64fde55b43b429de94c9e`  
		Last Modified: Tue, 31 Jan 2023 21:59:33 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159934fd6a3375efa277859c7ea8d73ba4cdc2f1348518f23f2c8be09b264941`  
		Last Modified: Tue, 31 Jan 2023 21:59:41 GMT  
		Size: 211.2 MB (211241279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:67e9d04d3f796071778d301b6371cf89940a079e5db203afc969f830500303b8
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
$ docker pull neo4j@sha256:bf1d85b1081fd556288f0c204756b4db616740b5c4e88badcf1d443ca4d298ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da0dd68954d57ef80e0675d9a718b3246fb314e948876f4fef7943b654cb1cf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:57:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:57:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:57:50 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:57:50 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:57:50 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:57:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:57:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a5c4e04f9bcf426624cdddd72be1ee3b881e3343b3b4fdba019406e3e19c4`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b40a34bc69773588a218a7f59e57a44423c30b870271af697637e0b998a823`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7e2b8dcc69dc7857585c0a42bb279013e506142b19e3dcb30ca055674272b`  
		Last Modified: Tue, 31 Jan 2023 21:59:15 GMT  
		Size: 114.6 MB (114578996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:f6958bb9e76b210c9599c9924e8aa91c1fb122cac5cbad5b1a18a1231bfdb0c8
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
$ docker pull neo4j@sha256:bfabb752fc0c628e37be06b1d26ef3534088afb7bfbba1adedb07645e87573bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06dd04bfe22073df40bd40c3852336e5c259200878ed779a35598c3ba4f268fe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:55 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:58:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:58:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:58:07 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:58:07 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:58:08 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:58:08 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:58:08 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483baeece87ea32f7b15e6242c8c556cd4580d42a4e2cf52d1e422cd79fff89a`  
		Last Modified: Tue, 31 Jan 2023 21:59:33 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90597eb3cb286c2822c1098bccfb8922aec2613e06c64fde55b43b429de94c9e`  
		Last Modified: Tue, 31 Jan 2023 21:59:33 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159934fd6a3375efa277859c7ea8d73ba4cdc2f1348518f23f2c8be09b264941`  
		Last Modified: Tue, 31 Jan 2023 21:59:41 GMT  
		Size: 211.2 MB (211241279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:67e9d04d3f796071778d301b6371cf89940a079e5db203afc969f830500303b8
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
$ docker pull neo4j@sha256:bf1d85b1081fd556288f0c204756b4db616740b5c4e88badcf1d443ca4d298ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da0dd68954d57ef80e0675d9a718b3246fb314e948876f4fef7943b654cb1cf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 21:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Jan 2023 21:57:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Tue, 31 Jan 2023 21:57:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 31 Jan 2023 21:57:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Tue, 31 Jan 2023 21:57:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:57:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:57:50 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Jan 2023 21:57:50 GMT
VOLUME [/data /logs]
# Tue, 31 Jan 2023 21:57:50 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Jan 2023 21:57:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 21:57:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a5c4e04f9bcf426624cdddd72be1ee3b881e3343b3b4fdba019406e3e19c4`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b40a34bc69773588a218a7f59e57a44423c30b870271af697637e0b998a823`  
		Last Modified: Tue, 31 Jan 2023 21:59:10 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7e2b8dcc69dc7857585c0a42bb279013e506142b19e3dcb30ca055674272b`  
		Last Modified: Tue, 31 Jan 2023 21:59:15 GMT  
		Size: 114.6 MB (114578996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
