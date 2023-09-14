<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.25`](#neo4j4425)
-	[`neo4j:4.4.25-community`](#neo4j4425-community)
-	[`neo4j:4.4.25-enterprise`](#neo4j4425-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-bullseye`](#neo4j5-bullseye)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-community-bullseye`](#neo4j5-community-bullseye)
-	[`neo4j:5-community-ubi8`](#neo4j5-community-ubi8)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5-enterprise-bullseye`](#neo4j5-enterprise-bullseye)
-	[`neo4j:5-enterprise-ubi8`](#neo4j5-enterprise-ubi8)
-	[`neo4j:5-ubi8`](#neo4j5-ubi8)
-	[`neo4j:5.12`](#neo4j512)
-	[`neo4j:5.12-bullseye`](#neo4j512-bullseye)
-	[`neo4j:5.12-community`](#neo4j512-community)
-	[`neo4j:5.12-community-bullseye`](#neo4j512-community-bullseye)
-	[`neo4j:5.12-community-ubi8`](#neo4j512-community-ubi8)
-	[`neo4j:5.12-enterprise`](#neo4j512-enterprise)
-	[`neo4j:5.12-enterprise-bullseye`](#neo4j512-enterprise-bullseye)
-	[`neo4j:5.12-enterprise-ubi8`](#neo4j512-enterprise-ubi8)
-	[`neo4j:5.12-ubi8`](#neo4j512-ubi8)
-	[`neo4j:5.12.0`](#neo4j5120)
-	[`neo4j:5.12.0-bullseye`](#neo4j5120-bullseye)
-	[`neo4j:5.12.0-community`](#neo4j5120-community)
-	[`neo4j:5.12.0-community-bullseye`](#neo4j5120-community-bullseye)
-	[`neo4j:5.12.0-community-ubi8`](#neo4j5120-community-ubi8)
-	[`neo4j:5.12.0-enterprise`](#neo4j5120-enterprise)
-	[`neo4j:5.12.0-enterprise-bullseye`](#neo4j5120-enterprise-bullseye)
-	[`neo4j:5.12.0-enterprise-ubi8`](#neo4j5120-enterprise-ubi8)
-	[`neo4j:5.12.0-ubi8`](#neo4j5120-ubi8)
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
$ docker pull neo4j@sha256:0b5690d39d65b3c1cc052e6be8b9cea8f7b4f42664c1c614209fc19313c85b39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:40bb540b859fd057c1d98d52d9080ca697c0c6bc71e648fc7c3002310b284fcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298583225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2eff272a722e9e053cb89a0c5e13316b8d5bbf850a2ab192a30040f7713f8ef`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:04:50 GMT
COPY dir:3e9b1d3d54369337872a2b8aa8c30068d69b28c2def3ec3bf07ba34bd69d48a0 in /opt/java/openjdk 
# Thu, 07 Sep 2023 02:04:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=44d8e1c6af11199478ab8d2be399f8dc7ff819d23ef9983d70b15ae7d9918e26 NEO4J_TARBALL=neo4j-community-4.4.25-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 02:04:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 02:04:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 02:04:52 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 02:05:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:05:04 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 02:05:04 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 02:05:04 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 02:05:05 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 02:05:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 02:05:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc2204a29ef2517e9d39b89552fcfbd45063a2d758626e1aef118a701134c2d`  
		Last Modified: Thu, 07 Sep 2023 02:07:35 GMT  
		Size: 144.8 MB (144826055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb928eb6646105ce8b2c56c4ec3145aefc69178390ead7b5b955ea0a711e3e47`  
		Last Modified: Thu, 07 Sep 2023 02:07:23 GMT  
		Size: 3.9 KB (3853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c21946b77279c799dc11b4acf4f216126880df6f20762d21fbfe4faa776a377`  
		Last Modified: Thu, 07 Sep 2023 02:07:23 GMT  
		Size: 9.3 KB (9290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78897cb3f9a8720845142ade9ed2786746fd0301f699a5823ed3c40dc9e48e`  
		Last Modified: Thu, 07 Sep 2023 02:07:30 GMT  
		Size: 122.3 MB (122326524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7e782a38680d145d5ac900409024b2020975c18b629e90e9fd0c0a000d26af1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.9 MB (293865949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542a823a626617115a4fd79fc5954663561496313da87b455851679292a39dbd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:47:24 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Thu, 07 Sep 2023 06:47:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=44d8e1c6af11199478ab8d2be399f8dc7ff819d23ef9983d70b15ae7d9918e26 NEO4J_TARBALL=neo4j-community-4.4.25-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 06:47:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 06:47:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 06:47:29 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 06:47:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:47:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 06:47:39 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 06:47:39 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 06:47:39 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 06:47:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 06:47:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b018ed6a392610f1ab69e85cc642842b49d22521199586d6067dfd326f17f2`  
		Last Modified: Thu, 07 Sep 2023 06:49:54 GMT  
		Size: 141.6 MB (141570382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54f2dd17ce72dfd3c1ab6a58c660760ff0d92e39efd8a3df9a3f250ab2d0e8f`  
		Last Modified: Thu, 07 Sep 2023 06:49:45 GMT  
		Size: 3.9 KB (3880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603e1f735584d530ca0591fd88a867604558d18c53c5ba8d6c01b894bd1b58f`  
		Last Modified: Thu, 07 Sep 2023 06:49:45 GMT  
		Size: 9.3 KB (9290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6044112ea391c0cdf6eebe77ec76feb5d8c117da48b0764f4ebec842f341bdc`  
		Last Modified: Thu, 07 Sep 2023 06:49:51 GMT  
		Size: 122.2 MB (122219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:0b5690d39d65b3c1cc052e6be8b9cea8f7b4f42664c1c614209fc19313c85b39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:40bb540b859fd057c1d98d52d9080ca697c0c6bc71e648fc7c3002310b284fcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298583225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2eff272a722e9e053cb89a0c5e13316b8d5bbf850a2ab192a30040f7713f8ef`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:04:50 GMT
COPY dir:3e9b1d3d54369337872a2b8aa8c30068d69b28c2def3ec3bf07ba34bd69d48a0 in /opt/java/openjdk 
# Thu, 07 Sep 2023 02:04:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=44d8e1c6af11199478ab8d2be399f8dc7ff819d23ef9983d70b15ae7d9918e26 NEO4J_TARBALL=neo4j-community-4.4.25-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 02:04:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 02:04:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 02:04:52 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 02:05:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:05:04 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 02:05:04 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 02:05:04 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 02:05:05 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 02:05:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 02:05:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc2204a29ef2517e9d39b89552fcfbd45063a2d758626e1aef118a701134c2d`  
		Last Modified: Thu, 07 Sep 2023 02:07:35 GMT  
		Size: 144.8 MB (144826055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb928eb6646105ce8b2c56c4ec3145aefc69178390ead7b5b955ea0a711e3e47`  
		Last Modified: Thu, 07 Sep 2023 02:07:23 GMT  
		Size: 3.9 KB (3853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c21946b77279c799dc11b4acf4f216126880df6f20762d21fbfe4faa776a377`  
		Last Modified: Thu, 07 Sep 2023 02:07:23 GMT  
		Size: 9.3 KB (9290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78897cb3f9a8720845142ade9ed2786746fd0301f699a5823ed3c40dc9e48e`  
		Last Modified: Thu, 07 Sep 2023 02:07:30 GMT  
		Size: 122.3 MB (122326524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7e782a38680d145d5ac900409024b2020975c18b629e90e9fd0c0a000d26af1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.9 MB (293865949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542a823a626617115a4fd79fc5954663561496313da87b455851679292a39dbd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:47:24 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Thu, 07 Sep 2023 06:47:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=44d8e1c6af11199478ab8d2be399f8dc7ff819d23ef9983d70b15ae7d9918e26 NEO4J_TARBALL=neo4j-community-4.4.25-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 06:47:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 06:47:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 06:47:29 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 06:47:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:47:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 06:47:39 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 06:47:39 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 06:47:39 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 06:47:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 06:47:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b018ed6a392610f1ab69e85cc642842b49d22521199586d6067dfd326f17f2`  
		Last Modified: Thu, 07 Sep 2023 06:49:54 GMT  
		Size: 141.6 MB (141570382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54f2dd17ce72dfd3c1ab6a58c660760ff0d92e39efd8a3df9a3f250ab2d0e8f`  
		Last Modified: Thu, 07 Sep 2023 06:49:45 GMT  
		Size: 3.9 KB (3880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603e1f735584d530ca0591fd88a867604558d18c53c5ba8d6c01b894bd1b58f`  
		Last Modified: Thu, 07 Sep 2023 06:49:45 GMT  
		Size: 9.3 KB (9290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6044112ea391c0cdf6eebe77ec76feb5d8c117da48b0764f4ebec842f341bdc`  
		Last Modified: Thu, 07 Sep 2023 06:49:51 GMT  
		Size: 122.2 MB (122219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:078f52f4f8b34dd6a76d0d8c5a5f3fc5dbe9cb48f934dc2abc6d8556c1acfa9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:671fb40f844e65201bcb39a8730729580cf71565ecd3507379a5297a1f196098
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.5 MB (398469243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaae604473e9915a02deed4155fc3bfce523db9332ce6bda243644fb37b67207`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:04:50 GMT
COPY dir:3e9b1d3d54369337872a2b8aa8c30068d69b28c2def3ec3bf07ba34bd69d48a0 in /opt/java/openjdk 
# Thu, 07 Sep 2023 02:05:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c63ccf85c310be093cf030c85618555d75f06fce80239a1a618bd343f5c894aa NEO4J_TARBALL=neo4j-enterprise-4.4.25-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 02:05:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 02:05:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 02:05:09 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 02:05:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:05:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 02:05:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 02:05:26 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 02:05:26 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 02:05:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 02:05:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc2204a29ef2517e9d39b89552fcfbd45063a2d758626e1aef118a701134c2d`  
		Last Modified: Thu, 07 Sep 2023 02:07:35 GMT  
		Size: 144.8 MB (144826055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d693d532955dbd1a39da79540947c1a5d49344ae98a651bf79fe187a240b2`  
		Last Modified: Thu, 07 Sep 2023 02:07:47 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966482d5a012080e948a2a53998504a2556278cbae029882ad5fae10377b481`  
		Last Modified: Thu, 07 Sep 2023 02:07:47 GMT  
		Size: 9.3 KB (9288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302716c8458de53768e5437d25d639dea2257e3e5f616e461f643b786d6f1211`  
		Last Modified: Thu, 07 Sep 2023 02:08:01 GMT  
		Size: 222.2 MB (222212541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f51a87f24a5c375db1d20448d13258551ba31129e2c3e36d0f5c8e669045cec2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.8 MB (393752376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb4decd39b5dad47f49be217938cd46a5204873819e19a60bf50132517017756`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:47:24 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Thu, 07 Sep 2023 06:47:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c63ccf85c310be093cf030c85618555d75f06fce80239a1a618bd343f5c894aa NEO4J_TARBALL=neo4j-enterprise-4.4.25-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 06:47:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 06:47:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 06:47:43 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 06:47:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:47:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 06:47:57 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 06:47:57 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 06:47:57 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 06:47:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 06:47:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b018ed6a392610f1ab69e85cc642842b49d22521199586d6067dfd326f17f2`  
		Last Modified: Thu, 07 Sep 2023 06:49:54 GMT  
		Size: 141.6 MB (141570382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a251b15951da2cc5022e71f6ed78d09b4a7a4039054e58d8bcf52bc49e87d79b`  
		Last Modified: Thu, 07 Sep 2023 06:50:07 GMT  
		Size: 3.9 KB (3882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf3194eacc8873b194ae977bb5e39daef2a0046b4abb62cdbcd74e80f965e2`  
		Last Modified: Thu, 07 Sep 2023 06:50:07 GMT  
		Size: 9.3 KB (9287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c45a8ef1592e3a68f2a16ae8a0d00eb46a25db861146f6be02979fa1d72125`  
		Last Modified: Thu, 07 Sep 2023 06:50:23 GMT  
		Size: 222.1 MB (222105922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.25`

```console
$ docker pull neo4j@sha256:0b5690d39d65b3c1cc052e6be8b9cea8f7b4f42664c1c614209fc19313c85b39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.25` - linux; amd64

```console
$ docker pull neo4j@sha256:40bb540b859fd057c1d98d52d9080ca697c0c6bc71e648fc7c3002310b284fcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298583225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2eff272a722e9e053cb89a0c5e13316b8d5bbf850a2ab192a30040f7713f8ef`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:04:50 GMT
COPY dir:3e9b1d3d54369337872a2b8aa8c30068d69b28c2def3ec3bf07ba34bd69d48a0 in /opt/java/openjdk 
# Thu, 07 Sep 2023 02:04:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=44d8e1c6af11199478ab8d2be399f8dc7ff819d23ef9983d70b15ae7d9918e26 NEO4J_TARBALL=neo4j-community-4.4.25-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 02:04:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 02:04:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 02:04:52 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 02:05:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:05:04 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 02:05:04 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 02:05:04 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 02:05:05 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 02:05:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 02:05:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc2204a29ef2517e9d39b89552fcfbd45063a2d758626e1aef118a701134c2d`  
		Last Modified: Thu, 07 Sep 2023 02:07:35 GMT  
		Size: 144.8 MB (144826055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb928eb6646105ce8b2c56c4ec3145aefc69178390ead7b5b955ea0a711e3e47`  
		Last Modified: Thu, 07 Sep 2023 02:07:23 GMT  
		Size: 3.9 KB (3853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c21946b77279c799dc11b4acf4f216126880df6f20762d21fbfe4faa776a377`  
		Last Modified: Thu, 07 Sep 2023 02:07:23 GMT  
		Size: 9.3 KB (9290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78897cb3f9a8720845142ade9ed2786746fd0301f699a5823ed3c40dc9e48e`  
		Last Modified: Thu, 07 Sep 2023 02:07:30 GMT  
		Size: 122.3 MB (122326524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.25` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7e782a38680d145d5ac900409024b2020975c18b629e90e9fd0c0a000d26af1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.9 MB (293865949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542a823a626617115a4fd79fc5954663561496313da87b455851679292a39dbd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:47:24 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Thu, 07 Sep 2023 06:47:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=44d8e1c6af11199478ab8d2be399f8dc7ff819d23ef9983d70b15ae7d9918e26 NEO4J_TARBALL=neo4j-community-4.4.25-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 06:47:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 06:47:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 06:47:29 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 06:47:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:47:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 06:47:39 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 06:47:39 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 06:47:39 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 06:47:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 06:47:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b018ed6a392610f1ab69e85cc642842b49d22521199586d6067dfd326f17f2`  
		Last Modified: Thu, 07 Sep 2023 06:49:54 GMT  
		Size: 141.6 MB (141570382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54f2dd17ce72dfd3c1ab6a58c660760ff0d92e39efd8a3df9a3f250ab2d0e8f`  
		Last Modified: Thu, 07 Sep 2023 06:49:45 GMT  
		Size: 3.9 KB (3880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603e1f735584d530ca0591fd88a867604558d18c53c5ba8d6c01b894bd1b58f`  
		Last Modified: Thu, 07 Sep 2023 06:49:45 GMT  
		Size: 9.3 KB (9290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6044112ea391c0cdf6eebe77ec76feb5d8c117da48b0764f4ebec842f341bdc`  
		Last Modified: Thu, 07 Sep 2023 06:49:51 GMT  
		Size: 122.2 MB (122219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.25-community`

```console
$ docker pull neo4j@sha256:0b5690d39d65b3c1cc052e6be8b9cea8f7b4f42664c1c614209fc19313c85b39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.25-community` - linux; amd64

```console
$ docker pull neo4j@sha256:40bb540b859fd057c1d98d52d9080ca697c0c6bc71e648fc7c3002310b284fcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298583225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2eff272a722e9e053cb89a0c5e13316b8d5bbf850a2ab192a30040f7713f8ef`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:04:50 GMT
COPY dir:3e9b1d3d54369337872a2b8aa8c30068d69b28c2def3ec3bf07ba34bd69d48a0 in /opt/java/openjdk 
# Thu, 07 Sep 2023 02:04:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=44d8e1c6af11199478ab8d2be399f8dc7ff819d23ef9983d70b15ae7d9918e26 NEO4J_TARBALL=neo4j-community-4.4.25-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 02:04:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 02:04:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 02:04:52 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 02:05:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:05:04 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 02:05:04 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 02:05:04 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 02:05:05 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 02:05:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 02:05:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc2204a29ef2517e9d39b89552fcfbd45063a2d758626e1aef118a701134c2d`  
		Last Modified: Thu, 07 Sep 2023 02:07:35 GMT  
		Size: 144.8 MB (144826055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb928eb6646105ce8b2c56c4ec3145aefc69178390ead7b5b955ea0a711e3e47`  
		Last Modified: Thu, 07 Sep 2023 02:07:23 GMT  
		Size: 3.9 KB (3853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c21946b77279c799dc11b4acf4f216126880df6f20762d21fbfe4faa776a377`  
		Last Modified: Thu, 07 Sep 2023 02:07:23 GMT  
		Size: 9.3 KB (9290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78897cb3f9a8720845142ade9ed2786746fd0301f699a5823ed3c40dc9e48e`  
		Last Modified: Thu, 07 Sep 2023 02:07:30 GMT  
		Size: 122.3 MB (122326524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.25-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7e782a38680d145d5ac900409024b2020975c18b629e90e9fd0c0a000d26af1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.9 MB (293865949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542a823a626617115a4fd79fc5954663561496313da87b455851679292a39dbd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:47:24 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Thu, 07 Sep 2023 06:47:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=44d8e1c6af11199478ab8d2be399f8dc7ff819d23ef9983d70b15ae7d9918e26 NEO4J_TARBALL=neo4j-community-4.4.25-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 06:47:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 06:47:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 06:47:29 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 06:47:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:47:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 06:47:39 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 06:47:39 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 06:47:39 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 06:47:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 06:47:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b018ed6a392610f1ab69e85cc642842b49d22521199586d6067dfd326f17f2`  
		Last Modified: Thu, 07 Sep 2023 06:49:54 GMT  
		Size: 141.6 MB (141570382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54f2dd17ce72dfd3c1ab6a58c660760ff0d92e39efd8a3df9a3f250ab2d0e8f`  
		Last Modified: Thu, 07 Sep 2023 06:49:45 GMT  
		Size: 3.9 KB (3880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603e1f735584d530ca0591fd88a867604558d18c53c5ba8d6c01b894bd1b58f`  
		Last Modified: Thu, 07 Sep 2023 06:49:45 GMT  
		Size: 9.3 KB (9290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6044112ea391c0cdf6eebe77ec76feb5d8c117da48b0764f4ebec842f341bdc`  
		Last Modified: Thu, 07 Sep 2023 06:49:51 GMT  
		Size: 122.2 MB (122219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.25-enterprise`

```console
$ docker pull neo4j@sha256:078f52f4f8b34dd6a76d0d8c5a5f3fc5dbe9cb48f934dc2abc6d8556c1acfa9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.25-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:671fb40f844e65201bcb39a8730729580cf71565ecd3507379a5297a1f196098
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.5 MB (398469243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaae604473e9915a02deed4155fc3bfce523db9332ce6bda243644fb37b67207`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:04:50 GMT
COPY dir:3e9b1d3d54369337872a2b8aa8c30068d69b28c2def3ec3bf07ba34bd69d48a0 in /opt/java/openjdk 
# Thu, 07 Sep 2023 02:05:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c63ccf85c310be093cf030c85618555d75f06fce80239a1a618bd343f5c894aa NEO4J_TARBALL=neo4j-enterprise-4.4.25-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 02:05:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 02:05:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 02:05:09 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 02:05:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:05:25 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 02:05:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 02:05:26 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 02:05:26 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 02:05:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 02:05:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc2204a29ef2517e9d39b89552fcfbd45063a2d758626e1aef118a701134c2d`  
		Last Modified: Thu, 07 Sep 2023 02:07:35 GMT  
		Size: 144.8 MB (144826055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d693d532955dbd1a39da79540947c1a5d49344ae98a651bf79fe187a240b2`  
		Last Modified: Thu, 07 Sep 2023 02:07:47 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966482d5a012080e948a2a53998504a2556278cbae029882ad5fae10377b481`  
		Last Modified: Thu, 07 Sep 2023 02:07:47 GMT  
		Size: 9.3 KB (9288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302716c8458de53768e5437d25d639dea2257e3e5f616e461f643b786d6f1211`  
		Last Modified: Thu, 07 Sep 2023 02:08:01 GMT  
		Size: 222.2 MB (222212541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.25-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f51a87f24a5c375db1d20448d13258551ba31129e2c3e36d0f5c8e669045cec2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.8 MB (393752376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb4decd39b5dad47f49be217938cd46a5204873819e19a60bf50132517017756`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:47:24 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Thu, 07 Sep 2023 06:47:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c63ccf85c310be093cf030c85618555d75f06fce80239a1a618bd343f5c894aa NEO4J_TARBALL=neo4j-enterprise-4.4.25-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 07 Sep 2023 06:47:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
# Thu, 07 Sep 2023 06:47:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 07 Sep 2023 06:47:43 GMT
COPY multi:b4e555cf4a865db7ac955e204b7d9f288c4ba077e688882dbe94074bda1d191e in /startup/ 
# Thu, 07 Sep 2023 06:47:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.25-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:47:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 06:47:57 GMT
WORKDIR /var/lib/neo4j
# Thu, 07 Sep 2023 06:47:57 GMT
VOLUME [/data /logs]
# Thu, 07 Sep 2023 06:47:57 GMT
EXPOSE 7473 7474 7687
# Thu, 07 Sep 2023 06:47:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 06:47:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b018ed6a392610f1ab69e85cc642842b49d22521199586d6067dfd326f17f2`  
		Last Modified: Thu, 07 Sep 2023 06:49:54 GMT  
		Size: 141.6 MB (141570382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a251b15951da2cc5022e71f6ed78d09b4a7a4039054e58d8bcf52bc49e87d79b`  
		Last Modified: Thu, 07 Sep 2023 06:50:07 GMT  
		Size: 3.9 KB (3882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf3194eacc8873b194ae977bb5e39daef2a0046b4abb62cdbcd74e80f965e2`  
		Last Modified: Thu, 07 Sep 2023 06:50:07 GMT  
		Size: 9.3 KB (9287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c45a8ef1592e3a68f2a16ae8a0d00eb46a25db861146f6be02979fa1d72125`  
		Last Modified: Thu, 07 Sep 2023 06:50:23 GMT  
		Size: 222.1 MB (222105922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-bullseye`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community-bullseye`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community-ubi8`

```console
$ docker pull neo4j@sha256:d29478ad98405ad06087f23c8f2049aa036c3a8777c84b20ac17f8940822724c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:fdf7a80bc7dd807fdafbb2364cd0921827e3fcd2b6fab38dbbbadbc3ddefc321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303257353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5823c5426f54a894f9cdfc79c17b356ed9d056ab56a4ec9f256064a9ad8bac`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:20:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:54 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:20:58 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:58 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:58 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:58 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919fe744d5f603d87da82bdadbc5d011fdf5adf4910cedf6b9e9588e46dffa6e`  
		Last Modified: Thu, 14 Sep 2023 21:23:26 GMT  
		Size: 9.4 KB (9429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88653088570193201dc09d69eb4938fbcc51c7ad2e0459a0b61a57f1695f5aab`  
		Last Modified: Thu, 14 Sep 2023 21:23:32 GMT  
		Size: 112.7 MB (112652971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:15f58472ef484515f428bacf3e5a699d38eecfcdcbcc6afba7004c8e0f12f703
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300234017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4778c2d781e075ce6f1482ad7142533eade8221941fb898a9dc441a1814597fb`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:52 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:42:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:56 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:56 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:56 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6618326ab8e89e417d1e87239720ea529da8606c89719f7594bda95e3e2a3618`  
		Last Modified: Thu, 14 Sep 2023 21:45:15 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f793dea39a11763e145f397c62687392563260fd1e0bc27e5c26019f3cba18`  
		Last Modified: Thu, 14 Sep 2023 21:45:22 GMT  
		Size: 112.7 MB (112652999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:cb917c096c02edd439f8bcf2f7ac9d0ef6de23e8096bad897dd5b553f16edb9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:37e94cbc52075a434ef9d11e1d86b4eef0a03b7cf8a43963fac914ca64303a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566221125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14efaaa0dcf39596de84809a9a769495167941a321d12738a1f1f78649b558c9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:30 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:49 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:49 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:49 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:49 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71d426758301d4947dbba8ab34ead273c10ea4100981e4f1460588860669e`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4531025ff8adeffd13a3498a6ceaaddba41a242c0328f7255d5cadd87a2bed20`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e631f80eed66d3942de8684d3d44c24edb3f45fe6b4fe1a97ad223ef6c01dc`  
		Last Modified: Thu, 14 Sep 2023 21:23:00 GMT  
		Size: 390.0 MB (390014534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66c52877d1c5dd44ff660f38ac3c69a1673f6b4ddfe09bfb7585f3a233c2776a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.5 MB (563527053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c1878f67b3347aae5ddce87ef592cc09ee8d7e9cb07cd3b7e02f24d60e5996`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:29 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:48 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:48 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4068aad1006a13ed4cb11dd7c97f7ab4bdc215428ddb26e71e2684180dc14e63`  
		Last Modified: Thu, 14 Sep 2023 21:44:28 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff12171a6ca712702966999243525fdf8b5017b189b180c90b0dfc057f4cec44`  
		Last Modified: Thu, 14 Sep 2023 21:44:29 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9dd7247e936b62300eaf14a21de67d4abe159907e803c76c7a12d69c69100`  
		Last Modified: Thu, 14 Sep 2023 21:44:52 GMT  
		Size: 389.9 MB (389907339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:cb917c096c02edd439f8bcf2f7ac9d0ef6de23e8096bad897dd5b553f16edb9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:37e94cbc52075a434ef9d11e1d86b4eef0a03b7cf8a43963fac914ca64303a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566221125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14efaaa0dcf39596de84809a9a769495167941a321d12738a1f1f78649b558c9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:30 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:49 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:49 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:49 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:49 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71d426758301d4947dbba8ab34ead273c10ea4100981e4f1460588860669e`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4531025ff8adeffd13a3498a6ceaaddba41a242c0328f7255d5cadd87a2bed20`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e631f80eed66d3942de8684d3d44c24edb3f45fe6b4fe1a97ad223ef6c01dc`  
		Last Modified: Thu, 14 Sep 2023 21:23:00 GMT  
		Size: 390.0 MB (390014534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66c52877d1c5dd44ff660f38ac3c69a1673f6b4ddfe09bfb7585f3a233c2776a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.5 MB (563527053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c1878f67b3347aae5ddce87ef592cc09ee8d7e9cb07cd3b7e02f24d60e5996`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:29 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:48 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:48 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4068aad1006a13ed4cb11dd7c97f7ab4bdc215428ddb26e71e2684180dc14e63`  
		Last Modified: Thu, 14 Sep 2023 21:44:28 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff12171a6ca712702966999243525fdf8b5017b189b180c90b0dfc057f4cec44`  
		Last Modified: Thu, 14 Sep 2023 21:44:29 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9dd7247e936b62300eaf14a21de67d4abe159907e803c76c7a12d69c69100`  
		Last Modified: Thu, 14 Sep 2023 21:44:52 GMT  
		Size: 389.9 MB (389907339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:dcc0128f2c74f695ac160de2a63a0796f34815ece63f2268e9586751c08c919d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:acb00e347a8b0c23829dc223ae4c21110d3f9bb88a995de5ee8ca79163ba1939
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576806555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3632616d479662517387da2cd8693d4bd3290cf22e7378510a6a9a49287ef7e6`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:21:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:21:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:21:01 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:21:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:21:13 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:21:13 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:21:13 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:21:13 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:21:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:21:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905c1a9914702e1ded4d179bcea6480d8823ff87610c2b611a481fb85ed91a65`  
		Last Modified: Thu, 14 Sep 2023 21:23:53 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3810440fad8ae2bed5c6b23c938c9fcfeda80b1567c6891f67eb17acafce18c`  
		Last Modified: Thu, 14 Sep 2023 21:24:15 GMT  
		Size: 386.2 MB (386202177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:799ada3cfba426348323addaf3cf49a0410ef51963d2eb0dec3b5e15f7874978
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.8 MB (573783139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fec4ceb3eee5a2a126c101865623c5cc6c8106f9b8a193a5615d476195f9424`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:59 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:43:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:43:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:43:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:43:10 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:43:11 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:43:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:43:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34b095071b2b485881518e679e60de2195359bfe6ecc186294d96d68308a157`  
		Last Modified: Thu, 14 Sep 2023 21:45:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca560ea4398cc72428516cda7e657937a516ecfa36d9941d0bf4331150cfba6`  
		Last Modified: Thu, 14 Sep 2023 21:46:02 GMT  
		Size: 386.2 MB (386202117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-ubi8`

```console
$ docker pull neo4j@sha256:d29478ad98405ad06087f23c8f2049aa036c3a8777c84b20ac17f8940822724c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:fdf7a80bc7dd807fdafbb2364cd0921827e3fcd2b6fab38dbbbadbc3ddefc321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303257353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5823c5426f54a894f9cdfc79c17b356ed9d056ab56a4ec9f256064a9ad8bac`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:20:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:54 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:20:58 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:58 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:58 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:58 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919fe744d5f603d87da82bdadbc5d011fdf5adf4910cedf6b9e9588e46dffa6e`  
		Last Modified: Thu, 14 Sep 2023 21:23:26 GMT  
		Size: 9.4 KB (9429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88653088570193201dc09d69eb4938fbcc51c7ad2e0459a0b61a57f1695f5aab`  
		Last Modified: Thu, 14 Sep 2023 21:23:32 GMT  
		Size: 112.7 MB (112652971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:15f58472ef484515f428bacf3e5a699d38eecfcdcbcc6afba7004c8e0f12f703
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300234017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4778c2d781e075ce6f1482ad7142533eade8221941fb898a9dc441a1814597fb`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:52 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:42:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:56 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:56 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:56 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6618326ab8e89e417d1e87239720ea529da8606c89719f7594bda95e3e2a3618`  
		Last Modified: Thu, 14 Sep 2023 21:45:15 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f793dea39a11763e145f397c62687392563260fd1e0bc27e5c26019f3cba18`  
		Last Modified: Thu, 14 Sep 2023 21:45:22 GMT  
		Size: 112.7 MB (112652999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12-bullseye`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12-community`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12-community` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12-community-bullseye`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12-community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12-community-ubi8`

```console
$ docker pull neo4j@sha256:d29478ad98405ad06087f23c8f2049aa036c3a8777c84b20ac17f8940822724c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12-community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:fdf7a80bc7dd807fdafbb2364cd0921827e3fcd2b6fab38dbbbadbc3ddefc321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303257353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5823c5426f54a894f9cdfc79c17b356ed9d056ab56a4ec9f256064a9ad8bac`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:20:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:54 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:20:58 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:58 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:58 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:58 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919fe744d5f603d87da82bdadbc5d011fdf5adf4910cedf6b9e9588e46dffa6e`  
		Last Modified: Thu, 14 Sep 2023 21:23:26 GMT  
		Size: 9.4 KB (9429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88653088570193201dc09d69eb4938fbcc51c7ad2e0459a0b61a57f1695f5aab`  
		Last Modified: Thu, 14 Sep 2023 21:23:32 GMT  
		Size: 112.7 MB (112652971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:15f58472ef484515f428bacf3e5a699d38eecfcdcbcc6afba7004c8e0f12f703
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300234017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4778c2d781e075ce6f1482ad7142533eade8221941fb898a9dc441a1814597fb`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:52 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:42:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:56 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:56 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:56 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6618326ab8e89e417d1e87239720ea529da8606c89719f7594bda95e3e2a3618`  
		Last Modified: Thu, 14 Sep 2023 21:45:15 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f793dea39a11763e145f397c62687392563260fd1e0bc27e5c26019f3cba18`  
		Last Modified: Thu, 14 Sep 2023 21:45:22 GMT  
		Size: 112.7 MB (112652999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12-enterprise`

```console
$ docker pull neo4j@sha256:cb917c096c02edd439f8bcf2f7ac9d0ef6de23e8096bad897dd5b553f16edb9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:37e94cbc52075a434ef9d11e1d86b4eef0a03b7cf8a43963fac914ca64303a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566221125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14efaaa0dcf39596de84809a9a769495167941a321d12738a1f1f78649b558c9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:30 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:49 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:49 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:49 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:49 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71d426758301d4947dbba8ab34ead273c10ea4100981e4f1460588860669e`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4531025ff8adeffd13a3498a6ceaaddba41a242c0328f7255d5cadd87a2bed20`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e631f80eed66d3942de8684d3d44c24edb3f45fe6b4fe1a97ad223ef6c01dc`  
		Last Modified: Thu, 14 Sep 2023 21:23:00 GMT  
		Size: 390.0 MB (390014534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66c52877d1c5dd44ff660f38ac3c69a1673f6b4ddfe09bfb7585f3a233c2776a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.5 MB (563527053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c1878f67b3347aae5ddce87ef592cc09ee8d7e9cb07cd3b7e02f24d60e5996`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:29 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:48 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:48 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4068aad1006a13ed4cb11dd7c97f7ab4bdc215428ddb26e71e2684180dc14e63`  
		Last Modified: Thu, 14 Sep 2023 21:44:28 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff12171a6ca712702966999243525fdf8b5017b189b180c90b0dfc057f4cec44`  
		Last Modified: Thu, 14 Sep 2023 21:44:29 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9dd7247e936b62300eaf14a21de67d4abe159907e803c76c7a12d69c69100`  
		Last Modified: Thu, 14 Sep 2023 21:44:52 GMT  
		Size: 389.9 MB (389907339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:cb917c096c02edd439f8bcf2f7ac9d0ef6de23e8096bad897dd5b553f16edb9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:37e94cbc52075a434ef9d11e1d86b4eef0a03b7cf8a43963fac914ca64303a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566221125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14efaaa0dcf39596de84809a9a769495167941a321d12738a1f1f78649b558c9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:30 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:49 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:49 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:49 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:49 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71d426758301d4947dbba8ab34ead273c10ea4100981e4f1460588860669e`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4531025ff8adeffd13a3498a6ceaaddba41a242c0328f7255d5cadd87a2bed20`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e631f80eed66d3942de8684d3d44c24edb3f45fe6b4fe1a97ad223ef6c01dc`  
		Last Modified: Thu, 14 Sep 2023 21:23:00 GMT  
		Size: 390.0 MB (390014534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66c52877d1c5dd44ff660f38ac3c69a1673f6b4ddfe09bfb7585f3a233c2776a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.5 MB (563527053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c1878f67b3347aae5ddce87ef592cc09ee8d7e9cb07cd3b7e02f24d60e5996`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:29 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:48 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:48 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4068aad1006a13ed4cb11dd7c97f7ab4bdc215428ddb26e71e2684180dc14e63`  
		Last Modified: Thu, 14 Sep 2023 21:44:28 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff12171a6ca712702966999243525fdf8b5017b189b180c90b0dfc057f4cec44`  
		Last Modified: Thu, 14 Sep 2023 21:44:29 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9dd7247e936b62300eaf14a21de67d4abe159907e803c76c7a12d69c69100`  
		Last Modified: Thu, 14 Sep 2023 21:44:52 GMT  
		Size: 389.9 MB (389907339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:dcc0128f2c74f695ac160de2a63a0796f34815ece63f2268e9586751c08c919d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12-enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:acb00e347a8b0c23829dc223ae4c21110d3f9bb88a995de5ee8ca79163ba1939
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576806555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3632616d479662517387da2cd8693d4bd3290cf22e7378510a6a9a49287ef7e6`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:21:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:21:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:21:01 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:21:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:21:13 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:21:13 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:21:13 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:21:13 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:21:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:21:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905c1a9914702e1ded4d179bcea6480d8823ff87610c2b611a481fb85ed91a65`  
		Last Modified: Thu, 14 Sep 2023 21:23:53 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3810440fad8ae2bed5c6b23c938c9fcfeda80b1567c6891f67eb17acafce18c`  
		Last Modified: Thu, 14 Sep 2023 21:24:15 GMT  
		Size: 386.2 MB (386202177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12-enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:799ada3cfba426348323addaf3cf49a0410ef51963d2eb0dec3b5e15f7874978
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.8 MB (573783139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fec4ceb3eee5a2a126c101865623c5cc6c8106f9b8a193a5615d476195f9424`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:59 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:43:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:43:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:43:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:43:10 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:43:11 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:43:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:43:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34b095071b2b485881518e679e60de2195359bfe6ecc186294d96d68308a157`  
		Last Modified: Thu, 14 Sep 2023 21:45:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca560ea4398cc72428516cda7e657937a516ecfa36d9941d0bf4331150cfba6`  
		Last Modified: Thu, 14 Sep 2023 21:46:02 GMT  
		Size: 386.2 MB (386202117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12-ubi8`

```console
$ docker pull neo4j@sha256:d29478ad98405ad06087f23c8f2049aa036c3a8777c84b20ac17f8940822724c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:fdf7a80bc7dd807fdafbb2364cd0921827e3fcd2b6fab38dbbbadbc3ddefc321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303257353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5823c5426f54a894f9cdfc79c17b356ed9d056ab56a4ec9f256064a9ad8bac`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:20:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:54 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:20:58 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:58 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:58 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:58 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919fe744d5f603d87da82bdadbc5d011fdf5adf4910cedf6b9e9588e46dffa6e`  
		Last Modified: Thu, 14 Sep 2023 21:23:26 GMT  
		Size: 9.4 KB (9429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88653088570193201dc09d69eb4938fbcc51c7ad2e0459a0b61a57f1695f5aab`  
		Last Modified: Thu, 14 Sep 2023 21:23:32 GMT  
		Size: 112.7 MB (112652971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:15f58472ef484515f428bacf3e5a699d38eecfcdcbcc6afba7004c8e0f12f703
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300234017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4778c2d781e075ce6f1482ad7142533eade8221941fb898a9dc441a1814597fb`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:52 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:42:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:56 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:56 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:56 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6618326ab8e89e417d1e87239720ea529da8606c89719f7594bda95e3e2a3618`  
		Last Modified: Thu, 14 Sep 2023 21:45:15 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f793dea39a11763e145f397c62687392563260fd1e0bc27e5c26019f3cba18`  
		Last Modified: Thu, 14 Sep 2023 21:45:22 GMT  
		Size: 112.7 MB (112652999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12.0`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12.0` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12.0-bullseye`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12.0-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12.0-community`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12.0-community-bullseye`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12.0-community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12.0-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12.0-community-ubi8`

```console
$ docker pull neo4j@sha256:d29478ad98405ad06087f23c8f2049aa036c3a8777c84b20ac17f8940822724c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12.0-community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:fdf7a80bc7dd807fdafbb2364cd0921827e3fcd2b6fab38dbbbadbc3ddefc321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303257353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5823c5426f54a894f9cdfc79c17b356ed9d056ab56a4ec9f256064a9ad8bac`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:20:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:54 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:20:58 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:58 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:58 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:58 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919fe744d5f603d87da82bdadbc5d011fdf5adf4910cedf6b9e9588e46dffa6e`  
		Last Modified: Thu, 14 Sep 2023 21:23:26 GMT  
		Size: 9.4 KB (9429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88653088570193201dc09d69eb4938fbcc51c7ad2e0459a0b61a57f1695f5aab`  
		Last Modified: Thu, 14 Sep 2023 21:23:32 GMT  
		Size: 112.7 MB (112652971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12.0-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:15f58472ef484515f428bacf3e5a699d38eecfcdcbcc6afba7004c8e0f12f703
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300234017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4778c2d781e075ce6f1482ad7142533eade8221941fb898a9dc441a1814597fb`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:52 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:42:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:56 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:56 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:56 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6618326ab8e89e417d1e87239720ea529da8606c89719f7594bda95e3e2a3618`  
		Last Modified: Thu, 14 Sep 2023 21:45:15 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f793dea39a11763e145f397c62687392563260fd1e0bc27e5c26019f3cba18`  
		Last Modified: Thu, 14 Sep 2023 21:45:22 GMT  
		Size: 112.7 MB (112652999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12.0-enterprise`

```console
$ docker pull neo4j@sha256:cb917c096c02edd439f8bcf2f7ac9d0ef6de23e8096bad897dd5b553f16edb9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:37e94cbc52075a434ef9d11e1d86b4eef0a03b7cf8a43963fac914ca64303a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566221125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14efaaa0dcf39596de84809a9a769495167941a321d12738a1f1f78649b558c9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:30 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:49 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:49 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:49 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:49 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71d426758301d4947dbba8ab34ead273c10ea4100981e4f1460588860669e`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4531025ff8adeffd13a3498a6ceaaddba41a242c0328f7255d5cadd87a2bed20`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e631f80eed66d3942de8684d3d44c24edb3f45fe6b4fe1a97ad223ef6c01dc`  
		Last Modified: Thu, 14 Sep 2023 21:23:00 GMT  
		Size: 390.0 MB (390014534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66c52877d1c5dd44ff660f38ac3c69a1673f6b4ddfe09bfb7585f3a233c2776a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.5 MB (563527053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c1878f67b3347aae5ddce87ef592cc09ee8d7e9cb07cd3b7e02f24d60e5996`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:29 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:48 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:48 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4068aad1006a13ed4cb11dd7c97f7ab4bdc215428ddb26e71e2684180dc14e63`  
		Last Modified: Thu, 14 Sep 2023 21:44:28 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff12171a6ca712702966999243525fdf8b5017b189b180c90b0dfc057f4cec44`  
		Last Modified: Thu, 14 Sep 2023 21:44:29 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9dd7247e936b62300eaf14a21de67d4abe159907e803c76c7a12d69c69100`  
		Last Modified: Thu, 14 Sep 2023 21:44:52 GMT  
		Size: 389.9 MB (389907339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12.0-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:cb917c096c02edd439f8bcf2f7ac9d0ef6de23e8096bad897dd5b553f16edb9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12.0-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:37e94cbc52075a434ef9d11e1d86b4eef0a03b7cf8a43963fac914ca64303a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566221125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14efaaa0dcf39596de84809a9a769495167941a321d12738a1f1f78649b558c9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:30 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:49 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:49 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:49 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:49 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71d426758301d4947dbba8ab34ead273c10ea4100981e4f1460588860669e`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4531025ff8adeffd13a3498a6ceaaddba41a242c0328f7255d5cadd87a2bed20`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e631f80eed66d3942de8684d3d44c24edb3f45fe6b4fe1a97ad223ef6c01dc`  
		Last Modified: Thu, 14 Sep 2023 21:23:00 GMT  
		Size: 390.0 MB (390014534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12.0-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66c52877d1c5dd44ff660f38ac3c69a1673f6b4ddfe09bfb7585f3a233c2776a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.5 MB (563527053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c1878f67b3347aae5ddce87ef592cc09ee8d7e9cb07cd3b7e02f24d60e5996`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:29 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:48 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:48 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4068aad1006a13ed4cb11dd7c97f7ab4bdc215428ddb26e71e2684180dc14e63`  
		Last Modified: Thu, 14 Sep 2023 21:44:28 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff12171a6ca712702966999243525fdf8b5017b189b180c90b0dfc057f4cec44`  
		Last Modified: Thu, 14 Sep 2023 21:44:29 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9dd7247e936b62300eaf14a21de67d4abe159907e803c76c7a12d69c69100`  
		Last Modified: Thu, 14 Sep 2023 21:44:52 GMT  
		Size: 389.9 MB (389907339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12.0-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:dcc0128f2c74f695ac160de2a63a0796f34815ece63f2268e9586751c08c919d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12.0-enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:acb00e347a8b0c23829dc223ae4c21110d3f9bb88a995de5ee8ca79163ba1939
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576806555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3632616d479662517387da2cd8693d4bd3290cf22e7378510a6a9a49287ef7e6`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:21:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:21:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:21:01 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:21:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:21:13 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:21:13 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:21:13 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:21:13 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:21:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:21:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905c1a9914702e1ded4d179bcea6480d8823ff87610c2b611a481fb85ed91a65`  
		Last Modified: Thu, 14 Sep 2023 21:23:53 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3810440fad8ae2bed5c6b23c938c9fcfeda80b1567c6891f67eb17acafce18c`  
		Last Modified: Thu, 14 Sep 2023 21:24:15 GMT  
		Size: 386.2 MB (386202177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12.0-enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:799ada3cfba426348323addaf3cf49a0410ef51963d2eb0dec3b5e15f7874978
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.8 MB (573783139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fec4ceb3eee5a2a126c101865623c5cc6c8106f9b8a193a5615d476195f9424`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:59 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:43:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:43:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:43:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:43:10 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:43:11 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:43:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:43:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34b095071b2b485881518e679e60de2195359bfe6ecc186294d96d68308a157`  
		Last Modified: Thu, 14 Sep 2023 21:45:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca560ea4398cc72428516cda7e657937a516ecfa36d9941d0bf4331150cfba6`  
		Last Modified: Thu, 14 Sep 2023 21:46:02 GMT  
		Size: 386.2 MB (386202117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.12.0-ubi8`

```console
$ docker pull neo4j@sha256:d29478ad98405ad06087f23c8f2049aa036c3a8777c84b20ac17f8940822724c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.12.0-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:fdf7a80bc7dd807fdafbb2364cd0921827e3fcd2b6fab38dbbbadbc3ddefc321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303257353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5823c5426f54a894f9cdfc79c17b356ed9d056ab56a4ec9f256064a9ad8bac`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:20:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:54 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:20:58 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:58 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:58 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:58 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919fe744d5f603d87da82bdadbc5d011fdf5adf4910cedf6b9e9588e46dffa6e`  
		Last Modified: Thu, 14 Sep 2023 21:23:26 GMT  
		Size: 9.4 KB (9429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88653088570193201dc09d69eb4938fbcc51c7ad2e0459a0b61a57f1695f5aab`  
		Last Modified: Thu, 14 Sep 2023 21:23:32 GMT  
		Size: 112.7 MB (112652971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.12.0-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:15f58472ef484515f428bacf3e5a699d38eecfcdcbcc6afba7004c8e0f12f703
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300234017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4778c2d781e075ce6f1482ad7142533eade8221941fb898a9dc441a1814597fb`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:52 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:42:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:56 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:56 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:56 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6618326ab8e89e417d1e87239720ea529da8606c89719f7594bda95e3e2a3618`  
		Last Modified: Thu, 14 Sep 2023 21:45:15 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f793dea39a11763e145f397c62687392563260fd1e0bc27e5c26019f3cba18`  
		Last Modified: Thu, 14 Sep 2023 21:45:22 GMT  
		Size: 112.7 MB (112652999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:bullseye`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community-bullseye`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community-ubi8`

```console
$ docker pull neo4j@sha256:d29478ad98405ad06087f23c8f2049aa036c3a8777c84b20ac17f8940822724c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:fdf7a80bc7dd807fdafbb2364cd0921827e3fcd2b6fab38dbbbadbc3ddefc321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303257353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5823c5426f54a894f9cdfc79c17b356ed9d056ab56a4ec9f256064a9ad8bac`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:20:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:54 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:20:58 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:58 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:58 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:58 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919fe744d5f603d87da82bdadbc5d011fdf5adf4910cedf6b9e9588e46dffa6e`  
		Last Modified: Thu, 14 Sep 2023 21:23:26 GMT  
		Size: 9.4 KB (9429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88653088570193201dc09d69eb4938fbcc51c7ad2e0459a0b61a57f1695f5aab`  
		Last Modified: Thu, 14 Sep 2023 21:23:32 GMT  
		Size: 112.7 MB (112652971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:15f58472ef484515f428bacf3e5a699d38eecfcdcbcc6afba7004c8e0f12f703
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300234017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4778c2d781e075ce6f1482ad7142533eade8221941fb898a9dc441a1814597fb`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:52 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:42:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:56 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:56 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:56 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6618326ab8e89e417d1e87239720ea529da8606c89719f7594bda95e3e2a3618`  
		Last Modified: Thu, 14 Sep 2023 21:45:15 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f793dea39a11763e145f397c62687392563260fd1e0bc27e5c26019f3cba18`  
		Last Modified: Thu, 14 Sep 2023 21:45:22 GMT  
		Size: 112.7 MB (112652999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:cb917c096c02edd439f8bcf2f7ac9d0ef6de23e8096bad897dd5b553f16edb9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:37e94cbc52075a434ef9d11e1d86b4eef0a03b7cf8a43963fac914ca64303a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566221125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14efaaa0dcf39596de84809a9a769495167941a321d12738a1f1f78649b558c9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:30 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:49 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:49 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:49 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:49 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71d426758301d4947dbba8ab34ead273c10ea4100981e4f1460588860669e`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4531025ff8adeffd13a3498a6ceaaddba41a242c0328f7255d5cadd87a2bed20`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e631f80eed66d3942de8684d3d44c24edb3f45fe6b4fe1a97ad223ef6c01dc`  
		Last Modified: Thu, 14 Sep 2023 21:23:00 GMT  
		Size: 390.0 MB (390014534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66c52877d1c5dd44ff660f38ac3c69a1673f6b4ddfe09bfb7585f3a233c2776a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.5 MB (563527053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c1878f67b3347aae5ddce87ef592cc09ee8d7e9cb07cd3b7e02f24d60e5996`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:29 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:48 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:48 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4068aad1006a13ed4cb11dd7c97f7ab4bdc215428ddb26e71e2684180dc14e63`  
		Last Modified: Thu, 14 Sep 2023 21:44:28 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff12171a6ca712702966999243525fdf8b5017b189b180c90b0dfc057f4cec44`  
		Last Modified: Thu, 14 Sep 2023 21:44:29 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9dd7247e936b62300eaf14a21de67d4abe159907e803c76c7a12d69c69100`  
		Last Modified: Thu, 14 Sep 2023 21:44:52 GMT  
		Size: 389.9 MB (389907339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise-bullseye`

```console
$ docker pull neo4j@sha256:cb917c096c02edd439f8bcf2f7ac9d0ef6de23e8096bad897dd5b553f16edb9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:37e94cbc52075a434ef9d11e1d86b4eef0a03b7cf8a43963fac914ca64303a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566221125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14efaaa0dcf39596de84809a9a769495167941a321d12738a1f1f78649b558c9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:30 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:49 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:49 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:49 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:49 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71d426758301d4947dbba8ab34ead273c10ea4100981e4f1460588860669e`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4531025ff8adeffd13a3498a6ceaaddba41a242c0328f7255d5cadd87a2bed20`  
		Last Modified: Thu, 14 Sep 2023 21:22:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e631f80eed66d3942de8684d3d44c24edb3f45fe6b4fe1a97ad223ef6c01dc`  
		Last Modified: Thu, 14 Sep 2023 21:23:00 GMT  
		Size: 390.0 MB (390014534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:66c52877d1c5dd44ff660f38ac3c69a1673f6b4ddfe09bfb7585f3a233c2776a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.5 MB (563527053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c1878f67b3347aae5ddce87ef592cc09ee8d7e9cb07cd3b7e02f24d60e5996`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:29 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:48 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:48 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4068aad1006a13ed4cb11dd7c97f7ab4bdc215428ddb26e71e2684180dc14e63`  
		Last Modified: Thu, 14 Sep 2023 21:44:28 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff12171a6ca712702966999243525fdf8b5017b189b180c90b0dfc057f4cec44`  
		Last Modified: Thu, 14 Sep 2023 21:44:29 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9dd7247e936b62300eaf14a21de67d4abe159907e803c76c7a12d69c69100`  
		Last Modified: Thu, 14 Sep 2023 21:44:52 GMT  
		Size: 389.9 MB (389907339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise-ubi8`

```console
$ docker pull neo4j@sha256:dcc0128f2c74f695ac160de2a63a0796f34815ece63f2268e9586751c08c919d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:acb00e347a8b0c23829dc223ae4c21110d3f9bb88a995de5ee8ca79163ba1939
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576806555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3632616d479662517387da2cd8693d4bd3290cf22e7378510a6a9a49287ef7e6`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:21:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:21:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:21:01 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:21:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:21:13 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:21:13 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:21:13 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:21:13 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:21:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:21:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905c1a9914702e1ded4d179bcea6480d8823ff87610c2b611a481fb85ed91a65`  
		Last Modified: Thu, 14 Sep 2023 21:23:53 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3810440fad8ae2bed5c6b23c938c9fcfeda80b1567c6891f67eb17acafce18c`  
		Last Modified: Thu, 14 Sep 2023 21:24:15 GMT  
		Size: 386.2 MB (386202177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:799ada3cfba426348323addaf3cf49a0410ef51963d2eb0dec3b5e15f7874978
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.8 MB (573783139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fec4ceb3eee5a2a126c101865623c5cc6c8106f9b8a193a5615d476195f9424`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=282c8601cbcc04fc49dfefec305c1f3d824ba2cd16ea3d30721051bfcea05239 NEO4J_TARBALL=neo4j-enterprise-5.12.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:59 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:43:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:43:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:43:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:43:10 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:43:11 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:43:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:43:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34b095071b2b485881518e679e60de2195359bfe6ecc186294d96d68308a157`  
		Last Modified: Thu, 14 Sep 2023 21:45:43 GMT  
		Size: 9.4 KB (9431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca560ea4398cc72428516cda7e657937a516ecfa36d9941d0bf4331150cfba6`  
		Last Modified: Thu, 14 Sep 2023 21:46:02 GMT  
		Size: 386.2 MB (386202117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:9cec926c48209ba106e6c9eeb6454112c5d8f1b4ff5067bf2a75cb162b7514c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:dc497d0de22522c0b1e1e3e874e7df4c876587d5ae13ce2266b1964c0a6d7016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292665190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f63c85a7b03e25228be9f24de1030063761e345233193a453837937a5397aab`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:20:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:20:10 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:20:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:23 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:23 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d734d2deca94a63896944f62629cffc9c69bac985aedb4b08fb3736c767377ad`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ac29574a2a198c6f5c01263cff98202cb4cd88d163d493b10bd232f4a3e50`  
		Last Modified: Thu, 14 Sep 2023 21:21:55 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1c9a6bed0e54128889e4f6101b56bad707140ac1e2d0ab666f3bb4f09286e`  
		Last Modified: Thu, 14 Sep 2023 21:22:01 GMT  
		Size: 116.5 MB (116458603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:47ab9e05d4cfe43f89bb7c82153241f4b1095fa04ae0decb844cf55796c266b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (289971017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937a938bd2f5d847c2f5a244a95d9343c8617a42be8d295c8ebcf0032a5d6642`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 14 Sep 2023 21:42:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 14 Sep 2023 21:42:13 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 14 Sep 2023 21:42:24 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:24 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:24 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:24 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0498f9039a723905f7c5f269ebf5a3de77da540ef8457b5ba94675b185b6ce05`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7abba314650844ea592ae83d36590b464dfaa5eafdb5b3a75a245f96e2b820`  
		Last Modified: Thu, 14 Sep 2023 21:43:46 GMT  
		Size: 9.4 KB (9432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8e1dcd0c8f9d4ec0478351e6df7519be973eaf9928d68996e74c8204bfeb3`  
		Last Modified: Thu, 14 Sep 2023 21:43:52 GMT  
		Size: 116.4 MB (116351303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:ubi8`

```console
$ docker pull neo4j@sha256:d29478ad98405ad06087f23c8f2049aa036c3a8777c84b20ac17f8940822724c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:fdf7a80bc7dd807fdafbb2364cd0921827e3fcd2b6fab38dbbbadbc3ddefc321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303257353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5823c5426f54a894f9cdfc79c17b356ed9d056ab56a4ec9f256064a9ad8bac`
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
# Sat, 02 Sep 2023 02:47:05 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:47:15 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:20:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:20:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:20:54 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:20:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:20:58 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:20:58 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:20:58 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:20:58 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:20:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:20:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:d2b5f358ecf170222d561c3811b4d74699c0078ec14ffaa84434d303b0b3591f`  
		Last Modified: Tue, 16 May 2023 13:59:36 GMT  
		Size: 39.3 MB (39289044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e607cc5876c0bfb7285f94800f1484d58fe9bd21ff0940f8e199a8ec19669d`  
		Last Modified: Sat, 02 Sep 2023 02:50:10 GMT  
		Size: 144.8 MB (144775777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540a5874536ce61a9f53e4278b486a0dff74d391fab34c27efabdefc0a38d646`  
		Last Modified: Sat, 02 Sep 2023 02:50:00 GMT  
		Size: 6.5 MB (6530132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919fe744d5f603d87da82bdadbc5d011fdf5adf4910cedf6b9e9588e46dffa6e`  
		Last Modified: Thu, 14 Sep 2023 21:23:26 GMT  
		Size: 9.4 KB (9429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88653088570193201dc09d69eb4938fbcc51c7ad2e0459a0b61a57f1695f5aab`  
		Last Modified: Thu, 14 Sep 2023 21:23:32 GMT  
		Size: 112.7 MB (112652971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:15f58472ef484515f428bacf3e5a699d38eecfcdcbcc6afba7004c8e0f12f703
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300234017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4778c2d781e075ce6f1482ad7142533eade8221941fb898a9dc441a1814597fb`
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
# Sat, 02 Sep 2023 02:39:24 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:39:34 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Thu, 14 Sep 2023 21:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=adf9e7915f5c10dfa4daf9eab79852660887eac3c3e165741fce48415c0b6f34 NEO4J_TARBALL=neo4j-community-5.12.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 14 Sep 2023 21:42:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
# Thu, 14 Sep 2023 21:42:52 GMT
COPY multi:f4e8828c26bc3c80f7c5af331adb809a61a5b929b6f67c8cd774aa23152e75a5 in /startup/ 
# Thu, 14 Sep 2023 21:42:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.12.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Thu, 14 Sep 2023 21:42:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Sep 2023 21:42:56 GMT
WORKDIR /var/lib/neo4j
# Thu, 14 Sep 2023 21:42:56 GMT
VOLUME [/data /logs]
# Thu, 14 Sep 2023 21:42:56 GMT
EXPOSE 7473 7474 7687
# Thu, 14 Sep 2023 21:42:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 14 Sep 2023 21:42:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b964235f9f3052ef964da88e3540367964bd517e4c985fcdc8a6b705c48326ed`  
		Last Modified: Tue, 16 May 2023 16:09:53 GMT  
		Size: 37.5 MB (37531440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ca9ac3c4d8ddd57788859e956015214d4e4fae8c8f54d57685a5869dd9ed3b`  
		Last Modified: Sat, 02 Sep 2023 02:42:21 GMT  
		Size: 143.5 MB (143543467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f62b3cfd3612a7f30d0c2183297b1bfb8c45f4a7859b6cef82656c9c268bd6`  
		Last Modified: Sat, 02 Sep 2023 02:42:13 GMT  
		Size: 6.5 MB (6496684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6618326ab8e89e417d1e87239720ea529da8606c89719f7594bda95e3e2a3618`  
		Last Modified: Thu, 14 Sep 2023 21:45:15 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f793dea39a11763e145f397c62687392563260fd1e0bc27e5c26019f3cba18`  
		Last Modified: Thu, 14 Sep 2023 21:45:22 GMT  
		Size: 112.7 MB (112652999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
