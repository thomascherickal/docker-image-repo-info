<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.3`](#neo4j43)
-	[`neo4j:4.3-community`](#neo4j43-community)
-	[`neo4j:4.3-enterprise`](#neo4j43-enterprise)
-	[`neo4j:4.3.22`](#neo4j4322)
-	[`neo4j:4.3.22-community`](#neo4j4322-community)
-	[`neo4j:4.3.22-enterprise`](#neo4j4322-enterprise)
-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.15`](#neo4j4415)
-	[`neo4j:4.4.15-community`](#neo4j4415-community)
-	[`neo4j:4.4.15-enterprise`](#neo4j4415-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5.2`](#neo4j52)
-	[`neo4j:5.2-enterprise`](#neo4j52-enterprise)
-	[`neo4j:5.2.0`](#neo4j520)
-	[`neo4j:5.2.0-community`](#neo4j520-community)
-	[`neo4j:5.2.0-enterprise`](#neo4j520-enterprise)
-	[`neo4j:5.3`](#neo4j53)
-	[`neo4j:5.3-enterprise`](#neo4j53-enterprise)
-	[`neo4j:5.3.0`](#neo4j530)
-	[`neo4j:5.3.0-community`](#neo4j530-community)
-	[`neo4j:5.3.0-enterprise`](#neo4j530-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.3`

```console
$ docker pull neo4j@sha256:49c38830b21ead260e760baca13c7f5fd356f78d97328a1c4d05536fc06fa151
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3` - linux; amd64

```console
$ docker pull neo4j@sha256:6df4d837bfb66a630039052656840487eee6f55749067d6a9129a55b5cbbe6ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.4 MB (360413042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640452b0b406e99310fd56fe156c06e9951a62868c9d247a37c23ae6bf2964aa`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:25:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=cb4f97266d8057fbf15012235106a7241c66cc27475187eb6a6d3cdc9298e534 NEO4J_TARBALL=neo4j-community-4.3.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:25:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
# Fri, 09 Dec 2022 07:25:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:25:33 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Fri, 09 Dec 2022 07:25:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:25:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:25:50 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:25:50 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:25:50 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:25:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:25:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e6229301e0012ee3b652cbf147d3bcb943bf913b9add954300f93ccf645f2`  
		Last Modified: Fri, 09 Dec 2022 07:28:11 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c64261eaec0fc5ec43215073ade83712927be21e65882d351a747c9a47d7da5`  
		Last Modified: Fri, 09 Dec 2022 07:28:11 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c7859735d268f10e27b6763f8ce4ab55a7cb4f5183b46e9f34bda4982a2024`  
		Last Modified: Fri, 09 Dec 2022 07:28:18 GMT  
		Size: 130.5 MB (130534153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3-community`

```console
$ docker pull neo4j@sha256:49c38830b21ead260e760baca13c7f5fd356f78d97328a1c4d05536fc06fa151
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3-community` - linux; amd64

```console
$ docker pull neo4j@sha256:6df4d837bfb66a630039052656840487eee6f55749067d6a9129a55b5cbbe6ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.4 MB (360413042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640452b0b406e99310fd56fe156c06e9951a62868c9d247a37c23ae6bf2964aa`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:25:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=cb4f97266d8057fbf15012235106a7241c66cc27475187eb6a6d3cdc9298e534 NEO4J_TARBALL=neo4j-community-4.3.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:25:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
# Fri, 09 Dec 2022 07:25:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:25:33 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Fri, 09 Dec 2022 07:25:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:25:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:25:50 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:25:50 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:25:50 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:25:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:25:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e6229301e0012ee3b652cbf147d3bcb943bf913b9add954300f93ccf645f2`  
		Last Modified: Fri, 09 Dec 2022 07:28:11 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c64261eaec0fc5ec43215073ade83712927be21e65882d351a747c9a47d7da5`  
		Last Modified: Fri, 09 Dec 2022 07:28:11 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c7859735d268f10e27b6763f8ce4ab55a7cb4f5183b46e9f34bda4982a2024`  
		Last Modified: Fri, 09 Dec 2022 07:28:18 GMT  
		Size: 130.5 MB (130534153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3-enterprise`

```console
$ docker pull neo4j@sha256:4ac89f8e6b50d8887cac2a1d5ba042d1a1ef86a8ba12a08f5e3a0becf3461422
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:6b4cca0e895d06105b07220b0dda481cdfe21340853eafdaf87132d5934c7bac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.9 MB (390915975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b893debd7733b293cc180c662698c1b3ecc22135eae9121a05b3d189e9c74c40`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:25:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=eac8dab9669ad128ae65fabfac982087eaebb6b3bc011e688d33eb379ed92629 NEO4J_TARBALL=neo4j-enterprise-4.3.22-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:25:56 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.22-unix.tar.gz
# Fri, 09 Dec 2022 07:25:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:25:57 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Fri, 09 Dec 2022 07:26:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:26:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:26:15 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:26:15 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:26:15 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:26:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:26:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a997a54eb0bb616fff0b46cbb3992f8ca0fc7174ce65180a0928f205b57f05`  
		Last Modified: Fri, 09 Dec 2022 07:28:30 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef73c133b4a14754fc5798ec5ee14a0608ab46d76932939b66e8f7a4d90851ff`  
		Last Modified: Fri, 09 Dec 2022 07:28:31 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd70c588ffbb05aeaf2e7e238b15aa55d78dd71b07da2167e026edf33634d06`  
		Last Modified: Fri, 09 Dec 2022 07:28:37 GMT  
		Size: 161.0 MB (161037083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.22`

```console
$ docker pull neo4j@sha256:49c38830b21ead260e760baca13c7f5fd356f78d97328a1c4d05536fc06fa151
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.22` - linux; amd64

```console
$ docker pull neo4j@sha256:6df4d837bfb66a630039052656840487eee6f55749067d6a9129a55b5cbbe6ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.4 MB (360413042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640452b0b406e99310fd56fe156c06e9951a62868c9d247a37c23ae6bf2964aa`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:25:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=cb4f97266d8057fbf15012235106a7241c66cc27475187eb6a6d3cdc9298e534 NEO4J_TARBALL=neo4j-community-4.3.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:25:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
# Fri, 09 Dec 2022 07:25:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:25:33 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Fri, 09 Dec 2022 07:25:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:25:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:25:50 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:25:50 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:25:50 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:25:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:25:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e6229301e0012ee3b652cbf147d3bcb943bf913b9add954300f93ccf645f2`  
		Last Modified: Fri, 09 Dec 2022 07:28:11 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c64261eaec0fc5ec43215073ade83712927be21e65882d351a747c9a47d7da5`  
		Last Modified: Fri, 09 Dec 2022 07:28:11 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c7859735d268f10e27b6763f8ce4ab55a7cb4f5183b46e9f34bda4982a2024`  
		Last Modified: Fri, 09 Dec 2022 07:28:18 GMT  
		Size: 130.5 MB (130534153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.22-community`

```console
$ docker pull neo4j@sha256:49c38830b21ead260e760baca13c7f5fd356f78d97328a1c4d05536fc06fa151
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.22-community` - linux; amd64

```console
$ docker pull neo4j@sha256:6df4d837bfb66a630039052656840487eee6f55749067d6a9129a55b5cbbe6ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.4 MB (360413042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640452b0b406e99310fd56fe156c06e9951a62868c9d247a37c23ae6bf2964aa`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:25:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=cb4f97266d8057fbf15012235106a7241c66cc27475187eb6a6d3cdc9298e534 NEO4J_TARBALL=neo4j-community-4.3.22-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:25:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
# Fri, 09 Dec 2022 07:25:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:25:33 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Fri, 09 Dec 2022 07:25:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:25:50 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:25:50 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:25:50 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:25:50 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:25:50 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:25:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e6229301e0012ee3b652cbf147d3bcb943bf913b9add954300f93ccf645f2`  
		Last Modified: Fri, 09 Dec 2022 07:28:11 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c64261eaec0fc5ec43215073ade83712927be21e65882d351a747c9a47d7da5`  
		Last Modified: Fri, 09 Dec 2022 07:28:11 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c7859735d268f10e27b6763f8ce4ab55a7cb4f5183b46e9f34bda4982a2024`  
		Last Modified: Fri, 09 Dec 2022 07:28:18 GMT  
		Size: 130.5 MB (130534153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.22-enterprise`

```console
$ docker pull neo4j@sha256:4ac89f8e6b50d8887cac2a1d5ba042d1a1ef86a8ba12a08f5e3a0becf3461422
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.22-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:6b4cca0e895d06105b07220b0dda481cdfe21340853eafdaf87132d5934c7bac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.9 MB (390915975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b893debd7733b293cc180c662698c1b3ecc22135eae9121a05b3d189e9c74c40`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:25:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=eac8dab9669ad128ae65fabfac982087eaebb6b3bc011e688d33eb379ed92629 NEO4J_TARBALL=neo4j-enterprise-4.3.22-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:25:56 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.22-unix.tar.gz
# Fri, 09 Dec 2022 07:25:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.22-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:25:57 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Fri, 09 Dec 2022 07:26:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.22-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:26:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:26:15 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:26:15 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:26:15 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:26:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:26:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a997a54eb0bb616fff0b46cbb3992f8ca0fc7174ce65180a0928f205b57f05`  
		Last Modified: Fri, 09 Dec 2022 07:28:30 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef73c133b4a14754fc5798ec5ee14a0608ab46d76932939b66e8f7a4d90851ff`  
		Last Modified: Fri, 09 Dec 2022 07:28:31 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd70c588ffbb05aeaf2e7e238b15aa55d78dd71b07da2167e026edf33634d06`  
		Last Modified: Fri, 09 Dec 2022 07:28:37 GMT  
		Size: 161.0 MB (161037083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:cf34f47c1f4fc0c4961ac083c33efd2398ae7c1e54a07c034e51af58d0bfe633
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:ec83105c04a8ec59613d91f19ce726c938a30a20c22154f0469a3de08e68360c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.3 MB (365298707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecb7d227f6c2da9bc8af0eca928f8fe971e5f65197c36f3107b3bf5ac43c7b1f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:24:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=310527e15a88fc6c874148e1807b9dbdf3c094c30bb27e7bba08655f1ea06352 NEO4J_TARBALL=neo4j-community-4.4.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:24:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 07:24:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:24:48 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 07:24:59 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:25:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:25:00 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:25:00 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:25:00 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:25:00 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:25:00 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529ea15b0de45b69ffe4e69cc9a6b079dca42510c27711506fa2598644057cdc`  
		Last Modified: Fri, 09 Dec 2022 07:27:33 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eecaa211c550c56c156a0afe7b1f62988fa1f553d6a970d5d8928cde350d68`  
		Last Modified: Fri, 09 Dec 2022 07:27:33 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab04657f3861b05f48379c91faa0184e9f161b8b7173b081709908f3c86c391d`  
		Last Modified: Fri, 09 Dec 2022 07:27:41 GMT  
		Size: 135.4 MB (135419272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0b8463a7237f648a135381fe814b747fe90beb9b9f159190ccef082b54bc90ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.6 MB (360552059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4251b853f2a32a447e7657725de68a4c57b42c13309b55cb974ae4e3ebb00003`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:04:05 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:05:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=310527e15a88fc6c874148e1807b9dbdf3c094c30bb27e7bba08655f1ea06352 NEO4J_TARBALL=neo4j-community-4.4.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:05:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 06:05:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:05:02 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 06:05:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:05:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:05:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:05:12 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:05:12 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:05:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:05:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44bbb0380eb6b5cd1051003f5ce31baf496a9113c5e9927f76bcf714c433145`  
		Last Modified: Fri, 09 Dec 2022 05:18:38 GMT  
		Size: 195.2 MB (195203372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddf1b63ee1021fb4d42c559adb38c1d219199899fd8bcf7038761056f945da9`  
		Last Modified: Fri, 09 Dec 2022 06:06:36 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7908f81ea6f9cbbe67af97908251bbe3fcedc00404f51aea9877d58fd2bc203`  
		Last Modified: Fri, 09 Dec 2022 06:06:36 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985e7402c856a98be43526738a98d3219f5597ae049f7b7ef521bec802b01430`  
		Last Modified: Fri, 09 Dec 2022 06:06:42 GMT  
		Size: 135.3 MB (135276309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:cf34f47c1f4fc0c4961ac083c33efd2398ae7c1e54a07c034e51af58d0bfe633
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:ec83105c04a8ec59613d91f19ce726c938a30a20c22154f0469a3de08e68360c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.3 MB (365298707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecb7d227f6c2da9bc8af0eca928f8fe971e5f65197c36f3107b3bf5ac43c7b1f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:24:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=310527e15a88fc6c874148e1807b9dbdf3c094c30bb27e7bba08655f1ea06352 NEO4J_TARBALL=neo4j-community-4.4.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:24:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 07:24:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:24:48 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 07:24:59 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:25:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:25:00 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:25:00 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:25:00 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:25:00 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:25:00 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529ea15b0de45b69ffe4e69cc9a6b079dca42510c27711506fa2598644057cdc`  
		Last Modified: Fri, 09 Dec 2022 07:27:33 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eecaa211c550c56c156a0afe7b1f62988fa1f553d6a970d5d8928cde350d68`  
		Last Modified: Fri, 09 Dec 2022 07:27:33 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab04657f3861b05f48379c91faa0184e9f161b8b7173b081709908f3c86c391d`  
		Last Modified: Fri, 09 Dec 2022 07:27:41 GMT  
		Size: 135.4 MB (135419272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0b8463a7237f648a135381fe814b747fe90beb9b9f159190ccef082b54bc90ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.6 MB (360552059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4251b853f2a32a447e7657725de68a4c57b42c13309b55cb974ae4e3ebb00003`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:04:05 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:05:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=310527e15a88fc6c874148e1807b9dbdf3c094c30bb27e7bba08655f1ea06352 NEO4J_TARBALL=neo4j-community-4.4.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:05:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 06:05:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:05:02 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 06:05:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:05:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:05:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:05:12 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:05:12 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:05:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:05:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44bbb0380eb6b5cd1051003f5ce31baf496a9113c5e9927f76bcf714c433145`  
		Last Modified: Fri, 09 Dec 2022 05:18:38 GMT  
		Size: 195.2 MB (195203372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddf1b63ee1021fb4d42c559adb38c1d219199899fd8bcf7038761056f945da9`  
		Last Modified: Fri, 09 Dec 2022 06:06:36 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7908f81ea6f9cbbe67af97908251bbe3fcedc00404f51aea9877d58fd2bc203`  
		Last Modified: Fri, 09 Dec 2022 06:06:36 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985e7402c856a98be43526738a98d3219f5597ae049f7b7ef521bec802b01430`  
		Last Modified: Fri, 09 Dec 2022 06:06:42 GMT  
		Size: 135.3 MB (135276309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:9f237e63d35437bb014f6ecf74fed250198703349c11b2425fe7a66e1e5feeef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:3707f4e88c9a2823103f2b7ff354ace72cead3642f0d68570de08f69d934bfed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.5 MB (460485952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5201d89781d0443544b19b097c43024364e45580ba1d3522daf87a840e417cc4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:25:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=54531e7d1a7c381138fa527e1f5f22482d1687c04f237532b24fe42a1ef57491 NEO4J_TARBALL=neo4j-enterprise-4.4.15-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:25:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 07:25:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:25:05 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 07:25:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:25:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:25:27 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:25:27 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:25:27 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:25:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:25:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae855d560a037d18ca46fb8627cc3a1d74f4a5a610b6be529d129fa1c45a1bf5`  
		Last Modified: Fri, 09 Dec 2022 07:27:52 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e930b59a9f7f5db01fc5f6fb0d18664f68bb6cc9611bb49079b301dbf8cfb2db`  
		Last Modified: Fri, 09 Dec 2022 07:27:52 GMT  
		Size: 8.2 KB (8168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f640a4a910f1f436b560b12e79f33c9d27f4dc87d04b395500f317432f6652`  
		Last Modified: Fri, 09 Dec 2022 07:28:03 GMT  
		Size: 230.6 MB (230606518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fe035722b31508838c2e45343c6f202bb38cdfb780eff5c738653ca1b075c1a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.7 MB (455740012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbfff103274fe27f4f165a6823c2081bfaae5d2e6d802784b4fd90e1098e7de`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:04:05 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:05:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=54531e7d1a7c381138fa527e1f5f22482d1687c04f237532b24fe42a1ef57491 NEO4J_TARBALL=neo4j-enterprise-4.4.15-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:05:15 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 06:05:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:05:16 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 06:05:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:05:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:05:29 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:05:30 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:05:30 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:05:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:05:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44bbb0380eb6b5cd1051003f5ce31baf496a9113c5e9927f76bcf714c433145`  
		Last Modified: Fri, 09 Dec 2022 05:18:38 GMT  
		Size: 195.2 MB (195203372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437386a1c9ab0c608339d48a631ea93729e9ea22f147be4c6a8be740ce4a3584`  
		Last Modified: Fri, 09 Dec 2022 06:06:56 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e9611a7805dd1c1f6fd7295bafa8a7c41966fa210925efdf7be27820ccef3a`  
		Last Modified: Fri, 09 Dec 2022 06:06:56 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931de49b35611b3761e9e6485b5454e8e8743f2696cdbfb2574519c638441201`  
		Last Modified: Fri, 09 Dec 2022 06:07:05 GMT  
		Size: 230.5 MB (230464261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.15`

```console
$ docker pull neo4j@sha256:cf34f47c1f4fc0c4961ac083c33efd2398ae7c1e54a07c034e51af58d0bfe633
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.15` - linux; amd64

```console
$ docker pull neo4j@sha256:ec83105c04a8ec59613d91f19ce726c938a30a20c22154f0469a3de08e68360c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.3 MB (365298707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecb7d227f6c2da9bc8af0eca928f8fe971e5f65197c36f3107b3bf5ac43c7b1f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:24:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=310527e15a88fc6c874148e1807b9dbdf3c094c30bb27e7bba08655f1ea06352 NEO4J_TARBALL=neo4j-community-4.4.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:24:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 07:24:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:24:48 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 07:24:59 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:25:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:25:00 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:25:00 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:25:00 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:25:00 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:25:00 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529ea15b0de45b69ffe4e69cc9a6b079dca42510c27711506fa2598644057cdc`  
		Last Modified: Fri, 09 Dec 2022 07:27:33 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eecaa211c550c56c156a0afe7b1f62988fa1f553d6a970d5d8928cde350d68`  
		Last Modified: Fri, 09 Dec 2022 07:27:33 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab04657f3861b05f48379c91faa0184e9f161b8b7173b081709908f3c86c391d`  
		Last Modified: Fri, 09 Dec 2022 07:27:41 GMT  
		Size: 135.4 MB (135419272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.15` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0b8463a7237f648a135381fe814b747fe90beb9b9f159190ccef082b54bc90ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.6 MB (360552059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4251b853f2a32a447e7657725de68a4c57b42c13309b55cb974ae4e3ebb00003`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:04:05 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:05:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=310527e15a88fc6c874148e1807b9dbdf3c094c30bb27e7bba08655f1ea06352 NEO4J_TARBALL=neo4j-community-4.4.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:05:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 06:05:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:05:02 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 06:05:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:05:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:05:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:05:12 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:05:12 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:05:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:05:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44bbb0380eb6b5cd1051003f5ce31baf496a9113c5e9927f76bcf714c433145`  
		Last Modified: Fri, 09 Dec 2022 05:18:38 GMT  
		Size: 195.2 MB (195203372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddf1b63ee1021fb4d42c559adb38c1d219199899fd8bcf7038761056f945da9`  
		Last Modified: Fri, 09 Dec 2022 06:06:36 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7908f81ea6f9cbbe67af97908251bbe3fcedc00404f51aea9877d58fd2bc203`  
		Last Modified: Fri, 09 Dec 2022 06:06:36 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985e7402c856a98be43526738a98d3219f5597ae049f7b7ef521bec802b01430`  
		Last Modified: Fri, 09 Dec 2022 06:06:42 GMT  
		Size: 135.3 MB (135276309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.15-community`

```console
$ docker pull neo4j@sha256:cf34f47c1f4fc0c4961ac083c33efd2398ae7c1e54a07c034e51af58d0bfe633
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.15-community` - linux; amd64

```console
$ docker pull neo4j@sha256:ec83105c04a8ec59613d91f19ce726c938a30a20c22154f0469a3de08e68360c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.3 MB (365298707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecb7d227f6c2da9bc8af0eca928f8fe971e5f65197c36f3107b3bf5ac43c7b1f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:24:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=310527e15a88fc6c874148e1807b9dbdf3c094c30bb27e7bba08655f1ea06352 NEO4J_TARBALL=neo4j-community-4.4.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:24:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 07:24:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:24:48 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 07:24:59 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:25:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:25:00 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:25:00 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:25:00 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:25:00 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:25:00 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529ea15b0de45b69ffe4e69cc9a6b079dca42510c27711506fa2598644057cdc`  
		Last Modified: Fri, 09 Dec 2022 07:27:33 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eecaa211c550c56c156a0afe7b1f62988fa1f553d6a970d5d8928cde350d68`  
		Last Modified: Fri, 09 Dec 2022 07:27:33 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab04657f3861b05f48379c91faa0184e9f161b8b7173b081709908f3c86c391d`  
		Last Modified: Fri, 09 Dec 2022 07:27:41 GMT  
		Size: 135.4 MB (135419272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.15-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0b8463a7237f648a135381fe814b747fe90beb9b9f159190ccef082b54bc90ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.6 MB (360552059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4251b853f2a32a447e7657725de68a4c57b42c13309b55cb974ae4e3ebb00003`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:04:05 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:05:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=310527e15a88fc6c874148e1807b9dbdf3c094c30bb27e7bba08655f1ea06352 NEO4J_TARBALL=neo4j-community-4.4.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:05:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 06:05:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:05:02 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 06:05:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:05:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:05:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:05:12 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:05:12 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:05:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:05:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44bbb0380eb6b5cd1051003f5ce31baf496a9113c5e9927f76bcf714c433145`  
		Last Modified: Fri, 09 Dec 2022 05:18:38 GMT  
		Size: 195.2 MB (195203372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddf1b63ee1021fb4d42c559adb38c1d219199899fd8bcf7038761056f945da9`  
		Last Modified: Fri, 09 Dec 2022 06:06:36 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7908f81ea6f9cbbe67af97908251bbe3fcedc00404f51aea9877d58fd2bc203`  
		Last Modified: Fri, 09 Dec 2022 06:06:36 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985e7402c856a98be43526738a98d3219f5597ae049f7b7ef521bec802b01430`  
		Last Modified: Fri, 09 Dec 2022 06:06:42 GMT  
		Size: 135.3 MB (135276309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.15-enterprise`

```console
$ docker pull neo4j@sha256:9f237e63d35437bb014f6ecf74fed250198703349c11b2425fe7a66e1e5feeef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.15-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:3707f4e88c9a2823103f2b7ff354ace72cead3642f0d68570de08f69d934bfed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.5 MB (460485952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5201d89781d0443544b19b097c43024364e45580ba1d3522daf87a840e417cc4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:25:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=54531e7d1a7c381138fa527e1f5f22482d1687c04f237532b24fe42a1ef57491 NEO4J_TARBALL=neo4j-enterprise-4.4.15-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:25:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 07:25:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:25:05 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 07:25:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:25:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:25:27 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:25:27 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:25:27 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:25:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:25:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae855d560a037d18ca46fb8627cc3a1d74f4a5a610b6be529d129fa1c45a1bf5`  
		Last Modified: Fri, 09 Dec 2022 07:27:52 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e930b59a9f7f5db01fc5f6fb0d18664f68bb6cc9611bb49079b301dbf8cfb2db`  
		Last Modified: Fri, 09 Dec 2022 07:27:52 GMT  
		Size: 8.2 KB (8168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f640a4a910f1f436b560b12e79f33c9d27f4dc87d04b395500f317432f6652`  
		Last Modified: Fri, 09 Dec 2022 07:28:03 GMT  
		Size: 230.6 MB (230606518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.15-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fe035722b31508838c2e45343c6f202bb38cdfb780eff5c738653ca1b075c1a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.7 MB (455740012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbfff103274fe27f4f165a6823c2081bfaae5d2e6d802784b4fd90e1098e7de`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:04:05 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:05:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=54531e7d1a7c381138fa527e1f5f22482d1687c04f237532b24fe42a1ef57491 NEO4J_TARBALL=neo4j-enterprise-4.4.15-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:05:15 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
# Fri, 09 Dec 2022 06:05:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:05:16 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Fri, 09 Dec 2022 06:05:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:05:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:05:29 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:05:30 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:05:30 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:05:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:05:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44bbb0380eb6b5cd1051003f5ce31baf496a9113c5e9927f76bcf714c433145`  
		Last Modified: Fri, 09 Dec 2022 05:18:38 GMT  
		Size: 195.2 MB (195203372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437386a1c9ab0c608339d48a631ea93729e9ea22f147be4c6a8be740ce4a3584`  
		Last Modified: Fri, 09 Dec 2022 06:06:56 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e9611a7805dd1c1f6fd7295bafa8a7c41966fa210925efdf7be27820ccef3a`  
		Last Modified: Fri, 09 Dec 2022 06:06:56 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931de49b35611b3761e9e6485b5454e8e8743f2696cdbfb2574519c638441201`  
		Last Modified: Fri, 09 Dec 2022 06:07:05 GMT  
		Size: 230.5 MB (230464261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:adc0af7d5f9d2e219bb30a6783db29cb67ef60de6a3e5e6fd1e9de1240958c74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:382e22aa9bad8aa949478b717f651daf822aa6b648add5d04d3958ca5526cc3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338464632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f56e3bbddcfdfb7081d6d01a7b81aca5aa9b0385170d0e924713ce38c9d729`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:20 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:36 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:36 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:36 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520f74d879542f551aea3add57a17ce2e8868037a959b159a527f3c057e6ba35`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc23b03f1cd449c5ded745f780bb5231d2268d83d835c2f6f900a1b3b8c090f`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7810df2ef0fa3530dbf691cb48f6bb4af959ed05d7ff2edc6110eb16f0ab3`  
		Last Modified: Fri, 16 Dec 2022 00:27:48 GMT  
		Size: 114.6 MB (114608318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:58bce60b97dd2dd98fa89dcdfdd69c719357a558ccd8681e653438995e0350a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335754395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c3c3bead319235f58f3ee73115fc52efdcece681b9ad2702e4a7eda54708f3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:45:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:45:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:45:45 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:45:45 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:45:45 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:45:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:45:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5571ed58cae932e57ef3bd2ca64315900f8585ee787f92c938c6c7b0b305bd9`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac3bb26b2bf1c39c5fd6c1f881cc86ce31225b6499409c19df707d9a3ae642`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 8.3 KB (8336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636e32d56069fc06e62c2b94da87c5034e3b2511f1ae4c02f50a820c3eff831`  
		Last Modified: Fri, 16 Dec 2022 00:46:43 GMT  
		Size: 114.5 MB (114466647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:adc0af7d5f9d2e219bb30a6783db29cb67ef60de6a3e5e6fd1e9de1240958c74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:382e22aa9bad8aa949478b717f651daf822aa6b648add5d04d3958ca5526cc3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338464632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f56e3bbddcfdfb7081d6d01a7b81aca5aa9b0385170d0e924713ce38c9d729`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:20 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:36 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:36 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:36 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520f74d879542f551aea3add57a17ce2e8868037a959b159a527f3c057e6ba35`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc23b03f1cd449c5ded745f780bb5231d2268d83d835c2f6f900a1b3b8c090f`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7810df2ef0fa3530dbf691cb48f6bb4af959ed05d7ff2edc6110eb16f0ab3`  
		Last Modified: Fri, 16 Dec 2022 00:27:48 GMT  
		Size: 114.6 MB (114608318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:58bce60b97dd2dd98fa89dcdfdd69c719357a558ccd8681e653438995e0350a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335754395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c3c3bead319235f58f3ee73115fc52efdcece681b9ad2702e4a7eda54708f3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:45:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:45:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:45:45 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:45:45 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:45:45 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:45:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:45:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5571ed58cae932e57ef3bd2ca64315900f8585ee787f92c938c6c7b0b305bd9`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac3bb26b2bf1c39c5fd6c1f881cc86ce31225b6499409c19df707d9a3ae642`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 8.3 KB (8336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636e32d56069fc06e62c2b94da87c5034e3b2511f1ae4c02f50a820c3eff831`  
		Last Modified: Fri, 16 Dec 2022 00:46:43 GMT  
		Size: 114.5 MB (114466647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:04b8cd990d99213c0ecd33bdfe7d6a02dc70b30e0d528acaa6e08c568a576301
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:825e8777389ba387255b35450fe4e6b1cece4fda9e3a7e105a89388bcc425703
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.8 MB (434840782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69017d22c9243c4b34efe793c76aeb84be76061586d5fb7190a1fe55a94ee2e8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=078aaf4da22ed43eae8164d8446b52c6d3751476db9000b83daa163dcf634bc2 NEO4J_TARBALL=neo4j-enterprise-5.3.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:41 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:56 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:56 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b38a068aeedb8fd15e0c491e3af4f02d9c7106cf44852f06e2b8b96630b602`  
		Last Modified: Fri, 16 Dec 2022 00:28:06 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c24fc233dc320ea7e77f1eb753630372ddf39736498149046e19230681d97`  
		Last Modified: Fri, 16 Dec 2022 00:28:06 GMT  
		Size: 8.3 KB (8340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640f1c34930f5d845e12b017e132751127eb9533537398bdbf8f96b78e13fa90`  
		Last Modified: Fri, 16 Dec 2022 00:28:16 GMT  
		Size: 211.0 MB (210984470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e0194f242e44418de30c92e5d4aef46136bb475742685952e014554c15af4741
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.1 MB (432129984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e950e8c4d16184c757f0dd278f4351f2595cbcb5a4ccc3603a856c3b369639e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=078aaf4da22ed43eae8164d8446b52c6d3751476db9000b83daa163dcf634bc2 NEO4J_TARBALL=neo4j-enterprise-5.3.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:50 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:46:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:46:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:46:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:46:02 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:46:02 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:46:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:46:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8071d0dc16b80b644cd90edfe37ed45bf4230b603813370223b3c0dfd146be5`  
		Last Modified: Fri, 16 Dec 2022 00:47:02 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f17ac8c8583fd5ebe569eecdc368fe59dcb326161e158e20c9744bf3b71e513`  
		Last Modified: Fri, 16 Dec 2022 00:47:02 GMT  
		Size: 8.3 KB (8337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb01de83d5e887c3df94db71062b5e52951a123fa6eed0e22b708fcace816a4`  
		Last Modified: Fri, 16 Dec 2022 00:47:11 GMT  
		Size: 210.8 MB (210842235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.2`

```console
$ docker pull neo4j@sha256:7fc91f2c16cf52dadb125b320c9a547d2d7a9565b6b96e6639b374025d5f56c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.2` - linux; amd64

```console
$ docker pull neo4j@sha256:eb626e4b6c5956c190e864ec7ea2d2d3c1975cfbc3bef446130e8320c78f3049
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.8 MB (336774731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0393f054dc7f833476289501bc72fe55784c0b99914fc06f47260e236a2b46b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:24:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5fe22a0ff4cb11152b40b7ba0228f0e9af6a0b899006c413adf498314fd4b4f9 NEO4J_TARBALL=neo4j-community-5.2.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:24:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
# Fri, 09 Dec 2022 07:24:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:24:10 GMT
COPY multi:4c38b038fb207d3b3e018c6de201a35723320a0beef5d4b7a28a0fdf507334bd in /startup/ 
# Fri, 09 Dec 2022 07:24:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:24:22 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:24:22 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:24:23 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:24:23 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:24:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:24:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f953c3133dea11ad4119388794c08351dc59d033b148b1e21dd2540c8a259d2e`  
		Last Modified: Fri, 09 Dec 2022 07:26:43 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dc3a881de5b61d1b4a16220ccfbd608609af9e93c1e40aad4f5ff4213887d2`  
		Last Modified: Fri, 09 Dec 2022 07:26:43 GMT  
		Size: 8.2 KB (8165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39a521fdef67208223f07ba77bd966d4ecaaeb47832a52d59e091d0d8d405db`  
		Last Modified: Fri, 09 Dec 2022 07:26:50 GMT  
		Size: 112.9 MB (112918594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.2` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66a86b47786f9ece3d499c8112d71916663da0dd2229f0ccbfb4652f628d2168
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334063410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3924171754e99a92127c8f1fafed34be8fc1c81da16500dc3be5e1e37431dde`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:04:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5fe22a0ff4cb11152b40b7ba0228f0e9af6a0b899006c413adf498314fd4b4f9 NEO4J_TARBALL=neo4j-community-5.2.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:04:22 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
# Fri, 09 Dec 2022 06:04:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:04:23 GMT
COPY multi:4c38b038fb207d3b3e018c6de201a35723320a0beef5d4b7a28a0fdf507334bd in /startup/ 
# Fri, 09 Dec 2022 06:04:32 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:04:33 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:04:33 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:04:33 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:04:33 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:04:33 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:04:33 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4438ae9db4dc6039bc424a68c980ce15d81123c7217b787cc8f1555cd3ee9900`  
		Last Modified: Fri, 09 Dec 2022 06:05:52 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fadab086183024cd7601e4f6521c502a33abac72a24df0c10394c3ada6195c0`  
		Last Modified: Fri, 09 Dec 2022 06:05:52 GMT  
		Size: 8.2 KB (8163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391d1c9dfc0b8451b1db0a957e1c30e888bd8adb73a3d600c11e261847e08805`  
		Last Modified: Fri, 09 Dec 2022 06:05:57 GMT  
		Size: 112.8 MB (112775836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.2-enterprise`

```console
$ docker pull neo4j@sha256:83ca269245f040232943592286e7571bde40751e73290489d657cf32d7b29d0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.2-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:4ea502847e26beee2b5c47edc1581752e26dcafe47b1f1222e1d4933b99219a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.9 MB (432869753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9f83ddfd18e220f9c1df1c1bba91502212c1ab5fa9884c9f29e5a6276784cc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:24:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4a32f8a2800b00f690e4fcca670d268d40b8080c55796de1e6c92e39589026eb NEO4J_TARBALL=neo4j-enterprise-5.2.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:24:27 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
# Fri, 09 Dec 2022 07:24:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:24:28 GMT
COPY multi:4c38b038fb207d3b3e018c6de201a35723320a0beef5d4b7a28a0fdf507334bd in /startup/ 
# Fri, 09 Dec 2022 07:24:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:24:42 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:24:42 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:24:43 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:24:43 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:24:43 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:24:43 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e306e07ea3b58d1bb17833cb009a17b11f525413b51212b50f4cad9766a7446`  
		Last Modified: Fri, 09 Dec 2022 07:27:07 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c31c28f54c78bde862fd5399bfa609c84a57e321cc2dbf8b3ea478834b2a8bc`  
		Last Modified: Fri, 09 Dec 2022 07:27:07 GMT  
		Size: 8.2 KB (8166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb9711d68ddc6a87e7849d94542ba7ec5ed728aff66bd5e496d6c47e33c6a63`  
		Last Modified: Fri, 09 Dec 2022 07:27:21 GMT  
		Size: 209.0 MB (209013614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.2-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:18d6289eba4991525677f122ab0d3eec3b57e9e5c00452bb31ca72e799fdf808
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.2 MB (430158080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:485602c515591203d5f46c0966061d90e17c8aec5ed7a94fc61fd846060e30c0`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:04:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4a32f8a2800b00f690e4fcca670d268d40b8080c55796de1e6c92e39589026eb NEO4J_TARBALL=neo4j-enterprise-5.2.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:04:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
# Fri, 09 Dec 2022 06:04:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:04:38 GMT
COPY multi:4c38b038fb207d3b3e018c6de201a35723320a0beef5d4b7a28a0fdf507334bd in /startup/ 
# Fri, 09 Dec 2022 06:04:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:04:56 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:04:56 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:04:56 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:04:56 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:04:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:04:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d26ef527972959e82e9c8c5dadeeed2ce449840d705813c3bb65e26187c3d8`  
		Last Modified: Fri, 09 Dec 2022 06:06:15 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3098263ed95b81de5db6fdbde47099d8ee8603c6e4852db3a552ba58b91e66ee`  
		Last Modified: Fri, 09 Dec 2022 06:06:15 GMT  
		Size: 8.2 KB (8164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7080f7dc677d1ade020cb3417f0e9b6b7ac79456c207e0d41f69695ae2a9159a`  
		Last Modified: Fri, 09 Dec 2022 06:06:24 GMT  
		Size: 208.9 MB (208870505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.2.0`

```console
$ docker pull neo4j@sha256:7fc91f2c16cf52dadb125b320c9a547d2d7a9565b6b96e6639b374025d5f56c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.2.0` - linux; amd64

```console
$ docker pull neo4j@sha256:eb626e4b6c5956c190e864ec7ea2d2d3c1975cfbc3bef446130e8320c78f3049
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.8 MB (336774731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0393f054dc7f833476289501bc72fe55784c0b99914fc06f47260e236a2b46b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:24:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5fe22a0ff4cb11152b40b7ba0228f0e9af6a0b899006c413adf498314fd4b4f9 NEO4J_TARBALL=neo4j-community-5.2.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:24:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
# Fri, 09 Dec 2022 07:24:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:24:10 GMT
COPY multi:4c38b038fb207d3b3e018c6de201a35723320a0beef5d4b7a28a0fdf507334bd in /startup/ 
# Fri, 09 Dec 2022 07:24:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:24:22 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:24:22 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:24:23 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:24:23 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:24:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:24:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f953c3133dea11ad4119388794c08351dc59d033b148b1e21dd2540c8a259d2e`  
		Last Modified: Fri, 09 Dec 2022 07:26:43 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dc3a881de5b61d1b4a16220ccfbd608609af9e93c1e40aad4f5ff4213887d2`  
		Last Modified: Fri, 09 Dec 2022 07:26:43 GMT  
		Size: 8.2 KB (8165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39a521fdef67208223f07ba77bd966d4ecaaeb47832a52d59e091d0d8d405db`  
		Last Modified: Fri, 09 Dec 2022 07:26:50 GMT  
		Size: 112.9 MB (112918594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.2.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66a86b47786f9ece3d499c8112d71916663da0dd2229f0ccbfb4652f628d2168
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334063410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3924171754e99a92127c8f1fafed34be8fc1c81da16500dc3be5e1e37431dde`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:04:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5fe22a0ff4cb11152b40b7ba0228f0e9af6a0b899006c413adf498314fd4b4f9 NEO4J_TARBALL=neo4j-community-5.2.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:04:22 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
# Fri, 09 Dec 2022 06:04:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:04:23 GMT
COPY multi:4c38b038fb207d3b3e018c6de201a35723320a0beef5d4b7a28a0fdf507334bd in /startup/ 
# Fri, 09 Dec 2022 06:04:32 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:04:33 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:04:33 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:04:33 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:04:33 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:04:33 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:04:33 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4438ae9db4dc6039bc424a68c980ce15d81123c7217b787cc8f1555cd3ee9900`  
		Last Modified: Fri, 09 Dec 2022 06:05:52 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fadab086183024cd7601e4f6521c502a33abac72a24df0c10394c3ada6195c0`  
		Last Modified: Fri, 09 Dec 2022 06:05:52 GMT  
		Size: 8.2 KB (8163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391d1c9dfc0b8451b1db0a957e1c30e888bd8adb73a3d600c11e261847e08805`  
		Last Modified: Fri, 09 Dec 2022 06:05:57 GMT  
		Size: 112.8 MB (112775836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.2.0-community`

```console
$ docker pull neo4j@sha256:7fc91f2c16cf52dadb125b320c9a547d2d7a9565b6b96e6639b374025d5f56c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.2.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:eb626e4b6c5956c190e864ec7ea2d2d3c1975cfbc3bef446130e8320c78f3049
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.8 MB (336774731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0393f054dc7f833476289501bc72fe55784c0b99914fc06f47260e236a2b46b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:24:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5fe22a0ff4cb11152b40b7ba0228f0e9af6a0b899006c413adf498314fd4b4f9 NEO4J_TARBALL=neo4j-community-5.2.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:24:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
# Fri, 09 Dec 2022 07:24:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:24:10 GMT
COPY multi:4c38b038fb207d3b3e018c6de201a35723320a0beef5d4b7a28a0fdf507334bd in /startup/ 
# Fri, 09 Dec 2022 07:24:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:24:22 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:24:22 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:24:23 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:24:23 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:24:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:24:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f953c3133dea11ad4119388794c08351dc59d033b148b1e21dd2540c8a259d2e`  
		Last Modified: Fri, 09 Dec 2022 07:26:43 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dc3a881de5b61d1b4a16220ccfbd608609af9e93c1e40aad4f5ff4213887d2`  
		Last Modified: Fri, 09 Dec 2022 07:26:43 GMT  
		Size: 8.2 KB (8165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39a521fdef67208223f07ba77bd966d4ecaaeb47832a52d59e091d0d8d405db`  
		Last Modified: Fri, 09 Dec 2022 07:26:50 GMT  
		Size: 112.9 MB (112918594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.2.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66a86b47786f9ece3d499c8112d71916663da0dd2229f0ccbfb4652f628d2168
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334063410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3924171754e99a92127c8f1fafed34be8fc1c81da16500dc3be5e1e37431dde`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:04:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5fe22a0ff4cb11152b40b7ba0228f0e9af6a0b899006c413adf498314fd4b4f9 NEO4J_TARBALL=neo4j-community-5.2.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:04:22 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
# Fri, 09 Dec 2022 06:04:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:04:23 GMT
COPY multi:4c38b038fb207d3b3e018c6de201a35723320a0beef5d4b7a28a0fdf507334bd in /startup/ 
# Fri, 09 Dec 2022 06:04:32 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.2.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:04:33 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:04:33 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:04:33 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:04:33 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:04:33 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:04:33 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4438ae9db4dc6039bc424a68c980ce15d81123c7217b787cc8f1555cd3ee9900`  
		Last Modified: Fri, 09 Dec 2022 06:05:52 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fadab086183024cd7601e4f6521c502a33abac72a24df0c10394c3ada6195c0`  
		Last Modified: Fri, 09 Dec 2022 06:05:52 GMT  
		Size: 8.2 KB (8163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391d1c9dfc0b8451b1db0a957e1c30e888bd8adb73a3d600c11e261847e08805`  
		Last Modified: Fri, 09 Dec 2022 06:05:57 GMT  
		Size: 112.8 MB (112775836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.2.0-enterprise`

```console
$ docker pull neo4j@sha256:83ca269245f040232943592286e7571bde40751e73290489d657cf32d7b29d0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.2.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:4ea502847e26beee2b5c47edc1581752e26dcafe47b1f1222e1d4933b99219a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.9 MB (432869753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9f83ddfd18e220f9c1df1c1bba91502212c1ab5fa9884c9f29e5a6276784cc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 09 Dec 2022 07:24:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4a32f8a2800b00f690e4fcca670d268d40b8080c55796de1e6c92e39589026eb NEO4J_TARBALL=neo4j-enterprise-5.2.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 07:24:27 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
# Fri, 09 Dec 2022 07:24:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 07:24:28 GMT
COPY multi:4c38b038fb207d3b3e018c6de201a35723320a0beef5d4b7a28a0fdf507334bd in /startup/ 
# Fri, 09 Dec 2022 07:24:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:24:42 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:24:42 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 07:24:43 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 07:24:43 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 07:24:43 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 07:24:43 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e306e07ea3b58d1bb17833cb009a17b11f525413b51212b50f4cad9766a7446`  
		Last Modified: Fri, 09 Dec 2022 07:27:07 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c31c28f54c78bde862fd5399bfa609c84a57e321cc2dbf8b3ea478834b2a8bc`  
		Last Modified: Fri, 09 Dec 2022 07:27:07 GMT  
		Size: 8.2 KB (8166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb9711d68ddc6a87e7849d94542ba7ec5ed728aff66bd5e496d6c47e33c6a63`  
		Last Modified: Fri, 09 Dec 2022 07:27:21 GMT  
		Size: 209.0 MB (209013614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.2.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:18d6289eba4991525677f122ab0d3eec3b57e9e5c00452bb31ca72e799fdf808
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.2 MB (430158080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:485602c515591203d5f46c0966061d90e17c8aec5ed7a94fc61fd846060e30c0`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:04:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4a32f8a2800b00f690e4fcca670d268d40b8080c55796de1e6c92e39589026eb NEO4J_TARBALL=neo4j-enterprise-5.2.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 09 Dec 2022 06:04:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
# Fri, 09 Dec 2022 06:04:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 09 Dec 2022 06:04:38 GMT
COPY multi:4c38b038fb207d3b3e018c6de201a35723320a0beef5d4b7a28a0fdf507334bd in /startup/ 
# Fri, 09 Dec 2022 06:04:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.2.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:04:56 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:04:56 GMT
WORKDIR /var/lib/neo4j
# Fri, 09 Dec 2022 06:04:56 GMT
VOLUME [/data /logs]
# Fri, 09 Dec 2022 06:04:56 GMT
EXPOSE 7473 7474 7687
# Fri, 09 Dec 2022 06:04:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 06:04:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d26ef527972959e82e9c8c5dadeeed2ce449840d705813c3bb65e26187c3d8`  
		Last Modified: Fri, 09 Dec 2022 06:06:15 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3098263ed95b81de5db6fdbde47099d8ee8603c6e4852db3a552ba58b91e66ee`  
		Last Modified: Fri, 09 Dec 2022 06:06:15 GMT  
		Size: 8.2 KB (8164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7080f7dc677d1ade020cb3417f0e9b6b7ac79456c207e0d41f69695ae2a9159a`  
		Last Modified: Fri, 09 Dec 2022 06:06:24 GMT  
		Size: 208.9 MB (208870505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.3`

```console
$ docker pull neo4j@sha256:adc0af7d5f9d2e219bb30a6783db29cb67ef60de6a3e5e6fd1e9de1240958c74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.3` - linux; amd64

```console
$ docker pull neo4j@sha256:382e22aa9bad8aa949478b717f651daf822aa6b648add5d04d3958ca5526cc3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338464632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f56e3bbddcfdfb7081d6d01a7b81aca5aa9b0385170d0e924713ce38c9d729`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:20 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:36 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:36 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:36 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520f74d879542f551aea3add57a17ce2e8868037a959b159a527f3c057e6ba35`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc23b03f1cd449c5ded745f780bb5231d2268d83d835c2f6f900a1b3b8c090f`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7810df2ef0fa3530dbf691cb48f6bb4af959ed05d7ff2edc6110eb16f0ab3`  
		Last Modified: Fri, 16 Dec 2022 00:27:48 GMT  
		Size: 114.6 MB (114608318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.3` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:58bce60b97dd2dd98fa89dcdfdd69c719357a558ccd8681e653438995e0350a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335754395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c3c3bead319235f58f3ee73115fc52efdcece681b9ad2702e4a7eda54708f3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:45:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:45:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:45:45 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:45:45 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:45:45 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:45:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:45:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5571ed58cae932e57ef3bd2ca64315900f8585ee787f92c938c6c7b0b305bd9`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac3bb26b2bf1c39c5fd6c1f881cc86ce31225b6499409c19df707d9a3ae642`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 8.3 KB (8336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636e32d56069fc06e62c2b94da87c5034e3b2511f1ae4c02f50a820c3eff831`  
		Last Modified: Fri, 16 Dec 2022 00:46:43 GMT  
		Size: 114.5 MB (114466647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.3-enterprise`

```console
$ docker pull neo4j@sha256:04b8cd990d99213c0ecd33bdfe7d6a02dc70b30e0d528acaa6e08c568a576301
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.3-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:825e8777389ba387255b35450fe4e6b1cece4fda9e3a7e105a89388bcc425703
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.8 MB (434840782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69017d22c9243c4b34efe793c76aeb84be76061586d5fb7190a1fe55a94ee2e8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=078aaf4da22ed43eae8164d8446b52c6d3751476db9000b83daa163dcf634bc2 NEO4J_TARBALL=neo4j-enterprise-5.3.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:41 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:56 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:56 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b38a068aeedb8fd15e0c491e3af4f02d9c7106cf44852f06e2b8b96630b602`  
		Last Modified: Fri, 16 Dec 2022 00:28:06 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c24fc233dc320ea7e77f1eb753630372ddf39736498149046e19230681d97`  
		Last Modified: Fri, 16 Dec 2022 00:28:06 GMT  
		Size: 8.3 KB (8340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640f1c34930f5d845e12b017e132751127eb9533537398bdbf8f96b78e13fa90`  
		Last Modified: Fri, 16 Dec 2022 00:28:16 GMT  
		Size: 211.0 MB (210984470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.3-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e0194f242e44418de30c92e5d4aef46136bb475742685952e014554c15af4741
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.1 MB (432129984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e950e8c4d16184c757f0dd278f4351f2595cbcb5a4ccc3603a856c3b369639e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=078aaf4da22ed43eae8164d8446b52c6d3751476db9000b83daa163dcf634bc2 NEO4J_TARBALL=neo4j-enterprise-5.3.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:50 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:46:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:46:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:46:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:46:02 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:46:02 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:46:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:46:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8071d0dc16b80b644cd90edfe37ed45bf4230b603813370223b3c0dfd146be5`  
		Last Modified: Fri, 16 Dec 2022 00:47:02 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f17ac8c8583fd5ebe569eecdc368fe59dcb326161e158e20c9744bf3b71e513`  
		Last Modified: Fri, 16 Dec 2022 00:47:02 GMT  
		Size: 8.3 KB (8337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb01de83d5e887c3df94db71062b5e52951a123fa6eed0e22b708fcace816a4`  
		Last Modified: Fri, 16 Dec 2022 00:47:11 GMT  
		Size: 210.8 MB (210842235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.3.0`

```console
$ docker pull neo4j@sha256:adc0af7d5f9d2e219bb30a6783db29cb67ef60de6a3e5e6fd1e9de1240958c74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.3.0` - linux; amd64

```console
$ docker pull neo4j@sha256:382e22aa9bad8aa949478b717f651daf822aa6b648add5d04d3958ca5526cc3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338464632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f56e3bbddcfdfb7081d6d01a7b81aca5aa9b0385170d0e924713ce38c9d729`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:20 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:36 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:36 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:36 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520f74d879542f551aea3add57a17ce2e8868037a959b159a527f3c057e6ba35`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc23b03f1cd449c5ded745f780bb5231d2268d83d835c2f6f900a1b3b8c090f`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7810df2ef0fa3530dbf691cb48f6bb4af959ed05d7ff2edc6110eb16f0ab3`  
		Last Modified: Fri, 16 Dec 2022 00:27:48 GMT  
		Size: 114.6 MB (114608318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.3.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:58bce60b97dd2dd98fa89dcdfdd69c719357a558ccd8681e653438995e0350a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335754395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c3c3bead319235f58f3ee73115fc52efdcece681b9ad2702e4a7eda54708f3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:45:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:45:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:45:45 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:45:45 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:45:45 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:45:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:45:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5571ed58cae932e57ef3bd2ca64315900f8585ee787f92c938c6c7b0b305bd9`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac3bb26b2bf1c39c5fd6c1f881cc86ce31225b6499409c19df707d9a3ae642`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 8.3 KB (8336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636e32d56069fc06e62c2b94da87c5034e3b2511f1ae4c02f50a820c3eff831`  
		Last Modified: Fri, 16 Dec 2022 00:46:43 GMT  
		Size: 114.5 MB (114466647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.3.0-community`

```console
$ docker pull neo4j@sha256:adc0af7d5f9d2e219bb30a6783db29cb67ef60de6a3e5e6fd1e9de1240958c74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.3.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:382e22aa9bad8aa949478b717f651daf822aa6b648add5d04d3958ca5526cc3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338464632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f56e3bbddcfdfb7081d6d01a7b81aca5aa9b0385170d0e924713ce38c9d729`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:20 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:36 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:36 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:36 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520f74d879542f551aea3add57a17ce2e8868037a959b159a527f3c057e6ba35`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc23b03f1cd449c5ded745f780bb5231d2268d83d835c2f6f900a1b3b8c090f`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7810df2ef0fa3530dbf691cb48f6bb4af959ed05d7ff2edc6110eb16f0ab3`  
		Last Modified: Fri, 16 Dec 2022 00:27:48 GMT  
		Size: 114.6 MB (114608318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.3.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:58bce60b97dd2dd98fa89dcdfdd69c719357a558ccd8681e653438995e0350a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335754395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c3c3bead319235f58f3ee73115fc52efdcece681b9ad2702e4a7eda54708f3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:45:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:45:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:45:45 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:45:45 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:45:45 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:45:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:45:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5571ed58cae932e57ef3bd2ca64315900f8585ee787f92c938c6c7b0b305bd9`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac3bb26b2bf1c39c5fd6c1f881cc86ce31225b6499409c19df707d9a3ae642`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 8.3 KB (8336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636e32d56069fc06e62c2b94da87c5034e3b2511f1ae4c02f50a820c3eff831`  
		Last Modified: Fri, 16 Dec 2022 00:46:43 GMT  
		Size: 114.5 MB (114466647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.3.0-enterprise`

```console
$ docker pull neo4j@sha256:04b8cd990d99213c0ecd33bdfe7d6a02dc70b30e0d528acaa6e08c568a576301
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.3.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:825e8777389ba387255b35450fe4e6b1cece4fda9e3a7e105a89388bcc425703
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.8 MB (434840782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69017d22c9243c4b34efe793c76aeb84be76061586d5fb7190a1fe55a94ee2e8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=078aaf4da22ed43eae8164d8446b52c6d3751476db9000b83daa163dcf634bc2 NEO4J_TARBALL=neo4j-enterprise-5.3.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:41 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:56 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:56 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b38a068aeedb8fd15e0c491e3af4f02d9c7106cf44852f06e2b8b96630b602`  
		Last Modified: Fri, 16 Dec 2022 00:28:06 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c24fc233dc320ea7e77f1eb753630372ddf39736498149046e19230681d97`  
		Last Modified: Fri, 16 Dec 2022 00:28:06 GMT  
		Size: 8.3 KB (8340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640f1c34930f5d845e12b017e132751127eb9533537398bdbf8f96b78e13fa90`  
		Last Modified: Fri, 16 Dec 2022 00:28:16 GMT  
		Size: 211.0 MB (210984470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.3.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e0194f242e44418de30c92e5d4aef46136bb475742685952e014554c15af4741
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.1 MB (432129984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e950e8c4d16184c757f0dd278f4351f2595cbcb5a4ccc3603a856c3b369639e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=078aaf4da22ed43eae8164d8446b52c6d3751476db9000b83daa163dcf634bc2 NEO4J_TARBALL=neo4j-enterprise-5.3.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:50 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:46:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:46:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:46:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:46:02 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:46:02 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:46:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:46:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8071d0dc16b80b644cd90edfe37ed45bf4230b603813370223b3c0dfd146be5`  
		Last Modified: Fri, 16 Dec 2022 00:47:02 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f17ac8c8583fd5ebe569eecdc368fe59dcb326161e158e20c9744bf3b71e513`  
		Last Modified: Fri, 16 Dec 2022 00:47:02 GMT  
		Size: 8.3 KB (8337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb01de83d5e887c3df94db71062b5e52951a123fa6eed0e22b708fcace816a4`  
		Last Modified: Fri, 16 Dec 2022 00:47:11 GMT  
		Size: 210.8 MB (210842235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:adc0af7d5f9d2e219bb30a6783db29cb67ef60de6a3e5e6fd1e9de1240958c74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:382e22aa9bad8aa949478b717f651daf822aa6b648add5d04d3958ca5526cc3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338464632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f56e3bbddcfdfb7081d6d01a7b81aca5aa9b0385170d0e924713ce38c9d729`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:20 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:36 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:36 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:36 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520f74d879542f551aea3add57a17ce2e8868037a959b159a527f3c057e6ba35`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc23b03f1cd449c5ded745f780bb5231d2268d83d835c2f6f900a1b3b8c090f`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7810df2ef0fa3530dbf691cb48f6bb4af959ed05d7ff2edc6110eb16f0ab3`  
		Last Modified: Fri, 16 Dec 2022 00:27:48 GMT  
		Size: 114.6 MB (114608318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:58bce60b97dd2dd98fa89dcdfdd69c719357a558ccd8681e653438995e0350a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335754395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c3c3bead319235f58f3ee73115fc52efdcece681b9ad2702e4a7eda54708f3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:45:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:45:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:45:45 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:45:45 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:45:45 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:45:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:45:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5571ed58cae932e57ef3bd2ca64315900f8585ee787f92c938c6c7b0b305bd9`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac3bb26b2bf1c39c5fd6c1f881cc86ce31225b6499409c19df707d9a3ae642`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 8.3 KB (8336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636e32d56069fc06e62c2b94da87c5034e3b2511f1ae4c02f50a820c3eff831`  
		Last Modified: Fri, 16 Dec 2022 00:46:43 GMT  
		Size: 114.5 MB (114466647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:04b8cd990d99213c0ecd33bdfe7d6a02dc70b30e0d528acaa6e08c568a576301
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:825e8777389ba387255b35450fe4e6b1cece4fda9e3a7e105a89388bcc425703
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.8 MB (434840782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69017d22c9243c4b34efe793c76aeb84be76061586d5fb7190a1fe55a94ee2e8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=078aaf4da22ed43eae8164d8446b52c6d3751476db9000b83daa163dcf634bc2 NEO4J_TARBALL=neo4j-enterprise-5.3.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:41 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:56 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:56 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b38a068aeedb8fd15e0c491e3af4f02d9c7106cf44852f06e2b8b96630b602`  
		Last Modified: Fri, 16 Dec 2022 00:28:06 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74c24fc233dc320ea7e77f1eb753630372ddf39736498149046e19230681d97`  
		Last Modified: Fri, 16 Dec 2022 00:28:06 GMT  
		Size: 8.3 KB (8340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640f1c34930f5d845e12b017e132751127eb9533537398bdbf8f96b78e13fa90`  
		Last Modified: Fri, 16 Dec 2022 00:28:16 GMT  
		Size: 211.0 MB (210984470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e0194f242e44418de30c92e5d4aef46136bb475742685952e014554c15af4741
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.1 MB (432129984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e950e8c4d16184c757f0dd278f4351f2595cbcb5a4ccc3603a856c3b369639e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=078aaf4da22ed43eae8164d8446b52c6d3751476db9000b83daa163dcf634bc2 NEO4J_TARBALL=neo4j-enterprise-5.3.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:50 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:46:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:46:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:46:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:46:02 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:46:02 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:46:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:46:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8071d0dc16b80b644cd90edfe37ed45bf4230b603813370223b3c0dfd146be5`  
		Last Modified: Fri, 16 Dec 2022 00:47:02 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f17ac8c8583fd5ebe569eecdc368fe59dcb326161e158e20c9744bf3b71e513`  
		Last Modified: Fri, 16 Dec 2022 00:47:02 GMT  
		Size: 8.3 KB (8337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb01de83d5e887c3df94db71062b5e52951a123fa6eed0e22b708fcace816a4`  
		Last Modified: Fri, 16 Dec 2022 00:47:11 GMT  
		Size: 210.8 MB (210842235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:adc0af7d5f9d2e219bb30a6783db29cb67ef60de6a3e5e6fd1e9de1240958c74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:382e22aa9bad8aa949478b717f651daf822aa6b648add5d04d3958ca5526cc3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338464632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f56e3bbddcfdfb7081d6d01a7b81aca5aa9b0385170d0e924713ce38c9d729`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:26:20 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:26:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:26:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:26:36 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:26:36 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:26:36 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:26:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:26:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520f74d879542f551aea3add57a17ce2e8868037a959b159a527f3c057e6ba35`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc23b03f1cd449c5ded745f780bb5231d2268d83d835c2f6f900a1b3b8c090f`  
		Last Modified: Fri, 16 Dec 2022 00:27:41 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7810df2ef0fa3530dbf691cb48f6bb4af959ed05d7ff2edc6110eb16f0ab3`  
		Last Modified: Fri, 16 Dec 2022 00:27:48 GMT  
		Size: 114.6 MB (114608318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:58bce60b97dd2dd98fa89dcdfdd69c719357a558ccd8681e653438995e0350a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335754395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c3c3bead319235f58f3ee73115fc52efdcece681b9ad2702e4a7eda54708f3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 16 Dec 2022 00:45:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Fri, 16 Dec 2022 00:45:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 16 Dec 2022 00:45:35 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 16 Dec 2022 00:45:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Dec 2022 00:45:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 00:45:45 GMT
WORKDIR /var/lib/neo4j
# Fri, 16 Dec 2022 00:45:45 GMT
VOLUME [/data /logs]
# Fri, 16 Dec 2022 00:45:45 GMT
EXPOSE 7473 7474 7687
# Fri, 16 Dec 2022 00:45:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 16 Dec 2022 00:45:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5571ed58cae932e57ef3bd2ca64315900f8585ee787f92c938c6c7b0b305bd9`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac3bb26b2bf1c39c5fd6c1f881cc86ce31225b6499409c19df707d9a3ae642`  
		Last Modified: Fri, 16 Dec 2022 00:46:38 GMT  
		Size: 8.3 KB (8336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636e32d56069fc06e62c2b94da87c5034e3b2511f1ae4c02f50a820c3eff831`  
		Last Modified: Fri, 16 Dec 2022 00:46:43 GMT  
		Size: 114.5 MB (114466647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
