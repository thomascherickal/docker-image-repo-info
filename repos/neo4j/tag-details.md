<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.24`](#neo4j4424)
-	[`neo4j:4.4.24-community`](#neo4j4424-community)
-	[`neo4j:4.4.24-enterprise`](#neo4j4424-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-bullseye`](#neo4j5-bullseye)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-community-bullseye`](#neo4j5-community-bullseye)
-	[`neo4j:5-community-ubi8`](#neo4j5-community-ubi8)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5-enterprise-bullseye`](#neo4j5-enterprise-bullseye)
-	[`neo4j:5-enterprise-ubi8`](#neo4j5-enterprise-ubi8)
-	[`neo4j:5-ubi8`](#neo4j5-ubi8)
-	[`neo4j:5.11`](#neo4j511)
-	[`neo4j:5.11-bullseye`](#neo4j511-bullseye)
-	[`neo4j:5.11-community`](#neo4j511-community)
-	[`neo4j:5.11-community-bullseye`](#neo4j511-community-bullseye)
-	[`neo4j:5.11-community-ubi8`](#neo4j511-community-ubi8)
-	[`neo4j:5.11-enterprise`](#neo4j511-enterprise)
-	[`neo4j:5.11-enterprise-bullseye`](#neo4j511-enterprise-bullseye)
-	[`neo4j:5.11-enterprise-ubi8`](#neo4j511-enterprise-ubi8)
-	[`neo4j:5.11-ubi8`](#neo4j511-ubi8)
-	[`neo4j:5.11.0`](#neo4j5110)
-	[`neo4j:5.11.0-bullseye`](#neo4j5110-bullseye)
-	[`neo4j:5.11.0-community`](#neo4j5110-community)
-	[`neo4j:5.11.0-community-bullseye`](#neo4j5110-community-bullseye)
-	[`neo4j:5.11.0-community-ubi8`](#neo4j5110-community-ubi8)
-	[`neo4j:5.11.0-enterprise`](#neo4j5110-enterprise)
-	[`neo4j:5.11.0-enterprise-bullseye`](#neo4j5110-enterprise-bullseye)
-	[`neo4j:5.11.0-enterprise-ubi8`](#neo4j5110-enterprise-ubi8)
-	[`neo4j:5.11.0-ubi8`](#neo4j5110-ubi8)
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
$ docker pull neo4j@sha256:f68efda475375454c3aa09633dc3893c0984f72252491ed19eeb77753ce7f05a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:4e263576afd9694d54d411b3d9dbd1ad11a6627cae25a63ede20566b5813f5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.5 MB (298549984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0078ab4e9e4976ab06453f01b57d4975e5224528b6f5c2d414f871d5d1fa6fc6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:02:38 GMT
COPY dir:72d046f3e284b8eca8066a837ab8a68f91b4cf5355de7f6803a8ee9b7ce3d682 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2e76f3d237648392c9fb43b6a93fbd30cb00da617a30d13712b386a69565e43a NEO4J_TARBALL=neo4j-community-4.4.24-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 17:02:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:02:40 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 17:02:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:02:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:02:52 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:02:52 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:02:52 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:02:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:02:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209f416efba54d09e37495a54336ac55d40fc467f753f97e78f060748b4513e5`  
		Last Modified: Wed, 16 Aug 2023 17:06:20 GMT  
		Size: 144.8 MB (144831672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d90d22bb9c3af24549dfdb794895f7ec444e1e7a2cf4b718fbfec705875b3a`  
		Last Modified: Wed, 16 Aug 2023 17:06:08 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40677c38fb05c03c597e2429ed8cb36f7393d42b0413c0c486540dee91fd7df`  
		Last Modified: Wed, 16 Aug 2023 17:06:08 GMT  
		Size: 9.3 KB (9324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd78884f79a99c17e0892e14f04a3350f264673410de7f82dd8fa1c25f31010`  
		Last Modified: Wed, 16 Aug 2023 17:06:15 GMT  
		Size: 122.3 MB (122287452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b133c2a9b52e6272811aa4f44355dea41c204fb8eccd166fb36fbaab0688226e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.8 MB (293820152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e408e84f33921d1ce862ec3ceacdb33b9591c4856863f287b082c406d01d9d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:22:18 GMT
COPY dir:6acc55ac013a722a8db4af8f0ce8de9270cd9aeb372e6c734b449d15adcc5218 in /opt/java/openjdk 
# Wed, 16 Aug 2023 18:04:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2e76f3d237648392c9fb43b6a93fbd30cb00da617a30d13712b386a69565e43a NEO4J_TARBALL=neo4j-community-4.4.24-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 18:04:18 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 18:04:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 18:04:19 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 18:04:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 18:04:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 18:04:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 18:04:29 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 18:04:29 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 18:04:29 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 18:04:29 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1e09cb30a1ef0915a1ffb7a7e09dbfbbd6ca50b0de70ef22c1ecb37d83b229`  
		Last Modified: Wed, 16 Aug 2023 17:31:53 GMT  
		Size: 141.6 MB (141565229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f12873017d7c816d3c56930a0d6202a10c96ad52ef95a126e5419dc6d8c15b`  
		Last Modified: Wed, 16 Aug 2023 18:07:39 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb462b6795cf1fce5c344899df88a65ee5e813ea1b320754b2f070628555add7`  
		Last Modified: Wed, 16 Aug 2023 18:07:39 GMT  
		Size: 9.3 KB (9327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7e70cf329892db2521d62e29116deffbbc8b3185e6bf6d40d733faced14f3e`  
		Last Modified: Wed, 16 Aug 2023 18:07:47 GMT  
		Size: 122.2 MB (122178893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:f68efda475375454c3aa09633dc3893c0984f72252491ed19eeb77753ce7f05a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:4e263576afd9694d54d411b3d9dbd1ad11a6627cae25a63ede20566b5813f5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.5 MB (298549984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0078ab4e9e4976ab06453f01b57d4975e5224528b6f5c2d414f871d5d1fa6fc6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:02:38 GMT
COPY dir:72d046f3e284b8eca8066a837ab8a68f91b4cf5355de7f6803a8ee9b7ce3d682 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2e76f3d237648392c9fb43b6a93fbd30cb00da617a30d13712b386a69565e43a NEO4J_TARBALL=neo4j-community-4.4.24-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 17:02:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:02:40 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 17:02:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:02:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:02:52 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:02:52 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:02:52 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:02:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:02:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209f416efba54d09e37495a54336ac55d40fc467f753f97e78f060748b4513e5`  
		Last Modified: Wed, 16 Aug 2023 17:06:20 GMT  
		Size: 144.8 MB (144831672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d90d22bb9c3af24549dfdb794895f7ec444e1e7a2cf4b718fbfec705875b3a`  
		Last Modified: Wed, 16 Aug 2023 17:06:08 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40677c38fb05c03c597e2429ed8cb36f7393d42b0413c0c486540dee91fd7df`  
		Last Modified: Wed, 16 Aug 2023 17:06:08 GMT  
		Size: 9.3 KB (9324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd78884f79a99c17e0892e14f04a3350f264673410de7f82dd8fa1c25f31010`  
		Last Modified: Wed, 16 Aug 2023 17:06:15 GMT  
		Size: 122.3 MB (122287452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b133c2a9b52e6272811aa4f44355dea41c204fb8eccd166fb36fbaab0688226e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.8 MB (293820152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e408e84f33921d1ce862ec3ceacdb33b9591c4856863f287b082c406d01d9d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:22:18 GMT
COPY dir:6acc55ac013a722a8db4af8f0ce8de9270cd9aeb372e6c734b449d15adcc5218 in /opt/java/openjdk 
# Wed, 16 Aug 2023 18:04:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2e76f3d237648392c9fb43b6a93fbd30cb00da617a30d13712b386a69565e43a NEO4J_TARBALL=neo4j-community-4.4.24-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 18:04:18 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 18:04:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 18:04:19 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 18:04:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 18:04:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 18:04:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 18:04:29 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 18:04:29 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 18:04:29 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 18:04:29 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1e09cb30a1ef0915a1ffb7a7e09dbfbbd6ca50b0de70ef22c1ecb37d83b229`  
		Last Modified: Wed, 16 Aug 2023 17:31:53 GMT  
		Size: 141.6 MB (141565229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f12873017d7c816d3c56930a0d6202a10c96ad52ef95a126e5419dc6d8c15b`  
		Last Modified: Wed, 16 Aug 2023 18:07:39 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb462b6795cf1fce5c344899df88a65ee5e813ea1b320754b2f070628555add7`  
		Last Modified: Wed, 16 Aug 2023 18:07:39 GMT  
		Size: 9.3 KB (9327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7e70cf329892db2521d62e29116deffbbc8b3185e6bf6d40d733faced14f3e`  
		Last Modified: Wed, 16 Aug 2023 18:07:47 GMT  
		Size: 122.2 MB (122178893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:d3d9f7ba3e30578c6d5e350dd2d4df5dfe968f0c455710493933d2f914834688
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:98edc0360ba3371d33d48949283aa854ad5ec6724c5cca1c3bad12b2f9f32d19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.0 MB (398014150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95dc963300ea220e7f8fe2be8232cdfaa088fd8f8101b9532f72a93a9e643918`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:02:38 GMT
COPY dir:72d046f3e284b8eca8066a837ab8a68f91b4cf5355de7f6803a8ee9b7ce3d682 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=f1b4862dd7312590036d9167eb0120df62b792522ef2e567a59549bfad880cca NEO4J_TARBALL=neo4j-enterprise-4.4.24-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:56 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 17:02:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:02:57 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 17:03:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:03:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:03:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:03:12 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:03:12 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:03:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:03:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209f416efba54d09e37495a54336ac55d40fc467f753f97e78f060748b4513e5`  
		Last Modified: Wed, 16 Aug 2023 17:06:20 GMT  
		Size: 144.8 MB (144831672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a79f99067de6451801530c8d1c15f06ab08c8cb2c5f19c105708b1a4fcd630`  
		Last Modified: Wed, 16 Aug 2023 17:06:32 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69f7b6c012d6adc0c61d694a242fb84de74d4e5e5729c736533e5d57653a5af`  
		Last Modified: Wed, 16 Aug 2023 17:06:32 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477723cb6a8b21f2dd0278a28e572b30cfb2977ad3652506a2796333ea254bd`  
		Last Modified: Wed, 16 Aug 2023 17:06:43 GMT  
		Size: 221.8 MB (221751617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:dd9def3019ea59311c2decc09b6e68e04ceaf4f6e7d2137b9c89c01b1a88e370
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.3 MB (393285157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2e27c14ad3ac23ae15d860184abbf7a3c158a6886931a3f05c7f6787c042892`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:22:18 GMT
COPY dir:6acc55ac013a722a8db4af8f0ce8de9270cd9aeb372e6c734b449d15adcc5218 in /opt/java/openjdk 
# Wed, 16 Aug 2023 18:04:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=f1b4862dd7312590036d9167eb0120df62b792522ef2e567a59549bfad880cca NEO4J_TARBALL=neo4j-enterprise-4.4.24-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 18:04:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 18:04:32 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 18:04:32 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 18:04:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 18:04:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 18:04:46 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 18:04:46 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 18:04:46 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 18:04:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 18:04:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1e09cb30a1ef0915a1ffb7a7e09dbfbbd6ca50b0de70ef22c1ecb37d83b229`  
		Last Modified: Wed, 16 Aug 2023 17:31:53 GMT  
		Size: 141.6 MB (141565229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025d8d49ee65a6d6d52e8e9b49b73761d6ad0abdd931cb6b06908bc52c3b3d59`  
		Last Modified: Wed, 16 Aug 2023 18:08:00 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ed9f34b163ebcea6608dc14b742318f841c96449213d47b2fdb3e9a1f0b2de`  
		Last Modified: Wed, 16 Aug 2023 18:08:00 GMT  
		Size: 9.3 KB (9324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642c23fc8eb372fef6d739c83306d6a7ebf26d6c8e85e5f6eaebdbd169e269f1`  
		Last Modified: Wed, 16 Aug 2023 18:08:13 GMT  
		Size: 221.6 MB (221643901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.24`

```console
$ docker pull neo4j@sha256:f68efda475375454c3aa09633dc3893c0984f72252491ed19eeb77753ce7f05a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.24` - linux; amd64

```console
$ docker pull neo4j@sha256:4e263576afd9694d54d411b3d9dbd1ad11a6627cae25a63ede20566b5813f5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.5 MB (298549984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0078ab4e9e4976ab06453f01b57d4975e5224528b6f5c2d414f871d5d1fa6fc6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:02:38 GMT
COPY dir:72d046f3e284b8eca8066a837ab8a68f91b4cf5355de7f6803a8ee9b7ce3d682 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2e76f3d237648392c9fb43b6a93fbd30cb00da617a30d13712b386a69565e43a NEO4J_TARBALL=neo4j-community-4.4.24-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 17:02:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:02:40 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 17:02:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:02:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:02:52 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:02:52 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:02:52 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:02:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:02:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209f416efba54d09e37495a54336ac55d40fc467f753f97e78f060748b4513e5`  
		Last Modified: Wed, 16 Aug 2023 17:06:20 GMT  
		Size: 144.8 MB (144831672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d90d22bb9c3af24549dfdb794895f7ec444e1e7a2cf4b718fbfec705875b3a`  
		Last Modified: Wed, 16 Aug 2023 17:06:08 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40677c38fb05c03c597e2429ed8cb36f7393d42b0413c0c486540dee91fd7df`  
		Last Modified: Wed, 16 Aug 2023 17:06:08 GMT  
		Size: 9.3 KB (9324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd78884f79a99c17e0892e14f04a3350f264673410de7f82dd8fa1c25f31010`  
		Last Modified: Wed, 16 Aug 2023 17:06:15 GMT  
		Size: 122.3 MB (122287452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.24` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b133c2a9b52e6272811aa4f44355dea41c204fb8eccd166fb36fbaab0688226e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.8 MB (293820152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e408e84f33921d1ce862ec3ceacdb33b9591c4856863f287b082c406d01d9d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:22:18 GMT
COPY dir:6acc55ac013a722a8db4af8f0ce8de9270cd9aeb372e6c734b449d15adcc5218 in /opt/java/openjdk 
# Wed, 16 Aug 2023 18:04:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2e76f3d237648392c9fb43b6a93fbd30cb00da617a30d13712b386a69565e43a NEO4J_TARBALL=neo4j-community-4.4.24-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 18:04:18 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 18:04:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 18:04:19 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 18:04:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 18:04:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 18:04:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 18:04:29 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 18:04:29 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 18:04:29 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 18:04:29 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1e09cb30a1ef0915a1ffb7a7e09dbfbbd6ca50b0de70ef22c1ecb37d83b229`  
		Last Modified: Wed, 16 Aug 2023 17:31:53 GMT  
		Size: 141.6 MB (141565229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f12873017d7c816d3c56930a0d6202a10c96ad52ef95a126e5419dc6d8c15b`  
		Last Modified: Wed, 16 Aug 2023 18:07:39 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb462b6795cf1fce5c344899df88a65ee5e813ea1b320754b2f070628555add7`  
		Last Modified: Wed, 16 Aug 2023 18:07:39 GMT  
		Size: 9.3 KB (9327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7e70cf329892db2521d62e29116deffbbc8b3185e6bf6d40d733faced14f3e`  
		Last Modified: Wed, 16 Aug 2023 18:07:47 GMT  
		Size: 122.2 MB (122178893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.24-community`

```console
$ docker pull neo4j@sha256:f68efda475375454c3aa09633dc3893c0984f72252491ed19eeb77753ce7f05a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.24-community` - linux; amd64

```console
$ docker pull neo4j@sha256:4e263576afd9694d54d411b3d9dbd1ad11a6627cae25a63ede20566b5813f5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.5 MB (298549984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0078ab4e9e4976ab06453f01b57d4975e5224528b6f5c2d414f871d5d1fa6fc6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:02:38 GMT
COPY dir:72d046f3e284b8eca8066a837ab8a68f91b4cf5355de7f6803a8ee9b7ce3d682 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2e76f3d237648392c9fb43b6a93fbd30cb00da617a30d13712b386a69565e43a NEO4J_TARBALL=neo4j-community-4.4.24-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 17:02:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:02:40 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 17:02:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:02:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:02:52 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:02:52 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:02:52 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:02:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:02:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209f416efba54d09e37495a54336ac55d40fc467f753f97e78f060748b4513e5`  
		Last Modified: Wed, 16 Aug 2023 17:06:20 GMT  
		Size: 144.8 MB (144831672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d90d22bb9c3af24549dfdb794895f7ec444e1e7a2cf4b718fbfec705875b3a`  
		Last Modified: Wed, 16 Aug 2023 17:06:08 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40677c38fb05c03c597e2429ed8cb36f7393d42b0413c0c486540dee91fd7df`  
		Last Modified: Wed, 16 Aug 2023 17:06:08 GMT  
		Size: 9.3 KB (9324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd78884f79a99c17e0892e14f04a3350f264673410de7f82dd8fa1c25f31010`  
		Last Modified: Wed, 16 Aug 2023 17:06:15 GMT  
		Size: 122.3 MB (122287452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.24-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b133c2a9b52e6272811aa4f44355dea41c204fb8eccd166fb36fbaab0688226e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.8 MB (293820152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e408e84f33921d1ce862ec3ceacdb33b9591c4856863f287b082c406d01d9d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:22:18 GMT
COPY dir:6acc55ac013a722a8db4af8f0ce8de9270cd9aeb372e6c734b449d15adcc5218 in /opt/java/openjdk 
# Wed, 16 Aug 2023 18:04:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2e76f3d237648392c9fb43b6a93fbd30cb00da617a30d13712b386a69565e43a NEO4J_TARBALL=neo4j-community-4.4.24-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 18:04:18 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 18:04:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 18:04:19 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 18:04:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 18:04:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 18:04:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 18:04:29 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 18:04:29 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 18:04:29 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 18:04:29 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1e09cb30a1ef0915a1ffb7a7e09dbfbbd6ca50b0de70ef22c1ecb37d83b229`  
		Last Modified: Wed, 16 Aug 2023 17:31:53 GMT  
		Size: 141.6 MB (141565229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f12873017d7c816d3c56930a0d6202a10c96ad52ef95a126e5419dc6d8c15b`  
		Last Modified: Wed, 16 Aug 2023 18:07:39 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb462b6795cf1fce5c344899df88a65ee5e813ea1b320754b2f070628555add7`  
		Last Modified: Wed, 16 Aug 2023 18:07:39 GMT  
		Size: 9.3 KB (9327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7e70cf329892db2521d62e29116deffbbc8b3185e6bf6d40d733faced14f3e`  
		Last Modified: Wed, 16 Aug 2023 18:07:47 GMT  
		Size: 122.2 MB (122178893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.24-enterprise`

```console
$ docker pull neo4j@sha256:d3d9f7ba3e30578c6d5e350dd2d4df5dfe968f0c455710493933d2f914834688
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.24-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:98edc0360ba3371d33d48949283aa854ad5ec6724c5cca1c3bad12b2f9f32d19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.0 MB (398014150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95dc963300ea220e7f8fe2be8232cdfaa088fd8f8101b9532f72a93a9e643918`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:02:38 GMT
COPY dir:72d046f3e284b8eca8066a837ab8a68f91b4cf5355de7f6803a8ee9b7ce3d682 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=f1b4862dd7312590036d9167eb0120df62b792522ef2e567a59549bfad880cca NEO4J_TARBALL=neo4j-enterprise-4.4.24-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:56 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 17:02:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:02:57 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 17:03:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:03:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:03:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:03:12 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:03:12 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:03:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:03:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209f416efba54d09e37495a54336ac55d40fc467f753f97e78f060748b4513e5`  
		Last Modified: Wed, 16 Aug 2023 17:06:20 GMT  
		Size: 144.8 MB (144831672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a79f99067de6451801530c8d1c15f06ab08c8cb2c5f19c105708b1a4fcd630`  
		Last Modified: Wed, 16 Aug 2023 17:06:32 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69f7b6c012d6adc0c61d694a242fb84de74d4e5e5729c736533e5d57653a5af`  
		Last Modified: Wed, 16 Aug 2023 17:06:32 GMT  
		Size: 9.3 KB (9325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477723cb6a8b21f2dd0278a28e572b30cfb2977ad3652506a2796333ea254bd`  
		Last Modified: Wed, 16 Aug 2023 17:06:43 GMT  
		Size: 221.8 MB (221751617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.24-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:dd9def3019ea59311c2decc09b6e68e04ceaf4f6e7d2137b9c89c01b1a88e370
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.3 MB (393285157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2e27c14ad3ac23ae15d860184abbf7a3c158a6886931a3f05c7f6787c042892`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:22:18 GMT
COPY dir:6acc55ac013a722a8db4af8f0ce8de9270cd9aeb372e6c734b449d15adcc5218 in /opt/java/openjdk 
# Wed, 16 Aug 2023 18:04:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=f1b4862dd7312590036d9167eb0120df62b792522ef2e567a59549bfad880cca NEO4J_TARBALL=neo4j-enterprise-4.4.24-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 18:04:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
# Wed, 16 Aug 2023 18:04:32 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 18:04:32 GMT
COPY multi:269f2bb89a34e8e23b4028baf2582795a6378669e17bfcf98f4ae14c2de48e0b in /startup/ 
# Wed, 16 Aug 2023 18:04:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.24-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 18:04:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 18:04:46 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 18:04:46 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 18:04:46 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 18:04:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 18:04:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1e09cb30a1ef0915a1ffb7a7e09dbfbbd6ca50b0de70ef22c1ecb37d83b229`  
		Last Modified: Wed, 16 Aug 2023 17:31:53 GMT  
		Size: 141.6 MB (141565229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025d8d49ee65a6d6d52e8e9b49b73761d6ad0abdd931cb6b06908bc52c3b3d59`  
		Last Modified: Wed, 16 Aug 2023 18:08:00 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ed9f34b163ebcea6608dc14b742318f841c96449213d47b2fdb3e9a1f0b2de`  
		Last Modified: Wed, 16 Aug 2023 18:08:00 GMT  
		Size: 9.3 KB (9324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642c23fc8eb372fef6d739c83306d6a7ebf26d6c8e85e5f6eaebdbd169e269f1`  
		Last Modified: Wed, 16 Aug 2023 18:08:13 GMT  
		Size: 221.6 MB (221643901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:2ea377845b25c84abed770d3be98ea5623f516144d3c5fb2b23d2aa7b16e09f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:d9fcd1c71ea4e113f76510f6ef953e545deba39d2f20baf5da86643db3625a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293694805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548e2d88b9907e17f5ed7ceef2b3d196a0241ebd328082629cdacee40bfa2717`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:13 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:14 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:27 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:27 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:27 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbbcabbc7f08c2176d6fcdda81fb40b452e0264f9210cd51b07cc5a29c8d14`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f078447b9e5feac9152dfd0e26ee1626a52eb32132e7b957429611990fb109`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbec5ecbe9f75583c2f1ad50fb132b61bd12cfd93d0dd28a06fb5d8b822e9e81`  
		Last Modified: Wed, 16 Aug 2023 17:03:46 GMT  
		Size: 117.5 MB (117490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-bullseye`

```console
$ docker pull neo4j@sha256:2ea377845b25c84abed770d3be98ea5623f516144d3c5fb2b23d2aa7b16e09f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:d9fcd1c71ea4e113f76510f6ef953e545deba39d2f20baf5da86643db3625a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293694805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548e2d88b9907e17f5ed7ceef2b3d196a0241ebd328082629cdacee40bfa2717`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:13 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:14 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:27 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:27 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:27 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbbcabbc7f08c2176d6fcdda81fb40b452e0264f9210cd51b07cc5a29c8d14`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f078447b9e5feac9152dfd0e26ee1626a52eb32132e7b957429611990fb109`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbec5ecbe9f75583c2f1ad50fb132b61bd12cfd93d0dd28a06fb5d8b822e9e81`  
		Last Modified: Wed, 16 Aug 2023 17:03:46 GMT  
		Size: 117.5 MB (117490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:2ea377845b25c84abed770d3be98ea5623f516144d3c5fb2b23d2aa7b16e09f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:d9fcd1c71ea4e113f76510f6ef953e545deba39d2f20baf5da86643db3625a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293694805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548e2d88b9907e17f5ed7ceef2b3d196a0241ebd328082629cdacee40bfa2717`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:13 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:14 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:27 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:27 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:27 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbbcabbc7f08c2176d6fcdda81fb40b452e0264f9210cd51b07cc5a29c8d14`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f078447b9e5feac9152dfd0e26ee1626a52eb32132e7b957429611990fb109`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbec5ecbe9f75583c2f1ad50fb132b61bd12cfd93d0dd28a06fb5d8b822e9e81`  
		Last Modified: Wed, 16 Aug 2023 17:03:46 GMT  
		Size: 117.5 MB (117490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community-bullseye`

```console
$ docker pull neo4j@sha256:2ea377845b25c84abed770d3be98ea5623f516144d3c5fb2b23d2aa7b16e09f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:d9fcd1c71ea4e113f76510f6ef953e545deba39d2f20baf5da86643db3625a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293694805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548e2d88b9907e17f5ed7ceef2b3d196a0241ebd328082629cdacee40bfa2717`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:13 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:14 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:27 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:27 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:27 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbbcabbc7f08c2176d6fcdda81fb40b452e0264f9210cd51b07cc5a29c8d14`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f078447b9e5feac9152dfd0e26ee1626a52eb32132e7b957429611990fb109`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbec5ecbe9f75583c2f1ad50fb132b61bd12cfd93d0dd28a06fb5d8b822e9e81`  
		Last Modified: Wed, 16 Aug 2023 17:03:46 GMT  
		Size: 117.5 MB (117490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community-ubi8`

```console
$ docker pull neo4j@sha256:d25e228710b277a03fe7dec31192b77339a7bf8a5b8b6cae8ba08bba23ef3824
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:71e9d964d3efc40f97d0b7b1be84508554794db93b29dba8111b7e9365c39d17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.3 MB (304288700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6fec9a77d8fff42eb6e150b0af89ae0ed70976cb6eeb48dc6e27ec4173fd881`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:34 GMT
ADD file:84dff5b0f84a1086a0a07b28849d08a18f2d658869173d376845a20a2cb34541 in / 
# Wed, 03 May 2023 15:11:35 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:35 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:36 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:36 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:36 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:36 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:36 GMT
ENV container oci
# Wed, 03 May 2023 15:11:36 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:36 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:36 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:36 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:37 GMT
ADD file:13e13737bf27853f3a47e1f55b843236868d5521b05c5fed54688856d11bd33f in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:37 GMT
ADD file:fcaeea1e052139bcd93a719356f6d30b0bd66243e25ccb0a8ed0e3b2013b5804 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:37 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:38 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:39 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:40 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 22:58:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:59 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:09 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Wed, 16 Aug 2023 17:02:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:02:09 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:02:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Wed, 16 Aug 2023 17:02:14 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:02:14 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:02:14 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:02:14 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:02:14 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:02:14 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccd9537bc52f60ded583bf06bc3a05063d4e52cbcd3d48df8c2748d454856e0`  
		Last Modified: Wed, 16 Aug 2023 17:05:18 GMT  
		Size: 144.8 MB (144773734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd322d091d865b89a25ec0a0e720119978c93f4020e1425c4294294088c205`  
		Last Modified: Wed, 16 Aug 2023 17:05:07 GMT  
		Size: 6.5 MB (6535977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde16abe682e00a68f584511d44efc49d2d49c02cad218f83cfde87541558447`  
		Last Modified: Wed, 16 Aug 2023 17:05:06 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a705d32035826f6b06be16631ac76d04e427ebe3a6f80b84a1477316f1b27e`  
		Last Modified: Wed, 16 Aug 2023 17:05:13 GMT  
		Size: 113.7 MB (113680595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9e46a4e4523b846c406c8df4a0c5b00f46e012cf5a335a4c56b5abdee56508d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301283576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5583646a630dc67b5478bcf12d494f23d9d3111bee3beea3312d2dd5cdb25595`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:42 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:46 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:46 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:46 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde3669de5dd9b71b5171db0ea80172e0434dd626fff921721810bdcd4da1abc`  
		Last Modified: Thu, 17 Aug 2023 01:28:55 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af814bcc2ddcf3c718c73ebb2ef5df96d2d0b35e9863c7dbf681ae9d5bae8a67`  
		Last Modified: Thu, 17 Aug 2023 01:29:01 GMT  
		Size: 113.7 MB (113704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:7be3d18f2b483bc0e4f717a46da8d5fe194ccad625cec86cde37ed98df9323d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:e48c29a2a94e1fe271d99d7ac3004ac4063e8cb7c874ea109694ad6b42e86f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.7 MB (574730794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b649ba4d2049bbd3cbde12aa2c123ddf28938b261d50da6cc8cddd0583705265`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:35 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:53 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:53 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:53 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:53 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916f94c1852938d165a027bfab885fdd0a04b6e17e011054ef437686fa96a40`  
		Last Modified: Wed, 16 Aug 2023 17:04:25 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308a66a2c4e044da61750ee3d666ae4b097a785e4c16365a5bed109c8be94994`  
		Last Modified: Wed, 16 Aug 2023 17:04:25 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff50bbd26468a734945fa2c0b5c004fe30bce87d223ea58eb3c84bbb5197776`  
		Last Modified: Wed, 16 Aug 2023 17:04:46 GMT  
		Size: 398.5 MB (398526180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:abcf760aa951a2d46741862c665adaf396d8bfdedfaaf53f4bfb866d744fb5a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.2 MB (577205982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:498c6b3fff483a76f8a78e912d01038f6b06995cb1fe860c8745666a6397bb4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:56 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:26:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:25 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:25 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bdfd7bf6c0410f6c5d3d5b1c09367d8da9a6b6dbb9a8600659fa1f060803f9`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc332bdc9cb98200cd3a234f8e71d7517e5525f507efe285373f227af49de3`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5645b7152fbaf5c18bf624421781149836837a9c5d71f898c771c42234f28384`  
		Last Modified: Thu, 17 Aug 2023 01:28:33 GMT  
		Size: 403.6 MB (403591821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:7be3d18f2b483bc0e4f717a46da8d5fe194ccad625cec86cde37ed98df9323d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:e48c29a2a94e1fe271d99d7ac3004ac4063e8cb7c874ea109694ad6b42e86f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.7 MB (574730794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b649ba4d2049bbd3cbde12aa2c123ddf28938b261d50da6cc8cddd0583705265`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:35 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:53 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:53 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:53 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:53 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916f94c1852938d165a027bfab885fdd0a04b6e17e011054ef437686fa96a40`  
		Last Modified: Wed, 16 Aug 2023 17:04:25 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308a66a2c4e044da61750ee3d666ae4b097a785e4c16365a5bed109c8be94994`  
		Last Modified: Wed, 16 Aug 2023 17:04:25 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff50bbd26468a734945fa2c0b5c004fe30bce87d223ea58eb3c84bbb5197776`  
		Last Modified: Wed, 16 Aug 2023 17:04:46 GMT  
		Size: 398.5 MB (398526180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:abcf760aa951a2d46741862c665adaf396d8bfdedfaaf53f4bfb866d744fb5a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.2 MB (577205982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:498c6b3fff483a76f8a78e912d01038f6b06995cb1fe860c8745666a6397bb4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:56 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:26:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:25 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:25 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bdfd7bf6c0410f6c5d3d5b1c09367d8da9a6b6dbb9a8600659fa1f060803f9`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc332bdc9cb98200cd3a234f8e71d7517e5525f507efe285373f227af49de3`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5645b7152fbaf5c18bf624421781149836837a9c5d71f898c771c42234f28384`  
		Last Modified: Thu, 17 Aug 2023 01:28:33 GMT  
		Size: 403.6 MB (403591821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:b6294fc3448ffe46caa396a1ede70ec01aaca0d8dce75127e302aa4d0fc820a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:58a8bd3a41dfd17b5e331ef13c3885001f18ff8bdf664eda0dcf346a69fa1cf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **585.3 MB (585324104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ebdb04867b6ca5f7cc373d1da99c9438cb0274898485e42187e7cc779f4dce6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:34 GMT
ADD file:84dff5b0f84a1086a0a07b28849d08a18f2d658869173d376845a20a2cb34541 in / 
# Wed, 03 May 2023 15:11:35 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:35 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:36 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:36 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:36 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:36 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:36 GMT
ENV container oci
# Wed, 03 May 2023 15:11:36 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:36 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:36 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:36 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:37 GMT
ADD file:13e13737bf27853f3a47e1f55b843236868d5521b05c5fed54688856d11bd33f in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:37 GMT
ADD file:fcaeea1e052139bcd93a719356f6d30b0bd66243e25ccb0a8ed0e3b2013b5804 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:37 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:38 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:39 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:40 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 22:58:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:59 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:09 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Wed, 16 Aug 2023 17:02:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:18 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:02:19 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:02:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Wed, 16 Aug 2023 17:02:30 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:02:30 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:02:30 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:02:30 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:02:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:02:31 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccd9537bc52f60ded583bf06bc3a05063d4e52cbcd3d48df8c2748d454856e0`  
		Last Modified: Wed, 16 Aug 2023 17:05:18 GMT  
		Size: 144.8 MB (144773734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd322d091d865b89a25ec0a0e720119978c93f4020e1425c4294294088c205`  
		Last Modified: Wed, 16 Aug 2023 17:05:07 GMT  
		Size: 6.5 MB (6535977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7a1b0e8a796e4fb9646cdd687e14fbb293e149037badc1e33966dbec58fb7f`  
		Last Modified: Wed, 16 Aug 2023 17:05:38 GMT  
		Size: 9.3 KB (9346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2b59785d2be424bb71a8a11cfaaef65885f250e3f0c0789e2b87870c827408`  
		Last Modified: Wed, 16 Aug 2023 17:05:56 GMT  
		Size: 394.7 MB (394716003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5db3cad3d34b4680e70762d88126cb5fb450465fa721b73138170f26c75d9ff5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **587.5 MB (587472173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673c50148db3dd955f7449f7b19d05a324dfeb168fc879f9edf8853a4b138594`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:48 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:48 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:59 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:27:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:27:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:27:01 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:27:01 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:27:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:27:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282ab0089796bc90ec405471494fce4aeb906f83c41d56f4eee5b53f7b7fe7c`  
		Last Modified: Thu, 17 Aug 2023 01:29:22 GMT  
		Size: 9.3 KB (9345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a067445f68579ce62d30a406c181f714a8f6ef4ae77461bbcf681b9ae3709a76`  
		Last Modified: Thu, 17 Aug 2023 01:29:40 GMT  
		Size: 399.9 MB (399892982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-ubi8`

```console
$ docker pull neo4j@sha256:d25e228710b277a03fe7dec31192b77339a7bf8a5b8b6cae8ba08bba23ef3824
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:71e9d964d3efc40f97d0b7b1be84508554794db93b29dba8111b7e9365c39d17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.3 MB (304288700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6fec9a77d8fff42eb6e150b0af89ae0ed70976cb6eeb48dc6e27ec4173fd881`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:34 GMT
ADD file:84dff5b0f84a1086a0a07b28849d08a18f2d658869173d376845a20a2cb34541 in / 
# Wed, 03 May 2023 15:11:35 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:35 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:36 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:36 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:36 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:36 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:36 GMT
ENV container oci
# Wed, 03 May 2023 15:11:36 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:36 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:36 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:36 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:37 GMT
ADD file:13e13737bf27853f3a47e1f55b843236868d5521b05c5fed54688856d11bd33f in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:37 GMT
ADD file:fcaeea1e052139bcd93a719356f6d30b0bd66243e25ccb0a8ed0e3b2013b5804 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:37 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:38 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:39 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:40 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 22:58:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:59 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:09 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Wed, 16 Aug 2023 17:02:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:02:09 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:02:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Wed, 16 Aug 2023 17:02:14 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:02:14 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:02:14 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:02:14 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:02:14 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:02:14 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccd9537bc52f60ded583bf06bc3a05063d4e52cbcd3d48df8c2748d454856e0`  
		Last Modified: Wed, 16 Aug 2023 17:05:18 GMT  
		Size: 144.8 MB (144773734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd322d091d865b89a25ec0a0e720119978c93f4020e1425c4294294088c205`  
		Last Modified: Wed, 16 Aug 2023 17:05:07 GMT  
		Size: 6.5 MB (6535977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde16abe682e00a68f584511d44efc49d2d49c02cad218f83cfde87541558447`  
		Last Modified: Wed, 16 Aug 2023 17:05:06 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a705d32035826f6b06be16631ac76d04e427ebe3a6f80b84a1477316f1b27e`  
		Last Modified: Wed, 16 Aug 2023 17:05:13 GMT  
		Size: 113.7 MB (113680595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9e46a4e4523b846c406c8df4a0c5b00f46e012cf5a335a4c56b5abdee56508d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301283576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5583646a630dc67b5478bcf12d494f23d9d3111bee3beea3312d2dd5cdb25595`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:42 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:46 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:46 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:46 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde3669de5dd9b71b5171db0ea80172e0434dd626fff921721810bdcd4da1abc`  
		Last Modified: Thu, 17 Aug 2023 01:28:55 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af814bcc2ddcf3c718c73ebb2ef5df96d2d0b35e9863c7dbf681ae9d5bae8a67`  
		Last Modified: Thu, 17 Aug 2023 01:29:01 GMT  
		Size: 113.7 MB (113704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11`

```console
$ docker pull neo4j@sha256:f582c7bb4666892abe0ce03af3100873daf378cb01f8c2bee87ab0adee798dc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11-bullseye`

```console
$ docker pull neo4j@sha256:f582c7bb4666892abe0ce03af3100873daf378cb01f8c2bee87ab0adee798dc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11-community`

```console
$ docker pull neo4j@sha256:f582c7bb4666892abe0ce03af3100873daf378cb01f8c2bee87ab0adee798dc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11-community-bullseye`

```console
$ docker pull neo4j@sha256:f582c7bb4666892abe0ce03af3100873daf378cb01f8c2bee87ab0adee798dc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11-community-ubi8`

```console
$ docker pull neo4j@sha256:7f443f914e42ddf53d0614cc813c7bd5a4b43241c976d09abae5b49d045bfae6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9e46a4e4523b846c406c8df4a0c5b00f46e012cf5a335a4c56b5abdee56508d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301283576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5583646a630dc67b5478bcf12d494f23d9d3111bee3beea3312d2dd5cdb25595`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:42 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:46 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:46 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:46 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde3669de5dd9b71b5171db0ea80172e0434dd626fff921721810bdcd4da1abc`  
		Last Modified: Thu, 17 Aug 2023 01:28:55 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af814bcc2ddcf3c718c73ebb2ef5df96d2d0b35e9863c7dbf681ae9d5bae8a67`  
		Last Modified: Thu, 17 Aug 2023 01:29:01 GMT  
		Size: 113.7 MB (113704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11-enterprise`

```console
$ docker pull neo4j@sha256:d0a28d855aa92962ec30ec2903fade1b4cafdd7308f0761c9f15bcbb8804fa8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:abcf760aa951a2d46741862c665adaf396d8bfdedfaaf53f4bfb866d744fb5a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.2 MB (577205982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:498c6b3fff483a76f8a78e912d01038f6b06995cb1fe860c8745666a6397bb4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:56 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:26:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:25 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:25 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bdfd7bf6c0410f6c5d3d5b1c09367d8da9a6b6dbb9a8600659fa1f060803f9`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc332bdc9cb98200cd3a234f8e71d7517e5525f507efe285373f227af49de3`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5645b7152fbaf5c18bf624421781149836837a9c5d71f898c771c42234f28384`  
		Last Modified: Thu, 17 Aug 2023 01:28:33 GMT  
		Size: 403.6 MB (403591821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:d0a28d855aa92962ec30ec2903fade1b4cafdd7308f0761c9f15bcbb8804fa8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:abcf760aa951a2d46741862c665adaf396d8bfdedfaaf53f4bfb866d744fb5a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.2 MB (577205982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:498c6b3fff483a76f8a78e912d01038f6b06995cb1fe860c8745666a6397bb4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:56 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:26:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:25 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:25 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bdfd7bf6c0410f6c5d3d5b1c09367d8da9a6b6dbb9a8600659fa1f060803f9`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc332bdc9cb98200cd3a234f8e71d7517e5525f507efe285373f227af49de3`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5645b7152fbaf5c18bf624421781149836837a9c5d71f898c771c42234f28384`  
		Last Modified: Thu, 17 Aug 2023 01:28:33 GMT  
		Size: 403.6 MB (403591821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:15e15a3f53025d70acf9d694f92125d5d6f6f32bd12bf4f892b8ab00d8a15a70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11-enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5db3cad3d34b4680e70762d88126cb5fb450465fa721b73138170f26c75d9ff5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **587.5 MB (587472173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673c50148db3dd955f7449f7b19d05a324dfeb168fc879f9edf8853a4b138594`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:48 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:48 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:59 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:27:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:27:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:27:01 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:27:01 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:27:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:27:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282ab0089796bc90ec405471494fce4aeb906f83c41d56f4eee5b53f7b7fe7c`  
		Last Modified: Thu, 17 Aug 2023 01:29:22 GMT  
		Size: 9.3 KB (9345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a067445f68579ce62d30a406c181f714a8f6ef4ae77461bbcf681b9ae3709a76`  
		Last Modified: Thu, 17 Aug 2023 01:29:40 GMT  
		Size: 399.9 MB (399892982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11-ubi8`

```console
$ docker pull neo4j@sha256:7f443f914e42ddf53d0614cc813c7bd5a4b43241c976d09abae5b49d045bfae6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9e46a4e4523b846c406c8df4a0c5b00f46e012cf5a335a4c56b5abdee56508d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301283576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5583646a630dc67b5478bcf12d494f23d9d3111bee3beea3312d2dd5cdb25595`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:42 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:46 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:46 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:46 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde3669de5dd9b71b5171db0ea80172e0434dd626fff921721810bdcd4da1abc`  
		Last Modified: Thu, 17 Aug 2023 01:28:55 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af814bcc2ddcf3c718c73ebb2ef5df96d2d0b35e9863c7dbf681ae9d5bae8a67`  
		Last Modified: Thu, 17 Aug 2023 01:29:01 GMT  
		Size: 113.7 MB (113704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11.0`

```console
$ docker pull neo4j@sha256:f582c7bb4666892abe0ce03af3100873daf378cb01f8c2bee87ab0adee798dc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11.0-bullseye`

```console
$ docker pull neo4j@sha256:f582c7bb4666892abe0ce03af3100873daf378cb01f8c2bee87ab0adee798dc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11.0-community`

```console
$ docker pull neo4j@sha256:f582c7bb4666892abe0ce03af3100873daf378cb01f8c2bee87ab0adee798dc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11.0-community-bullseye`

```console
$ docker pull neo4j@sha256:f582c7bb4666892abe0ce03af3100873daf378cb01f8c2bee87ab0adee798dc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11.0-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11.0-community-ubi8`

```console
$ docker pull neo4j@sha256:7f443f914e42ddf53d0614cc813c7bd5a4b43241c976d09abae5b49d045bfae6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11.0-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9e46a4e4523b846c406c8df4a0c5b00f46e012cf5a335a4c56b5abdee56508d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301283576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5583646a630dc67b5478bcf12d494f23d9d3111bee3beea3312d2dd5cdb25595`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:42 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:46 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:46 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:46 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde3669de5dd9b71b5171db0ea80172e0434dd626fff921721810bdcd4da1abc`  
		Last Modified: Thu, 17 Aug 2023 01:28:55 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af814bcc2ddcf3c718c73ebb2ef5df96d2d0b35e9863c7dbf681ae9d5bae8a67`  
		Last Modified: Thu, 17 Aug 2023 01:29:01 GMT  
		Size: 113.7 MB (113704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11.0-enterprise`

```console
$ docker pull neo4j@sha256:d0a28d855aa92962ec30ec2903fade1b4cafdd7308f0761c9f15bcbb8804fa8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:abcf760aa951a2d46741862c665adaf396d8bfdedfaaf53f4bfb866d744fb5a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.2 MB (577205982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:498c6b3fff483a76f8a78e912d01038f6b06995cb1fe860c8745666a6397bb4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:56 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:26:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:25 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:25 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bdfd7bf6c0410f6c5d3d5b1c09367d8da9a6b6dbb9a8600659fa1f060803f9`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc332bdc9cb98200cd3a234f8e71d7517e5525f507efe285373f227af49de3`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5645b7152fbaf5c18bf624421781149836837a9c5d71f898c771c42234f28384`  
		Last Modified: Thu, 17 Aug 2023 01:28:33 GMT  
		Size: 403.6 MB (403591821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11.0-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:d0a28d855aa92962ec30ec2903fade1b4cafdd7308f0761c9f15bcbb8804fa8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11.0-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:abcf760aa951a2d46741862c665adaf396d8bfdedfaaf53f4bfb866d744fb5a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.2 MB (577205982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:498c6b3fff483a76f8a78e912d01038f6b06995cb1fe860c8745666a6397bb4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:56 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:26:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:25 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:25 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bdfd7bf6c0410f6c5d3d5b1c09367d8da9a6b6dbb9a8600659fa1f060803f9`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc332bdc9cb98200cd3a234f8e71d7517e5525f507efe285373f227af49de3`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5645b7152fbaf5c18bf624421781149836837a9c5d71f898c771c42234f28384`  
		Last Modified: Thu, 17 Aug 2023 01:28:33 GMT  
		Size: 403.6 MB (403591821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11.0-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:15e15a3f53025d70acf9d694f92125d5d6f6f32bd12bf4f892b8ab00d8a15a70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11.0-enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5db3cad3d34b4680e70762d88126cb5fb450465fa721b73138170f26c75d9ff5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **587.5 MB (587472173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673c50148db3dd955f7449f7b19d05a324dfeb168fc879f9edf8853a4b138594`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:48 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:48 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:59 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:27:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:27:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:27:01 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:27:01 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:27:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:27:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282ab0089796bc90ec405471494fce4aeb906f83c41d56f4eee5b53f7b7fe7c`  
		Last Modified: Thu, 17 Aug 2023 01:29:22 GMT  
		Size: 9.3 KB (9345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a067445f68579ce62d30a406c181f714a8f6ef4ae77461bbcf681b9ae3709a76`  
		Last Modified: Thu, 17 Aug 2023 01:29:40 GMT  
		Size: 399.9 MB (399892982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.11.0-ubi8`

```console
$ docker pull neo4j@sha256:7f443f914e42ddf53d0614cc813c7bd5a4b43241c976d09abae5b49d045bfae6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `neo4j:5.11.0-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9e46a4e4523b846c406c8df4a0c5b00f46e012cf5a335a4c56b5abdee56508d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301283576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5583646a630dc67b5478bcf12d494f23d9d3111bee3beea3312d2dd5cdb25595`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:42 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:46 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:46 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:46 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde3669de5dd9b71b5171db0ea80172e0434dd626fff921721810bdcd4da1abc`  
		Last Modified: Thu, 17 Aug 2023 01:28:55 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af814bcc2ddcf3c718c73ebb2ef5df96d2d0b35e9863c7dbf681ae9d5bae8a67`  
		Last Modified: Thu, 17 Aug 2023 01:29:01 GMT  
		Size: 113.7 MB (113704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:bullseye`

```console
$ docker pull neo4j@sha256:2ea377845b25c84abed770d3be98ea5623f516144d3c5fb2b23d2aa7b16e09f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:d9fcd1c71ea4e113f76510f6ef953e545deba39d2f20baf5da86643db3625a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293694805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548e2d88b9907e17f5ed7ceef2b3d196a0241ebd328082629cdacee40bfa2717`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:13 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:14 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:27 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:27 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:27 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbbcabbc7f08c2176d6fcdda81fb40b452e0264f9210cd51b07cc5a29c8d14`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f078447b9e5feac9152dfd0e26ee1626a52eb32132e7b957429611990fb109`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbec5ecbe9f75583c2f1ad50fb132b61bd12cfd93d0dd28a06fb5d8b822e9e81`  
		Last Modified: Wed, 16 Aug 2023 17:03:46 GMT  
		Size: 117.5 MB (117490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:2ea377845b25c84abed770d3be98ea5623f516144d3c5fb2b23d2aa7b16e09f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:d9fcd1c71ea4e113f76510f6ef953e545deba39d2f20baf5da86643db3625a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293694805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548e2d88b9907e17f5ed7ceef2b3d196a0241ebd328082629cdacee40bfa2717`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:13 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:14 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:27 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:27 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:27 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbbcabbc7f08c2176d6fcdda81fb40b452e0264f9210cd51b07cc5a29c8d14`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f078447b9e5feac9152dfd0e26ee1626a52eb32132e7b957429611990fb109`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbec5ecbe9f75583c2f1ad50fb132b61bd12cfd93d0dd28a06fb5d8b822e9e81`  
		Last Modified: Wed, 16 Aug 2023 17:03:46 GMT  
		Size: 117.5 MB (117490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community-bullseye`

```console
$ docker pull neo4j@sha256:2ea377845b25c84abed770d3be98ea5623f516144d3c5fb2b23d2aa7b16e09f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:d9fcd1c71ea4e113f76510f6ef953e545deba39d2f20baf5da86643db3625a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293694805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548e2d88b9907e17f5ed7ceef2b3d196a0241ebd328082629cdacee40bfa2717`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:13 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:14 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:27 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:27 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:27 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbbcabbc7f08c2176d6fcdda81fb40b452e0264f9210cd51b07cc5a29c8d14`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f078447b9e5feac9152dfd0e26ee1626a52eb32132e7b957429611990fb109`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbec5ecbe9f75583c2f1ad50fb132b61bd12cfd93d0dd28a06fb5d8b822e9e81`  
		Last Modified: Wed, 16 Aug 2023 17:03:46 GMT  
		Size: 117.5 MB (117490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community-ubi8`

```console
$ docker pull neo4j@sha256:d25e228710b277a03fe7dec31192b77339a7bf8a5b8b6cae8ba08bba23ef3824
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:71e9d964d3efc40f97d0b7b1be84508554794db93b29dba8111b7e9365c39d17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.3 MB (304288700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6fec9a77d8fff42eb6e150b0af89ae0ed70976cb6eeb48dc6e27ec4173fd881`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:34 GMT
ADD file:84dff5b0f84a1086a0a07b28849d08a18f2d658869173d376845a20a2cb34541 in / 
# Wed, 03 May 2023 15:11:35 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:35 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:36 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:36 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:36 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:36 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:36 GMT
ENV container oci
# Wed, 03 May 2023 15:11:36 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:36 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:36 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:36 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:37 GMT
ADD file:13e13737bf27853f3a47e1f55b843236868d5521b05c5fed54688856d11bd33f in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:37 GMT
ADD file:fcaeea1e052139bcd93a719356f6d30b0bd66243e25ccb0a8ed0e3b2013b5804 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:37 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:38 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:39 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:40 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 22:58:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:59 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:09 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Wed, 16 Aug 2023 17:02:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:02:09 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:02:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Wed, 16 Aug 2023 17:02:14 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:02:14 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:02:14 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:02:14 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:02:14 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:02:14 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccd9537bc52f60ded583bf06bc3a05063d4e52cbcd3d48df8c2748d454856e0`  
		Last Modified: Wed, 16 Aug 2023 17:05:18 GMT  
		Size: 144.8 MB (144773734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd322d091d865b89a25ec0a0e720119978c93f4020e1425c4294294088c205`  
		Last Modified: Wed, 16 Aug 2023 17:05:07 GMT  
		Size: 6.5 MB (6535977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde16abe682e00a68f584511d44efc49d2d49c02cad218f83cfde87541558447`  
		Last Modified: Wed, 16 Aug 2023 17:05:06 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a705d32035826f6b06be16631ac76d04e427ebe3a6f80b84a1477316f1b27e`  
		Last Modified: Wed, 16 Aug 2023 17:05:13 GMT  
		Size: 113.7 MB (113680595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9e46a4e4523b846c406c8df4a0c5b00f46e012cf5a335a4c56b5abdee56508d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301283576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5583646a630dc67b5478bcf12d494f23d9d3111bee3beea3312d2dd5cdb25595`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:42 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:46 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:46 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:46 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde3669de5dd9b71b5171db0ea80172e0434dd626fff921721810bdcd4da1abc`  
		Last Modified: Thu, 17 Aug 2023 01:28:55 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af814bcc2ddcf3c718c73ebb2ef5df96d2d0b35e9863c7dbf681ae9d5bae8a67`  
		Last Modified: Thu, 17 Aug 2023 01:29:01 GMT  
		Size: 113.7 MB (113704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:7be3d18f2b483bc0e4f717a46da8d5fe194ccad625cec86cde37ed98df9323d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:e48c29a2a94e1fe271d99d7ac3004ac4063e8cb7c874ea109694ad6b42e86f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.7 MB (574730794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b649ba4d2049bbd3cbde12aa2c123ddf28938b261d50da6cc8cddd0583705265`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:35 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:53 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:53 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:53 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:53 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916f94c1852938d165a027bfab885fdd0a04b6e17e011054ef437686fa96a40`  
		Last Modified: Wed, 16 Aug 2023 17:04:25 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308a66a2c4e044da61750ee3d666ae4b097a785e4c16365a5bed109c8be94994`  
		Last Modified: Wed, 16 Aug 2023 17:04:25 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff50bbd26468a734945fa2c0b5c004fe30bce87d223ea58eb3c84bbb5197776`  
		Last Modified: Wed, 16 Aug 2023 17:04:46 GMT  
		Size: 398.5 MB (398526180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:abcf760aa951a2d46741862c665adaf396d8bfdedfaaf53f4bfb866d744fb5a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.2 MB (577205982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:498c6b3fff483a76f8a78e912d01038f6b06995cb1fe860c8745666a6397bb4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:56 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:26:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:25 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:25 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bdfd7bf6c0410f6c5d3d5b1c09367d8da9a6b6dbb9a8600659fa1f060803f9`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc332bdc9cb98200cd3a234f8e71d7517e5525f507efe285373f227af49de3`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5645b7152fbaf5c18bf624421781149836837a9c5d71f898c771c42234f28384`  
		Last Modified: Thu, 17 Aug 2023 01:28:33 GMT  
		Size: 403.6 MB (403591821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise-bullseye`

```console
$ docker pull neo4j@sha256:7be3d18f2b483bc0e4f717a46da8d5fe194ccad625cec86cde37ed98df9323d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:e48c29a2a94e1fe271d99d7ac3004ac4063e8cb7c874ea109694ad6b42e86f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.7 MB (574730794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b649ba4d2049bbd3cbde12aa2c123ddf28938b261d50da6cc8cddd0583705265`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:34 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:35 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:53 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:53 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:53 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:53 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916f94c1852938d165a027bfab885fdd0a04b6e17e011054ef437686fa96a40`  
		Last Modified: Wed, 16 Aug 2023 17:04:25 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308a66a2c4e044da61750ee3d666ae4b097a785e4c16365a5bed109c8be94994`  
		Last Modified: Wed, 16 Aug 2023 17:04:25 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff50bbd26468a734945fa2c0b5c004fe30bce87d223ea58eb3c84bbb5197776`  
		Last Modified: Wed, 16 Aug 2023 17:04:46 GMT  
		Size: 398.5 MB (398526180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:abcf760aa951a2d46741862c665adaf396d8bfdedfaaf53f4bfb866d744fb5a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.2 MB (577205982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:498c6b3fff483a76f8a78e912d01038f6b06995cb1fe860c8745666a6397bb4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:56 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:26:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:25 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:25 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:25 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bdfd7bf6c0410f6c5d3d5b1c09367d8da9a6b6dbb9a8600659fa1f060803f9`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc332bdc9cb98200cd3a234f8e71d7517e5525f507efe285373f227af49de3`  
		Last Modified: Thu, 17 Aug 2023 01:28:16 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5645b7152fbaf5c18bf624421781149836837a9c5d71f898c771c42234f28384`  
		Last Modified: Thu, 17 Aug 2023 01:28:33 GMT  
		Size: 403.6 MB (403591821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise-ubi8`

```console
$ docker pull neo4j@sha256:b6294fc3448ffe46caa396a1ede70ec01aaca0d8dce75127e302aa4d0fc820a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:58a8bd3a41dfd17b5e331ef13c3885001f18ff8bdf664eda0dcf346a69fa1cf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **585.3 MB (585324104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ebdb04867b6ca5f7cc373d1da99c9438cb0274898485e42187e7cc779f4dce6`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:34 GMT
ADD file:84dff5b0f84a1086a0a07b28849d08a18f2d658869173d376845a20a2cb34541 in / 
# Wed, 03 May 2023 15:11:35 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:35 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:36 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:36 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:36 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:36 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:36 GMT
ENV container oci
# Wed, 03 May 2023 15:11:36 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:36 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:36 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:36 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:37 GMT
ADD file:13e13737bf27853f3a47e1f55b843236868d5521b05c5fed54688856d11bd33f in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:37 GMT
ADD file:fcaeea1e052139bcd93a719356f6d30b0bd66243e25ccb0a8ed0e3b2013b5804 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:37 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:38 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:39 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:40 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 22:58:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:59 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:09 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Wed, 16 Aug 2023 17:02:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3d387334532ff35c6114343fadea68657f0c600665daa5af75fce96c087c6ddc NEO4J_TARBALL=neo4j-enterprise-5.10.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:18 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:02:19 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:02:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.10.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Wed, 16 Aug 2023 17:02:30 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:02:30 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:02:30 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:02:30 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:02:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:02:31 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccd9537bc52f60ded583bf06bc3a05063d4e52cbcd3d48df8c2748d454856e0`  
		Last Modified: Wed, 16 Aug 2023 17:05:18 GMT  
		Size: 144.8 MB (144773734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd322d091d865b89a25ec0a0e720119978c93f4020e1425c4294294088c205`  
		Last Modified: Wed, 16 Aug 2023 17:05:07 GMT  
		Size: 6.5 MB (6535977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7a1b0e8a796e4fb9646cdd687e14fbb293e149037badc1e33966dbec58fb7f`  
		Last Modified: Wed, 16 Aug 2023 17:05:38 GMT  
		Size: 9.3 KB (9346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2b59785d2be424bb71a8a11cfaaef65885f250e3f0c0789e2b87870c827408`  
		Last Modified: Wed, 16 Aug 2023 17:05:56 GMT  
		Size: 394.7 MB (394716003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:5db3cad3d34b4680e70762d88126cb5fb450465fa721b73138170f26c75d9ff5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **587.5 MB (587472173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673c50148db3dd955f7449f7b19d05a324dfeb168fc879f9edf8853a4b138594`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:48 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:48 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:59 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:27:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:27:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:27:01 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:27:01 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:27:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:27:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282ab0089796bc90ec405471494fce4aeb906f83c41d56f4eee5b53f7b7fe7c`  
		Last Modified: Thu, 17 Aug 2023 01:29:22 GMT  
		Size: 9.3 KB (9345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a067445f68579ce62d30a406c181f714a8f6ef4ae77461bbcf681b9ae3709a76`  
		Last Modified: Thu, 17 Aug 2023 01:29:40 GMT  
		Size: 399.9 MB (399892982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:2ea377845b25c84abed770d3be98ea5623f516144d3c5fb2b23d2aa7b16e09f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:d9fcd1c71ea4e113f76510f6ef953e545deba39d2f20baf5da86643db3625a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293694805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548e2d88b9907e17f5ed7ceef2b3d196a0241ebd328082629cdacee40bfa2717`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:01:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:01:13 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:01:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 16 Aug 2023 17:01:14 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:01:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:01:27 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:01:27 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:01:27 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:01:27 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:01:27 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:01:27 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbbcabbc7f08c2176d6fcdda81fb40b452e0264f9210cd51b07cc5a29c8d14`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f078447b9e5feac9152dfd0e26ee1626a52eb32132e7b957429611990fb109`  
		Last Modified: Wed, 16 Aug 2023 17:03:40 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbec5ecbe9f75583c2f1ad50fb132b61bd12cfd93d0dd28a06fb5d8b822e9e81`  
		Last Modified: Wed, 16 Aug 2023 17:03:46 GMT  
		Size: 117.5 MB (117490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:ubi8`

```console
$ docker pull neo4j@sha256:d25e228710b277a03fe7dec31192b77339a7bf8a5b8b6cae8ba08bba23ef3824
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:71e9d964d3efc40f97d0b7b1be84508554794db93b29dba8111b7e9365c39d17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.3 MB (304288700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6fec9a77d8fff42eb6e150b0af89ae0ed70976cb6eeb48dc6e27ec4173fd881`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:34 GMT
ADD file:84dff5b0f84a1086a0a07b28849d08a18f2d658869173d376845a20a2cb34541 in / 
# Wed, 03 May 2023 15:11:35 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:35 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:36 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:36 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:36 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:36 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:36 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:36 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:36 GMT
ENV container oci
# Wed, 03 May 2023 15:11:36 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:36 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:36 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:36 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:37 GMT
ADD file:13e13737bf27853f3a47e1f55b843236868d5521b05c5fed54688856d11bd33f in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:37 GMT
ADD file:fcaeea1e052139bcd93a719356f6d30b0bd66243e25ccb0a8ed0e3b2013b5804 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:37 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:38 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:39 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:40 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 22:58:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:59 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:02:09 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Wed, 16 Aug 2023 17:02:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=2bbf7257481874b0f4b025d0344f81fe972bba1f20fd18e3eb8840ff04ad1b33 NEO4J_TARBALL=neo4j-community-5.10.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 16 Aug 2023 17:02:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
# Wed, 16 Aug 2023 17:02:09 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Wed, 16 Aug 2023 17:02:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.10.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Wed, 16 Aug 2023 17:02:14 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:02:14 GMT
WORKDIR /var/lib/neo4j
# Wed, 16 Aug 2023 17:02:14 GMT
VOLUME [/data /logs]
# Wed, 16 Aug 2023 17:02:14 GMT
EXPOSE 7473 7474 7687
# Wed, 16 Aug 2023 17:02:14 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 17:02:14 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccd9537bc52f60ded583bf06bc3a05063d4e52cbcd3d48df8c2748d454856e0`  
		Last Modified: Wed, 16 Aug 2023 17:05:18 GMT  
		Size: 144.8 MB (144773734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd322d091d865b89a25ec0a0e720119978c93f4020e1425c4294294088c205`  
		Last Modified: Wed, 16 Aug 2023 17:05:07 GMT  
		Size: 6.5 MB (6535977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde16abe682e00a68f584511d44efc49d2d49c02cad218f83cfde87541558447`  
		Last Modified: Wed, 16 Aug 2023 17:05:06 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a705d32035826f6b06be16631ac76d04e427ebe3a6f80b84a1477316f1b27e`  
		Last Modified: Wed, 16 Aug 2023 17:05:13 GMT  
		Size: 113.7 MB (113680595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9e46a4e4523b846c406c8df4a0c5b00f46e012cf5a335a4c56b5abdee56508d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301283576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5583646a630dc67b5478bcf12d494f23d9d3111bee3beea3312d2dd5cdb25595`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 15:11:05 GMT
ADD file:c1449fa3fa5e28681c0d29ba138d06c93ca3be96e038d945ac7d474f9693e797 in / 
# Wed, 03 May 2023 15:11:07 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 03 May 2023 15:11:07 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 03 May 2023 15:11:07 GMT
ADD multi:62a5ed918ba581cb28e63a96c95a2291910a696c57ec0a22b415b43695503828 in /etc/yum.repos.d/ 
# Wed, 03 May 2023 15:11:07 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 03 May 2023 15:11:07 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 03 May 2023 15:11:07 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 03 May 2023 15:11:07 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.expose-services=""
# Wed, 03 May 2023 15:11:07 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 03 May 2023 15:11:07 GMT
ENV container oci
# Wed, 03 May 2023 15:11:07 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 15:11:07 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 15:11:08 GMT
RUN rm -rf /var/log/*
# Wed, 03 May 2023 15:11:08 GMT
LABEL release=860
# Wed, 03 May 2023 15:11:08 GMT
ADD file:a071058fca5391f210272bff5a389267bf1c9383b47b5473dff87949a9ea8630 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-860.json 
# Wed, 03 May 2023 15:11:08 GMT
ADD file:777f5b26862de30ef41c6c5468c53fe0c949b0ac6f03cb717986596bd3afd6d3 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-860 
# Wed, 03 May 2023 15:11:08 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-05-03T15:02:09" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-860"
# Wed, 03 May 2023 15:11:10 GMT
RUN rm -f '/etc/yum.repos.d/repo-700b5.repo' '/etc/yum.repos.d/repo-cb269.repo'
# Wed, 03 May 2023 15:11:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 03 May 2023 15:11:12 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Mon, 24 Jul 2023 21:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:03:36 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:26:42 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 17 Aug 2023 01:26:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:26:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:26:42 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:26:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 17 Aug 2023 01:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:26:46 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:26:46 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:26:46 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08f6a51aabcd289de7b8d70c5289e580719ee3b7d01c0c3df1914d03fd3ebde`  
		Last Modified: Wed, 16 Aug 2023 18:06:42 GMT  
		Size: 143.5 MB (143538102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bf1ec03e85f26ceccbf378dfd7452dcd10cb58982b6090f807edaf5c291eb`  
		Last Modified: Thu, 17 Aug 2023 01:28:56 GMT  
		Size: 6.5 MB (6500304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde3669de5dd9b71b5171db0ea80172e0434dd626fff921721810bdcd4da1abc`  
		Last Modified: Thu, 17 Aug 2023 01:28:55 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af814bcc2ddcf3c718c73ebb2ef5df96d2d0b35e9863c7dbf681ae9d5bae8a67`  
		Last Modified: Thu, 17 Aug 2023 01:29:01 GMT  
		Size: 113.7 MB (113704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
