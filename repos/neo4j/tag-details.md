<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.27`](#neo4j4427)
-	[`neo4j:4.4.27-community`](#neo4j4427-community)
-	[`neo4j:4.4.27-enterprise`](#neo4j4427-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-bullseye`](#neo4j5-bullseye)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-community-bullseye`](#neo4j5-community-bullseye)
-	[`neo4j:5-community-ubi8`](#neo4j5-community-ubi8)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5-enterprise-bullseye`](#neo4j5-enterprise-bullseye)
-	[`neo4j:5-enterprise-ubi8`](#neo4j5-enterprise-ubi8)
-	[`neo4j:5-ubi8`](#neo4j5-ubi8)
-	[`neo4j:5.13`](#neo4j513)
-	[`neo4j:5.13-bullseye`](#neo4j513-bullseye)
-	[`neo4j:5.13-community`](#neo4j513-community)
-	[`neo4j:5.13-community-bullseye`](#neo4j513-community-bullseye)
-	[`neo4j:5.13-community-ubi8`](#neo4j513-community-ubi8)
-	[`neo4j:5.13-enterprise`](#neo4j513-enterprise)
-	[`neo4j:5.13-enterprise-bullseye`](#neo4j513-enterprise-bullseye)
-	[`neo4j:5.13-enterprise-ubi8`](#neo4j513-enterprise-ubi8)
-	[`neo4j:5.13-ubi8`](#neo4j513-ubi8)
-	[`neo4j:5.13.0`](#neo4j5130)
-	[`neo4j:5.13.0-bullseye`](#neo4j5130-bullseye)
-	[`neo4j:5.13.0-community`](#neo4j5130-community)
-	[`neo4j:5.13.0-community-bullseye`](#neo4j5130-community-bullseye)
-	[`neo4j:5.13.0-community-ubi8`](#neo4j5130-community-ubi8)
-	[`neo4j:5.13.0-enterprise`](#neo4j5130-enterprise)
-	[`neo4j:5.13.0-enterprise-bullseye`](#neo4j5130-enterprise-bullseye)
-	[`neo4j:5.13.0-enterprise-ubi8`](#neo4j5130-enterprise-ubi8)
-	[`neo4j:5.13.0-ubi8`](#neo4j5130-ubi8)
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
$ docker pull neo4j@sha256:86b51684f3d4633729aab5e1907840d859e74982f595b161e4580179dba6111d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:35e6b99cb041037510e879a758820776ae5ba7600b69db4cba70cd4a438928b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.0 MB (299042245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f8cfd6664e0920442d05352bdcf092ea12f47c9ff3d8130eabc989a049108c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:18:55 GMT
COPY dir:a96babc4beed1ce86268c08da8bb1232eedf77a64576d0e7cc109ca29beb78ef in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:56:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=8c547187bdd00bdb735d4fcf4036e158b54071499608c1262d3108f5550155f7 NEO4J_TARBALL=neo4j-community-4.4.26-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:56:18 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
# Wed, 01 Nov 2023 11:56:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:56:19 GMT
COPY multi:a23c335136a31744c3da3fe5cd721fb899707ce1efde466c13bf9deefb000b04 in /startup/ 
# Wed, 01 Nov 2023 11:56:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:56:34 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:56:34 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:56:34 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:56:35 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:56:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:56:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0c2457a667e342734343cd296f94de2032329a37ee32ca0f48794427a59f05`  
		Last Modified: Wed, 01 Nov 2023 01:37:19 GMT  
		Size: 145.3 MB (145266641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75884059f2688d38c591634dd5af757a27244367ffa86986cb653100bb8b6c1`  
		Last Modified: Wed, 01 Nov 2023 11:59:01 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c6fa7859ad299c9fdb6962642157cf9ebec11e567b9ded7b0233b189a9ecc8`  
		Last Modified: Wed, 01 Nov 2023 11:59:01 GMT  
		Size: 9.3 KB (9296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9391d3e2ff6d89e7268435ef9aea9190b233151ce5dddfd8e46a71fdb2dadced`  
		Last Modified: Wed, 01 Nov 2023 11:59:08 GMT  
		Size: 122.3 MB (122344535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:a370acee7485a0b7c92817437aea820e211d0383833f02365b5a69b5a0d60a09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.3 MB (294314519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a642eb08689f5f82aca588951b30d78487db3b80d19b9f6ba353b11520361d0f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:28:12 GMT
COPY dir:434bcbe7e3d8ce2c5a3427f1d3fb9b84e4c00833b8498e54aed72311e918f97b in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:42:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=8c547187bdd00bdb735d4fcf4036e158b54071499608c1262d3108f5550155f7 NEO4J_TARBALL=neo4j-community-4.4.26-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:42:24 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
# Wed, 01 Nov 2023 08:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:42:24 GMT
COPY multi:a23c335136a31744c3da3fe5cd721fb899707ce1efde466c13bf9deefb000b04 in /startup/ 
# Wed, 01 Nov 2023 08:42:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:35 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:35 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:35 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117d3cf4375642fd4a8848e4f992aa9adeeeece9e9357c8f6512cdc3657e9748`  
		Last Modified: Wed, 01 Nov 2023 02:45:09 GMT  
		Size: 142.0 MB (142001956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b88c12b4f2adf560de78f8f57fc639e134740171f0d13446f425e9c04ec4b2e`  
		Last Modified: Wed, 01 Nov 2023 08:44:46 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474d5655b87a65f302f805e02a605e023ae62ad823a1756dbb5733a081deaa68`  
		Last Modified: Wed, 01 Nov 2023 08:44:46 GMT  
		Size: 9.3 KB (9285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51124e736e5e6adf0fb6752d4a0b01cc8d97c952447daae481f9f6fde65391a4`  
		Last Modified: Wed, 01 Nov 2023 08:44:53 GMT  
		Size: 122.2 MB (122235488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:86b51684f3d4633729aab5e1907840d859e74982f595b161e4580179dba6111d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:35e6b99cb041037510e879a758820776ae5ba7600b69db4cba70cd4a438928b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.0 MB (299042245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f8cfd6664e0920442d05352bdcf092ea12f47c9ff3d8130eabc989a049108c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:18:55 GMT
COPY dir:a96babc4beed1ce86268c08da8bb1232eedf77a64576d0e7cc109ca29beb78ef in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:56:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=8c547187bdd00bdb735d4fcf4036e158b54071499608c1262d3108f5550155f7 NEO4J_TARBALL=neo4j-community-4.4.26-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:56:18 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
# Wed, 01 Nov 2023 11:56:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:56:19 GMT
COPY multi:a23c335136a31744c3da3fe5cd721fb899707ce1efde466c13bf9deefb000b04 in /startup/ 
# Wed, 01 Nov 2023 11:56:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:56:34 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:56:34 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:56:34 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:56:35 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:56:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:56:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0c2457a667e342734343cd296f94de2032329a37ee32ca0f48794427a59f05`  
		Last Modified: Wed, 01 Nov 2023 01:37:19 GMT  
		Size: 145.3 MB (145266641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75884059f2688d38c591634dd5af757a27244367ffa86986cb653100bb8b6c1`  
		Last Modified: Wed, 01 Nov 2023 11:59:01 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c6fa7859ad299c9fdb6962642157cf9ebec11e567b9ded7b0233b189a9ecc8`  
		Last Modified: Wed, 01 Nov 2023 11:59:01 GMT  
		Size: 9.3 KB (9296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9391d3e2ff6d89e7268435ef9aea9190b233151ce5dddfd8e46a71fdb2dadced`  
		Last Modified: Wed, 01 Nov 2023 11:59:08 GMT  
		Size: 122.3 MB (122344535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:a370acee7485a0b7c92817437aea820e211d0383833f02365b5a69b5a0d60a09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.3 MB (294314519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a642eb08689f5f82aca588951b30d78487db3b80d19b9f6ba353b11520361d0f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:28:12 GMT
COPY dir:434bcbe7e3d8ce2c5a3427f1d3fb9b84e4c00833b8498e54aed72311e918f97b in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:42:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=8c547187bdd00bdb735d4fcf4036e158b54071499608c1262d3108f5550155f7 NEO4J_TARBALL=neo4j-community-4.4.26-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:42:24 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
# Wed, 01 Nov 2023 08:42:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:42:24 GMT
COPY multi:a23c335136a31744c3da3fe5cd721fb899707ce1efde466c13bf9deefb000b04 in /startup/ 
# Wed, 01 Nov 2023 08:42:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.26-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:35 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:35 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:35 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117d3cf4375642fd4a8848e4f992aa9adeeeece9e9357c8f6512cdc3657e9748`  
		Last Modified: Wed, 01 Nov 2023 02:45:09 GMT  
		Size: 142.0 MB (142001956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b88c12b4f2adf560de78f8f57fc639e134740171f0d13446f425e9c04ec4b2e`  
		Last Modified: Wed, 01 Nov 2023 08:44:46 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474d5655b87a65f302f805e02a605e023ae62ad823a1756dbb5733a081deaa68`  
		Last Modified: Wed, 01 Nov 2023 08:44:46 GMT  
		Size: 9.3 KB (9285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51124e736e5e6adf0fb6752d4a0b01cc8d97c952447daae481f9f6fde65391a4`  
		Last Modified: Wed, 01 Nov 2023 08:44:53 GMT  
		Size: 122.2 MB (122235488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:fb0bf5826fdc3433e4f87032b9de2f8056d0156af649542c0af15cb823adb3ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:66a16b9ac26106eaf071974aad8445859d55654bc8685f57a56b2684d8df5218
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **405.7 MB (405731716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f610ed3eea30578b9d346a87ea6b0c9eb14038413de80d9871bdf7eb249fcef`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:18:55 GMT
COPY dir:a96babc4beed1ce86268c08da8bb1232eedf77a64576d0e7cc109ca29beb78ef in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:56:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5059157293dee431cd78ad350b077792a481526b3994f5f043529d7145005914 NEO4J_TARBALL=neo4j-enterprise-4.4.26-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:56:38 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.26-unix.tar.gz
# Wed, 01 Nov 2023 11:56:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.26-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:56:39 GMT
COPY multi:a23c335136a31744c3da3fe5cd721fb899707ce1efde466c13bf9deefb000b04 in /startup/ 
# Wed, 01 Nov 2023 11:57:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.26-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:57:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:57:00 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:57:01 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:57:01 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:57:01 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:57:01 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0c2457a667e342734343cd296f94de2032329a37ee32ca0f48794427a59f05`  
		Last Modified: Wed, 01 Nov 2023 01:37:19 GMT  
		Size: 145.3 MB (145266641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fede7923a0eb68b976aa8350857c7504666f238bebb060a776fa523c5d1728f0`  
		Last Modified: Wed, 01 Nov 2023 11:59:21 GMT  
		Size: 3.9 KB (3864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450b449855eff13c2627cd369c03e38209ee538db9c26e05f8596da8304926a7`  
		Last Modified: Wed, 01 Nov 2023 11:59:21 GMT  
		Size: 9.3 KB (9298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68ebc7bbdedec78f655a6d03d3519ffaad6128c426d86435a82eabc8893bdfe`  
		Last Modified: Wed, 01 Nov 2023 11:59:33 GMT  
		Size: 229.0 MB (229033998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4a6a98d17a95524ef06c2dc34bf40c83e773ae2704365a7db266f9ae31108f27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.0 MB (401007031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0c8618195c1f91f7e06bbaa29e074d6c71a3514ecf8c18269aac72a6dbcc26`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:28:12 GMT
COPY dir:434bcbe7e3d8ce2c5a3427f1d3fb9b84e4c00833b8498e54aed72311e918f97b in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:42:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5059157293dee431cd78ad350b077792a481526b3994f5f043529d7145005914 NEO4J_TARBALL=neo4j-enterprise-4.4.26-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:42:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.26-unix.tar.gz
# Wed, 01 Nov 2023 08:42:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.26-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:42:38 GMT
COPY multi:a23c335136a31744c3da3fe5cd721fb899707ce1efde466c13bf9deefb000b04 in /startup/ 
# Wed, 01 Nov 2023 08:42:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.26-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:52 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:52 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:52 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117d3cf4375642fd4a8848e4f992aa9adeeeece9e9357c8f6512cdc3657e9748`  
		Last Modified: Wed, 01 Nov 2023 02:45:09 GMT  
		Size: 142.0 MB (142001956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701be5f952cce2cddcc129c4f1cace19c3d5cb15b306d0328be830343b1d81c0`  
		Last Modified: Wed, 01 Nov 2023 08:45:06 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ef5b5d7f4a825f6394dfd3c4d09e81fa9728ec32c43ea052c6d63f9a315686`  
		Last Modified: Wed, 01 Nov 2023 08:45:06 GMT  
		Size: 9.3 KB (9294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5a50cd0a913be024d60b45067d09138046575c036e704d409995a95c7a3f11`  
		Last Modified: Wed, 01 Nov 2023 08:45:16 GMT  
		Size: 228.9 MB (228927992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.27`

**does not exist** (yet?)

## `neo4j:4.4.27-community`

**does not exist** (yet?)

## `neo4j:4.4.27-enterprise`

**does not exist** (yet?)

## `neo4j:5`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-bullseye`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community-bullseye`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community-ubi8`

```console
$ docker pull neo4j@sha256:cada68dcf9da0d3c9834a302fe09b7c40e594674eee89b81457efa9e0183424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:7f529f9b883e7508d4d1a47443425886646969b67110faca226ecd6e3d7db0c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0876e68b678eab976554606ae27aabd58cc4db13da7af5ec730f198d334d1`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:09:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:09:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:09:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:02 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:02 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:03 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:03 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdc8bfe48d470191a4f525a0d0a2b2d2df8cf58b607493f4fe27287d41a7e8a`  
		Last Modified: Tue, 31 Oct 2023 03:12:42 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f61cdc434df46bf9943e942b815c6121c056d9a469e1d1ff9b88d8c8ac6b080`  
		Last Modified: Tue, 31 Oct 2023 03:12:49 GMT  
		Size: 112.6 MB (112571528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e852f99034810f3853e7fbd42ccb0207c3cfc7ea9a1cbc9458f169446970d2ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300468610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682e56eb5ed513792f1a3c4c10172712d2e63f8c1737aa35adea5df8ed058dbe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:37 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:37 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:37 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4cf921619b8aac5f90d22a4751c47aee713ce6ccc841fd7091823360a9953`  
		Last Modified: Tue, 31 Oct 2023 03:58:03 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787c30cb8efdf63af7a59c1dc194fc2f186fe59528309cacb4525b7ca4b18ea5`  
		Last Modified: Tue, 31 Oct 2023 03:58:08 GMT  
		Size: 112.6 MB (112571529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:3ba240f0f98a9dfb36b591658e9976423119ce3c4b0752effeecb436cb79141a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:c06d2e3593ace7b5984247570bc7bfa336afcc347a543f79b7e9593c64608444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.1 MB (564093810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f6974de9e5edca7c27b493cc9a4959fd4f997fe84db8e7cac6ff901e019159`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:50 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:56:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:56:09 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:56:09 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:56:09 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:56:09 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:56:09 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:56:09 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ce05f723ae6f403ba26b5d6efb3209577c09e9d60ec669883c5f799e3240d`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d8e127dcb8291bfb875525eab211a5fea04d223d0df3cd719dcf34821891c8`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7400cfd78a582a74d4a5cbec94f3d6aecb3d03ebd11838a8732505c9d0122`  
		Last Modified: Wed, 01 Nov 2023 11:58:33 GMT  
		Size: 387.8 MB (387788715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bafbdc4ed75df1abbb01b93416a08511aa5189672793d28b01e1b29367ea724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561438922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c834f2faaae66515d6d82c003a5cbf02a5396f8bad78309be9848a5154a9d4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:42:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:16 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:16 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd3e2b17175aa2df8cca1499ca69f75103438a03fa131090a082e671602504b`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78783676f896069de84f62f2fbb011f92359c7445a847918f1a662ed7b1680f1`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 9.4 KB (9420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3705cef4738487a702410b792ca8ff249ed68c9e513072c0c4c2f1e5a320716`  
		Last Modified: Wed, 01 Nov 2023 08:44:18 GMT  
		Size: 387.7 MB (387679965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:3ba240f0f98a9dfb36b591658e9976423119ce3c4b0752effeecb436cb79141a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:c06d2e3593ace7b5984247570bc7bfa336afcc347a543f79b7e9593c64608444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.1 MB (564093810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f6974de9e5edca7c27b493cc9a4959fd4f997fe84db8e7cac6ff901e019159`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:50 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:56:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:56:09 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:56:09 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:56:09 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:56:09 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:56:09 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:56:09 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ce05f723ae6f403ba26b5d6efb3209577c09e9d60ec669883c5f799e3240d`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d8e127dcb8291bfb875525eab211a5fea04d223d0df3cd719dcf34821891c8`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7400cfd78a582a74d4a5cbec94f3d6aecb3d03ebd11838a8732505c9d0122`  
		Last Modified: Wed, 01 Nov 2023 11:58:33 GMT  
		Size: 387.8 MB (387788715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bafbdc4ed75df1abbb01b93416a08511aa5189672793d28b01e1b29367ea724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561438922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c834f2faaae66515d6d82c003a5cbf02a5396f8bad78309be9848a5154a9d4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:42:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:16 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:16 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd3e2b17175aa2df8cca1499ca69f75103438a03fa131090a082e671602504b`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78783676f896069de84f62f2fbb011f92359c7445a847918f1a662ed7b1680f1`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 9.4 KB (9420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3705cef4738487a702410b792ca8ff249ed68c9e513072c0c4c2f1e5a320716`  
		Last Modified: Wed, 01 Nov 2023 08:44:18 GMT  
		Size: 387.7 MB (387679965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:fbf58db74d5fb993cd188808ae3a966f0119c4eefce3295fff49abc51fec549d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:a613d5196615fb0090ada8c126151e663bcf6bea31edf2a83570949d49352059
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.7 MB (574691704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8f814c463a4165096f3b6f1fa1836fa16bc3f13ec33011a9d49ecef17805155`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:10:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:10:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:10:07 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:17 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:17 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:17 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:18 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:18 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:18 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d9719156c8861c63c0f3d35884d03cdbfac1b86e31fff24c5c94c7c0baba3c`  
		Last Modified: Tue, 31 Oct 2023 03:13:15 GMT  
		Size: 9.4 KB (9421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b5411e7bd3bb3e8f212dc4a7abbd40cc839cfe7e6a4d0e179570c3ae9f11f8`  
		Last Modified: Tue, 31 Oct 2023 03:13:33 GMT  
		Size: 384.0 MB (383978163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:cbf81ff37755b9cb2196cfe822cb0671bc97bd69bb3cbfff84ad1114cdde5301
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **571.9 MB (571875278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433d59458c2f432f8c0153903d7ff89b6367a36b3088dd0e23fde154581c1bb9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:39 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:51 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:51 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:51 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:51 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9270bb2ee329178be9827cb8f5438ef26e8f5a4a6a5f87bfa19cf97b258ebf64`  
		Last Modified: Tue, 31 Oct 2023 03:58:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d1ebb2e92c7a0041a3eb8cf0052ed6c07948d47d0e86a3b4d99d799e7d9df2`  
		Last Modified: Tue, 31 Oct 2023 03:58:48 GMT  
		Size: 384.0 MB (383978199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-ubi8`

```console
$ docker pull neo4j@sha256:cada68dcf9da0d3c9834a302fe09b7c40e594674eee89b81457efa9e0183424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:7f529f9b883e7508d4d1a47443425886646969b67110faca226ecd6e3d7db0c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0876e68b678eab976554606ae27aabd58cc4db13da7af5ec730f198d334d1`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:09:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:09:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:09:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:02 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:02 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:03 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:03 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdc8bfe48d470191a4f525a0d0a2b2d2df8cf58b607493f4fe27287d41a7e8a`  
		Last Modified: Tue, 31 Oct 2023 03:12:42 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f61cdc434df46bf9943e942b815c6121c056d9a469e1d1ff9b88d8c8ac6b080`  
		Last Modified: Tue, 31 Oct 2023 03:12:49 GMT  
		Size: 112.6 MB (112571528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e852f99034810f3853e7fbd42ccb0207c3cfc7ea9a1cbc9458f169446970d2ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300468610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682e56eb5ed513792f1a3c4c10172712d2e63f8c1737aa35adea5df8ed058dbe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:37 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:37 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:37 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4cf921619b8aac5f90d22a4751c47aee713ce6ccc841fd7091823360a9953`  
		Last Modified: Tue, 31 Oct 2023 03:58:03 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787c30cb8efdf63af7a59c1dc194fc2f186fe59528309cacb4525b7ca4b18ea5`  
		Last Modified: Tue, 31 Oct 2023 03:58:08 GMT  
		Size: 112.6 MB (112571529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13-bullseye`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13-community`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13-community` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13-community-bullseye`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13-community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13-community-ubi8`

```console
$ docker pull neo4j@sha256:cada68dcf9da0d3c9834a302fe09b7c40e594674eee89b81457efa9e0183424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13-community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:7f529f9b883e7508d4d1a47443425886646969b67110faca226ecd6e3d7db0c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0876e68b678eab976554606ae27aabd58cc4db13da7af5ec730f198d334d1`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:09:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:09:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:09:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:02 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:02 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:03 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:03 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdc8bfe48d470191a4f525a0d0a2b2d2df8cf58b607493f4fe27287d41a7e8a`  
		Last Modified: Tue, 31 Oct 2023 03:12:42 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f61cdc434df46bf9943e942b815c6121c056d9a469e1d1ff9b88d8c8ac6b080`  
		Last Modified: Tue, 31 Oct 2023 03:12:49 GMT  
		Size: 112.6 MB (112571528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e852f99034810f3853e7fbd42ccb0207c3cfc7ea9a1cbc9458f169446970d2ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300468610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682e56eb5ed513792f1a3c4c10172712d2e63f8c1737aa35adea5df8ed058dbe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:37 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:37 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:37 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4cf921619b8aac5f90d22a4751c47aee713ce6ccc841fd7091823360a9953`  
		Last Modified: Tue, 31 Oct 2023 03:58:03 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787c30cb8efdf63af7a59c1dc194fc2f186fe59528309cacb4525b7ca4b18ea5`  
		Last Modified: Tue, 31 Oct 2023 03:58:08 GMT  
		Size: 112.6 MB (112571529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13-enterprise`

```console
$ docker pull neo4j@sha256:3ba240f0f98a9dfb36b591658e9976423119ce3c4b0752effeecb436cb79141a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:c06d2e3593ace7b5984247570bc7bfa336afcc347a543f79b7e9593c64608444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.1 MB (564093810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f6974de9e5edca7c27b493cc9a4959fd4f997fe84db8e7cac6ff901e019159`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:50 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:56:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:56:09 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:56:09 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:56:09 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:56:09 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:56:09 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:56:09 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ce05f723ae6f403ba26b5d6efb3209577c09e9d60ec669883c5f799e3240d`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d8e127dcb8291bfb875525eab211a5fea04d223d0df3cd719dcf34821891c8`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7400cfd78a582a74d4a5cbec94f3d6aecb3d03ebd11838a8732505c9d0122`  
		Last Modified: Wed, 01 Nov 2023 11:58:33 GMT  
		Size: 387.8 MB (387788715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bafbdc4ed75df1abbb01b93416a08511aa5189672793d28b01e1b29367ea724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561438922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c834f2faaae66515d6d82c003a5cbf02a5396f8bad78309be9848a5154a9d4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:42:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:16 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:16 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd3e2b17175aa2df8cca1499ca69f75103438a03fa131090a082e671602504b`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78783676f896069de84f62f2fbb011f92359c7445a847918f1a662ed7b1680f1`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 9.4 KB (9420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3705cef4738487a702410b792ca8ff249ed68c9e513072c0c4c2f1e5a320716`  
		Last Modified: Wed, 01 Nov 2023 08:44:18 GMT  
		Size: 387.7 MB (387679965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:3ba240f0f98a9dfb36b591658e9976423119ce3c4b0752effeecb436cb79141a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:c06d2e3593ace7b5984247570bc7bfa336afcc347a543f79b7e9593c64608444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.1 MB (564093810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f6974de9e5edca7c27b493cc9a4959fd4f997fe84db8e7cac6ff901e019159`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:50 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:56:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:56:09 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:56:09 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:56:09 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:56:09 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:56:09 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:56:09 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ce05f723ae6f403ba26b5d6efb3209577c09e9d60ec669883c5f799e3240d`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d8e127dcb8291bfb875525eab211a5fea04d223d0df3cd719dcf34821891c8`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7400cfd78a582a74d4a5cbec94f3d6aecb3d03ebd11838a8732505c9d0122`  
		Last Modified: Wed, 01 Nov 2023 11:58:33 GMT  
		Size: 387.8 MB (387788715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bafbdc4ed75df1abbb01b93416a08511aa5189672793d28b01e1b29367ea724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561438922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c834f2faaae66515d6d82c003a5cbf02a5396f8bad78309be9848a5154a9d4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:42:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:16 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:16 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd3e2b17175aa2df8cca1499ca69f75103438a03fa131090a082e671602504b`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78783676f896069de84f62f2fbb011f92359c7445a847918f1a662ed7b1680f1`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 9.4 KB (9420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3705cef4738487a702410b792ca8ff249ed68c9e513072c0c4c2f1e5a320716`  
		Last Modified: Wed, 01 Nov 2023 08:44:18 GMT  
		Size: 387.7 MB (387679965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:fbf58db74d5fb993cd188808ae3a966f0119c4eefce3295fff49abc51fec549d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13-enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:a613d5196615fb0090ada8c126151e663bcf6bea31edf2a83570949d49352059
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.7 MB (574691704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8f814c463a4165096f3b6f1fa1836fa16bc3f13ec33011a9d49ecef17805155`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:10:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:10:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:10:07 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:17 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:17 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:17 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:18 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:18 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:18 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d9719156c8861c63c0f3d35884d03cdbfac1b86e31fff24c5c94c7c0baba3c`  
		Last Modified: Tue, 31 Oct 2023 03:13:15 GMT  
		Size: 9.4 KB (9421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b5411e7bd3bb3e8f212dc4a7abbd40cc839cfe7e6a4d0e179570c3ae9f11f8`  
		Last Modified: Tue, 31 Oct 2023 03:13:33 GMT  
		Size: 384.0 MB (383978163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13-enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:cbf81ff37755b9cb2196cfe822cb0671bc97bd69bb3cbfff84ad1114cdde5301
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **571.9 MB (571875278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433d59458c2f432f8c0153903d7ff89b6367a36b3088dd0e23fde154581c1bb9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:39 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:51 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:51 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:51 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:51 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9270bb2ee329178be9827cb8f5438ef26e8f5a4a6a5f87bfa19cf97b258ebf64`  
		Last Modified: Tue, 31 Oct 2023 03:58:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d1ebb2e92c7a0041a3eb8cf0052ed6c07948d47d0e86a3b4d99d799e7d9df2`  
		Last Modified: Tue, 31 Oct 2023 03:58:48 GMT  
		Size: 384.0 MB (383978199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13-ubi8`

```console
$ docker pull neo4j@sha256:cada68dcf9da0d3c9834a302fe09b7c40e594674eee89b81457efa9e0183424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:7f529f9b883e7508d4d1a47443425886646969b67110faca226ecd6e3d7db0c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0876e68b678eab976554606ae27aabd58cc4db13da7af5ec730f198d334d1`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:09:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:09:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:09:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:02 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:02 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:03 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:03 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdc8bfe48d470191a4f525a0d0a2b2d2df8cf58b607493f4fe27287d41a7e8a`  
		Last Modified: Tue, 31 Oct 2023 03:12:42 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f61cdc434df46bf9943e942b815c6121c056d9a469e1d1ff9b88d8c8ac6b080`  
		Last Modified: Tue, 31 Oct 2023 03:12:49 GMT  
		Size: 112.6 MB (112571528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e852f99034810f3853e7fbd42ccb0207c3cfc7ea9a1cbc9458f169446970d2ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300468610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682e56eb5ed513792f1a3c4c10172712d2e63f8c1737aa35adea5df8ed058dbe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:37 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:37 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:37 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4cf921619b8aac5f90d22a4751c47aee713ce6ccc841fd7091823360a9953`  
		Last Modified: Tue, 31 Oct 2023 03:58:03 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787c30cb8efdf63af7a59c1dc194fc2f186fe59528309cacb4525b7ca4b18ea5`  
		Last Modified: Tue, 31 Oct 2023 03:58:08 GMT  
		Size: 112.6 MB (112571529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13.0`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13.0` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13.0-bullseye`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13.0-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13.0-community`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13.0-community-bullseye`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13.0-community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13.0-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13.0-community-ubi8`

```console
$ docker pull neo4j@sha256:cada68dcf9da0d3c9834a302fe09b7c40e594674eee89b81457efa9e0183424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13.0-community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:7f529f9b883e7508d4d1a47443425886646969b67110faca226ecd6e3d7db0c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0876e68b678eab976554606ae27aabd58cc4db13da7af5ec730f198d334d1`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:09:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:09:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:09:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:02 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:02 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:03 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:03 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdc8bfe48d470191a4f525a0d0a2b2d2df8cf58b607493f4fe27287d41a7e8a`  
		Last Modified: Tue, 31 Oct 2023 03:12:42 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f61cdc434df46bf9943e942b815c6121c056d9a469e1d1ff9b88d8c8ac6b080`  
		Last Modified: Tue, 31 Oct 2023 03:12:49 GMT  
		Size: 112.6 MB (112571528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13.0-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e852f99034810f3853e7fbd42ccb0207c3cfc7ea9a1cbc9458f169446970d2ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300468610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682e56eb5ed513792f1a3c4c10172712d2e63f8c1737aa35adea5df8ed058dbe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:37 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:37 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:37 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4cf921619b8aac5f90d22a4751c47aee713ce6ccc841fd7091823360a9953`  
		Last Modified: Tue, 31 Oct 2023 03:58:03 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787c30cb8efdf63af7a59c1dc194fc2f186fe59528309cacb4525b7ca4b18ea5`  
		Last Modified: Tue, 31 Oct 2023 03:58:08 GMT  
		Size: 112.6 MB (112571529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13.0-enterprise`

```console
$ docker pull neo4j@sha256:3ba240f0f98a9dfb36b591658e9976423119ce3c4b0752effeecb436cb79141a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:c06d2e3593ace7b5984247570bc7bfa336afcc347a543f79b7e9593c64608444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.1 MB (564093810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f6974de9e5edca7c27b493cc9a4959fd4f997fe84db8e7cac6ff901e019159`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:50 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:56:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:56:09 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:56:09 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:56:09 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:56:09 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:56:09 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:56:09 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ce05f723ae6f403ba26b5d6efb3209577c09e9d60ec669883c5f799e3240d`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d8e127dcb8291bfb875525eab211a5fea04d223d0df3cd719dcf34821891c8`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7400cfd78a582a74d4a5cbec94f3d6aecb3d03ebd11838a8732505c9d0122`  
		Last Modified: Wed, 01 Nov 2023 11:58:33 GMT  
		Size: 387.8 MB (387788715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bafbdc4ed75df1abbb01b93416a08511aa5189672793d28b01e1b29367ea724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561438922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c834f2faaae66515d6d82c003a5cbf02a5396f8bad78309be9848a5154a9d4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:42:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:16 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:16 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd3e2b17175aa2df8cca1499ca69f75103438a03fa131090a082e671602504b`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78783676f896069de84f62f2fbb011f92359c7445a847918f1a662ed7b1680f1`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 9.4 KB (9420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3705cef4738487a702410b792ca8ff249ed68c9e513072c0c4c2f1e5a320716`  
		Last Modified: Wed, 01 Nov 2023 08:44:18 GMT  
		Size: 387.7 MB (387679965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13.0-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:3ba240f0f98a9dfb36b591658e9976423119ce3c4b0752effeecb436cb79141a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13.0-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:c06d2e3593ace7b5984247570bc7bfa336afcc347a543f79b7e9593c64608444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.1 MB (564093810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f6974de9e5edca7c27b493cc9a4959fd4f997fe84db8e7cac6ff901e019159`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:50 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:56:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:56:09 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:56:09 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:56:09 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:56:09 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:56:09 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:56:09 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ce05f723ae6f403ba26b5d6efb3209577c09e9d60ec669883c5f799e3240d`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d8e127dcb8291bfb875525eab211a5fea04d223d0df3cd719dcf34821891c8`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7400cfd78a582a74d4a5cbec94f3d6aecb3d03ebd11838a8732505c9d0122`  
		Last Modified: Wed, 01 Nov 2023 11:58:33 GMT  
		Size: 387.8 MB (387788715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13.0-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bafbdc4ed75df1abbb01b93416a08511aa5189672793d28b01e1b29367ea724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561438922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c834f2faaae66515d6d82c003a5cbf02a5396f8bad78309be9848a5154a9d4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:42:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:16 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:16 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd3e2b17175aa2df8cca1499ca69f75103438a03fa131090a082e671602504b`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78783676f896069de84f62f2fbb011f92359c7445a847918f1a662ed7b1680f1`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 9.4 KB (9420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3705cef4738487a702410b792ca8ff249ed68c9e513072c0c4c2f1e5a320716`  
		Last Modified: Wed, 01 Nov 2023 08:44:18 GMT  
		Size: 387.7 MB (387679965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13.0-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:fbf58db74d5fb993cd188808ae3a966f0119c4eefce3295fff49abc51fec549d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13.0-enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:a613d5196615fb0090ada8c126151e663bcf6bea31edf2a83570949d49352059
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.7 MB (574691704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8f814c463a4165096f3b6f1fa1836fa16bc3f13ec33011a9d49ecef17805155`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:10:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:10:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:10:07 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:17 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:17 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:17 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:18 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:18 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:18 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d9719156c8861c63c0f3d35884d03cdbfac1b86e31fff24c5c94c7c0baba3c`  
		Last Modified: Tue, 31 Oct 2023 03:13:15 GMT  
		Size: 9.4 KB (9421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b5411e7bd3bb3e8f212dc4a7abbd40cc839cfe7e6a4d0e179570c3ae9f11f8`  
		Last Modified: Tue, 31 Oct 2023 03:13:33 GMT  
		Size: 384.0 MB (383978163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13.0-enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:cbf81ff37755b9cb2196cfe822cb0671bc97bd69bb3cbfff84ad1114cdde5301
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **571.9 MB (571875278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433d59458c2f432f8c0153903d7ff89b6367a36b3088dd0e23fde154581c1bb9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:39 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:51 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:51 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:51 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:51 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9270bb2ee329178be9827cb8f5438ef26e8f5a4a6a5f87bfa19cf97b258ebf64`  
		Last Modified: Tue, 31 Oct 2023 03:58:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d1ebb2e92c7a0041a3eb8cf0052ed6c07948d47d0e86a3b4d99d799e7d9df2`  
		Last Modified: Tue, 31 Oct 2023 03:58:48 GMT  
		Size: 384.0 MB (383978199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.13.0-ubi8`

```console
$ docker pull neo4j@sha256:cada68dcf9da0d3c9834a302fe09b7c40e594674eee89b81457efa9e0183424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.13.0-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:7f529f9b883e7508d4d1a47443425886646969b67110faca226ecd6e3d7db0c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0876e68b678eab976554606ae27aabd58cc4db13da7af5ec730f198d334d1`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:09:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:09:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:09:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:02 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:02 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:03 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:03 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdc8bfe48d470191a4f525a0d0a2b2d2df8cf58b607493f4fe27287d41a7e8a`  
		Last Modified: Tue, 31 Oct 2023 03:12:42 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f61cdc434df46bf9943e942b815c6121c056d9a469e1d1ff9b88d8c8ac6b080`  
		Last Modified: Tue, 31 Oct 2023 03:12:49 GMT  
		Size: 112.6 MB (112571528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.13.0-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e852f99034810f3853e7fbd42ccb0207c3cfc7ea9a1cbc9458f169446970d2ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300468610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682e56eb5ed513792f1a3c4c10172712d2e63f8c1737aa35adea5df8ed058dbe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:37 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:37 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:37 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4cf921619b8aac5f90d22a4751c47aee713ce6ccc841fd7091823360a9953`  
		Last Modified: Tue, 31 Oct 2023 03:58:03 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787c30cb8efdf63af7a59c1dc194fc2f186fe59528309cacb4525b7ca4b18ea5`  
		Last Modified: Tue, 31 Oct 2023 03:58:08 GMT  
		Size: 112.6 MB (112571529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:bullseye`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community-bullseye`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community-ubi8`

```console
$ docker pull neo4j@sha256:cada68dcf9da0d3c9834a302fe09b7c40e594674eee89b81457efa9e0183424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:7f529f9b883e7508d4d1a47443425886646969b67110faca226ecd6e3d7db0c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0876e68b678eab976554606ae27aabd58cc4db13da7af5ec730f198d334d1`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:09:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:09:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:09:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:02 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:02 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:03 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:03 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdc8bfe48d470191a4f525a0d0a2b2d2df8cf58b607493f4fe27287d41a7e8a`  
		Last Modified: Tue, 31 Oct 2023 03:12:42 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f61cdc434df46bf9943e942b815c6121c056d9a469e1d1ff9b88d8c8ac6b080`  
		Last Modified: Tue, 31 Oct 2023 03:12:49 GMT  
		Size: 112.6 MB (112571528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e852f99034810f3853e7fbd42ccb0207c3cfc7ea9a1cbc9458f169446970d2ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300468610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682e56eb5ed513792f1a3c4c10172712d2e63f8c1737aa35adea5df8ed058dbe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:37 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:37 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:37 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4cf921619b8aac5f90d22a4751c47aee713ce6ccc841fd7091823360a9953`  
		Last Modified: Tue, 31 Oct 2023 03:58:03 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787c30cb8efdf63af7a59c1dc194fc2f186fe59528309cacb4525b7ca4b18ea5`  
		Last Modified: Tue, 31 Oct 2023 03:58:08 GMT  
		Size: 112.6 MB (112571529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:3ba240f0f98a9dfb36b591658e9976423119ce3c4b0752effeecb436cb79141a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:c06d2e3593ace7b5984247570bc7bfa336afcc347a543f79b7e9593c64608444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.1 MB (564093810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f6974de9e5edca7c27b493cc9a4959fd4f997fe84db8e7cac6ff901e019159`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:50 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:56:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:56:09 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:56:09 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:56:09 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:56:09 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:56:09 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:56:09 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ce05f723ae6f403ba26b5d6efb3209577c09e9d60ec669883c5f799e3240d`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d8e127dcb8291bfb875525eab211a5fea04d223d0df3cd719dcf34821891c8`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7400cfd78a582a74d4a5cbec94f3d6aecb3d03ebd11838a8732505c9d0122`  
		Last Modified: Wed, 01 Nov 2023 11:58:33 GMT  
		Size: 387.8 MB (387788715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bafbdc4ed75df1abbb01b93416a08511aa5189672793d28b01e1b29367ea724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561438922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c834f2faaae66515d6d82c003a5cbf02a5396f8bad78309be9848a5154a9d4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:42:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:16 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:16 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd3e2b17175aa2df8cca1499ca69f75103438a03fa131090a082e671602504b`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78783676f896069de84f62f2fbb011f92359c7445a847918f1a662ed7b1680f1`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 9.4 KB (9420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3705cef4738487a702410b792ca8ff249ed68c9e513072c0c4c2f1e5a320716`  
		Last Modified: Wed, 01 Nov 2023 08:44:18 GMT  
		Size: 387.7 MB (387679965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise-bullseye`

```console
$ docker pull neo4j@sha256:3ba240f0f98a9dfb36b591658e9976423119ce3c4b0752effeecb436cb79141a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:c06d2e3593ace7b5984247570bc7bfa336afcc347a543f79b7e9593c64608444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.1 MB (564093810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f6974de9e5edca7c27b493cc9a4959fd4f997fe84db8e7cac6ff901e019159`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:49 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:50 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:56:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:56:09 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:56:09 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:56:09 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:56:09 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:56:09 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:56:09 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ce05f723ae6f403ba26b5d6efb3209577c09e9d60ec669883c5f799e3240d`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d8e127dcb8291bfb875525eab211a5fea04d223d0df3cd719dcf34821891c8`  
		Last Modified: Wed, 01 Nov 2023 11:58:17 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7400cfd78a582a74d4a5cbec94f3d6aecb3d03ebd11838a8732505c9d0122`  
		Last Modified: Wed, 01 Nov 2023 11:58:33 GMT  
		Size: 387.8 MB (387788715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:0bafbdc4ed75df1abbb01b93416a08511aa5189672793d28b01e1b29367ea724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561438922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c834f2faaae66515d6d82c003a5cbf02a5396f8bad78309be9848a5154a9d4f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:42:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:42:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:42:16 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:42:16 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd3e2b17175aa2df8cca1499ca69f75103438a03fa131090a082e671602504b`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78783676f896069de84f62f2fbb011f92359c7445a847918f1a662ed7b1680f1`  
		Last Modified: Wed, 01 Nov 2023 08:44:03 GMT  
		Size: 9.4 KB (9420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3705cef4738487a702410b792ca8ff249ed68c9e513072c0c4c2f1e5a320716`  
		Last Modified: Wed, 01 Nov 2023 08:44:18 GMT  
		Size: 387.7 MB (387679965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise-ubi8`

```console
$ docker pull neo4j@sha256:fbf58db74d5fb993cd188808ae3a966f0119c4eefce3295fff49abc51fec549d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:a613d5196615fb0090ada8c126151e663bcf6bea31edf2a83570949d49352059
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.7 MB (574691704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8f814c463a4165096f3b6f1fa1836fa16bc3f13ec33011a9d49ecef17805155`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:10:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:10:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:10:07 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:17 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:17 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:17 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:18 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:18 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:18 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d9719156c8861c63c0f3d35884d03cdbfac1b86e31fff24c5c94c7c0baba3c`  
		Last Modified: Tue, 31 Oct 2023 03:13:15 GMT  
		Size: 9.4 KB (9421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b5411e7bd3bb3e8f212dc4a7abbd40cc839cfe7e6a4d0e179570c3ae9f11f8`  
		Last Modified: Tue, 31 Oct 2023 03:13:33 GMT  
		Size: 384.0 MB (383978163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:cbf81ff37755b9cb2196cfe822cb0671bc97bd69bb3cbfff84ad1114cdde5301
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **571.9 MB (571875278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433d59458c2f432f8c0153903d7ff89b6367a36b3088dd0e23fde154581c1bb9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ddb9a8a703e097fe7cb4bb1f13787d38488f61f417397781b020bee71160fb6b NEO4J_TARBALL=neo4j-enterprise-5.13.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:39 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:51 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:51 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:51 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:51 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:51 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9270bb2ee329178be9827cb8f5438ef26e8f5a4a6a5f87bfa19cf97b258ebf64`  
		Last Modified: Tue, 31 Oct 2023 03:58:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d1ebb2e92c7a0041a3eb8cf0052ed6c07948d47d0e86a3b4d99d799e7d9df2`  
		Last Modified: Tue, 31 Oct 2023 03:58:48 GMT  
		Size: 384.0 MB (383978199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:6c96ccbac39e3df54ad8b644b711bf21676af298d044d3b599b2a7c6698143b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:5ee315b1a5612b6d04dfbd8d7f8f14995ab89b545608929cc0a0e4629c391bd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292686931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b803290e47448e96a35678e4aafa61e9f58af663cd5f5cb01080c019a239d44f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:13:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 01:24:07 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Wed, 01 Nov 2023 11:55:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 11:55:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 11:55:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 11:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 11:55:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:55:45 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:55:45 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 11:55:45 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 11:55:45 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 11:55:45 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 11:55:45 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c20750b154d64794fedb0a429e74999708e8bd1d859c9bc36ca5afefa982a25`  
		Last Modified: Wed, 01 Nov 2023 01:40:50 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4801ffbfe587b5d4e7f31ca730126a8b7099f1e440f888493e9a42262c342f5e`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaac3fe4d82efff16465dee15e125d9ee7a113fe049a74c7fbd84dd0c5b2308`  
		Last Modified: Wed, 01 Nov 2023 11:57:33 GMT  
		Size: 9.4 KB (9423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d1ef2b89ee635d18455de23863561edc9b8660e66d7ddd9e644bf5762d3d99`  
		Last Modified: Wed, 01 Nov 2023 11:57:39 GMT  
		Size: 116.4 MB (116381833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:01c3f780c24e264dcb859ee1610108f5c0e861e7783a6a84f4ec6a3ccbcd97d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.0 MB (290034157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c5f0cae401e2b9884bfc62d1d2c318d36e228abbe16fef4fba19682531c2f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:23:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Nov 2023 02:33:06 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Wed, 01 Nov 2023 08:41:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Nov 2023 08:41:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Wed, 01 Nov 2023 08:41:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Nov 2023 08:41:42 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Wed, 01 Nov 2023 08:41:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:41:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 08:41:54 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Nov 2023 08:41:54 GMT
VOLUME [/data /logs]
# Wed, 01 Nov 2023 08:41:54 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Nov 2023 08:41:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:41:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cca082400e47c6a11576684f6f97eebdf67ba34cbf7e1a6a23a5fdf35fbc01`  
		Last Modified: Wed, 01 Nov 2023 02:48:27 GMT  
		Size: 143.7 MB (143681748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c128c58836d3c89f383a49ab6efc432c14cdf627568c99fcb0efaecfac5e3a`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98708aff64b00fff7aba271c111e8ef45dc17d5850350b6402d5305837bd33db`  
		Last Modified: Wed, 01 Nov 2023 08:43:21 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11589975e52917231f324db641a5a86bfde4a33ae01c464fd3d999fcaffc953a`  
		Last Modified: Wed, 01 Nov 2023 08:43:27 GMT  
		Size: 116.3 MB (116275203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:ubi8`

```console
$ docker pull neo4j@sha256:cada68dcf9da0d3c9834a302fe09b7c40e594674eee89b81457efa9e0183424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:7f529f9b883e7508d4d1a47443425886646969b67110faca226ecd6e3d7db0c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0876e68b678eab976554606ae27aabd58cc4db13da7af5ec730f198d334d1`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:5c3db83b000dbd7f5ac652deca0885f748fc3927831292ee77f730ba2f248f5c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:5e368d6e32137dc736d21dd012bd92b380bff4b32507604f02cc3380ed1f27fc in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:9fbad41b814186dd0da1dae5e6ea38418efba78dbf999da629bbf906da226243 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:17:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:09:48 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:09:58 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:09:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:09:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:09:58 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:10:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:10:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:10:02 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:10:02 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:10:03 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:10:03 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:10:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dc35b837139a95d1b9f7f7b0435a024a74ab972416bdc248f3f608c9f917a753`  
		Last Modified: Wed, 18 Oct 2023 21:53:00 GMT  
		Size: 39.3 MB (39307955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853465de20699222566708b0cb06b4069871dad8bcce008ddcbbf0c1bbac40f`  
		Last Modified: Tue, 31 Oct 2023 03:12:54 GMT  
		Size: 144.9 MB (144873899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a62bc2ad4395e9ebe6c929c8e5e13d173c66164b7a20ee8484ab8d7e147ad`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 6.5 MB (6522266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdc8bfe48d470191a4f525a0d0a2b2d2df8cf58b607493f4fe27287d41a7e8a`  
		Last Modified: Tue, 31 Oct 2023 03:12:42 GMT  
		Size: 9.4 KB (9427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f61cdc434df46bf9943e942b815c6121c056d9a469e1d1ff9b88d8c8ac6b080`  
		Last Modified: Tue, 31 Oct 2023 03:12:49 GMT  
		Size: 112.6 MB (112571528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e852f99034810f3853e7fbd42ccb0207c3cfc7ea9a1cbc9458f169446970d2ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300468610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682e56eb5ed513792f1a3c4c10172712d2e63f8c1737aa35adea5df8ed058dbe`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 18 Oct 2023 12:49:52 GMT
ADD file:bb957a9ad1c49f868a6ddca1fc0d1a6d046a4ac78579016c86513ae2697c800c in / 
# Wed, 18 Oct 2023 12:49:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 12:49:53 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 12:49:53 GMT
ADD multi:02c4aafe003795d7be1bd5a3b6d53d7e91c3b729faa5c8f64c2cc816e6915a18 in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.8"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 12:49:53 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 18 Oct 2023 12:49:53 GMT
ENV container oci
# Wed, 18 Oct 2023 12:49:53 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 12:49:53 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 12:49:54 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:c3a7e153dd0c17454a58c2ee7b0344bb6c541bad125e5fd6aafe5502594445c7 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.8-1072.1697626218.json 
# Wed, 18 Oct 2023 12:49:54 GMT
ADD file:09b2a520966e606ac4a7e397becf400ecaebbb4f919dc1153b799e5c5e11e832 in /root/buildinfo/Dockerfile-ubi8-minimal-8.8-1072.1697626218 
# Wed, 18 Oct 2023 12:49:54 GMT
LABEL "release"="1072.1697626218" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:46:11" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="dee8029ddcc7ecbfbebb0905d2b15e134338616c" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.8-1072.1697626218"
# Wed, 18 Oct 2023 12:49:56 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460229-2a53b.repo' '/etc/yum.repos.d/gitweb-f6bee.repo'
# Wed, 18 Oct 2023 12:49:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 12:49:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Sat, 28 Oct 2023 00:14:02 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Oct 2023 03:55:13 GMT
COPY dir:888224b00e9a6a59c49b2cf85eae979985f73b3b17bec354827bf57eb1896417 in /opt/java/openjdk 
# Tue, 31 Oct 2023 03:55:33 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-amd64";             gosusha="3a4e1fc7430f9e7dd7b0cbbe0bfde26bf4a250702e84cf48a1eb2b631c64cf13";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             gosuurl="https://github.com/tianon/gosu/releases/download/1.16/gosu-arm64";             gosusha="23fa49907d5246d2e257de3bf883f57fba47fe1f559f7e732ff16c0f23d2b6a6";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y         findutils         gzip         hostname         jq         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     wget -q ${gosuurl} -O /usr/sbin/gosu;     wget -q  ${gosuurl}.asc -O gosu.asc;     echo "${gosusha}" /usr/sbin/gosu | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     chmod a+x /usr/sbin/gosu;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     gpg --batch --verify gosu.asc /usr/sbin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc gosu.asc;     microdnf clean all
# Tue, 31 Oct 2023 03:55:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c5b1834ae4493af9c623c7d4d68783de1f87d73adea34cd973d9daa3c2ea056c NEO4J_TARBALL=neo4j-community-5.13.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 31 Oct 2023 03:55:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
# Tue, 31 Oct 2023 03:55:33 GMT
COPY multi:b19c74ad2a70cdf4417b1421915c955c79ff7fa1bdf35404eadb22915ea27a8b in /startup/ 
# Tue, 31 Oct 2023 03:55:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.13.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Tue, 31 Oct 2023 03:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:55:37 GMT
WORKDIR /var/lib/neo4j
# Tue, 31 Oct 2023 03:55:37 GMT
VOLUME [/data /logs]
# Tue, 31 Oct 2023 03:55:37 GMT
EXPOSE 7473 7474 7687
# Tue, 31 Oct 2023 03:55:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 31 Oct 2023 03:55:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:4da493486a8e6bed896d94989fd40199cacab25cef2022dc5b72dc9b0be61387`  
		Last Modified: Thu, 19 Oct 2023 07:47:22 GMT  
		Size: 37.7 MB (37689299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fed2ff3e93e200ff72bc61afff6be5f7308927c09ac68cf254714c7fabd2492`  
		Last Modified: Tue, 31 Oct 2023 03:58:12 GMT  
		Size: 143.7 MB (143681766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2deb54bf49d8218d04bbfbd9825b15f7b0149c7ee4c607a2e40a99c1832842`  
		Last Modified: Tue, 31 Oct 2023 03:58:04 GMT  
		Size: 6.5 MB (6516591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4cf921619b8aac5f90d22a4751c47aee713ce6ccc841fd7091823360a9953`  
		Last Modified: Tue, 31 Oct 2023 03:58:03 GMT  
		Size: 9.4 KB (9425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787c30cb8efdf63af7a59c1dc194fc2f186fe59528309cacb4525b7ca4b18ea5`  
		Last Modified: Tue, 31 Oct 2023 03:58:08 GMT  
		Size: 112.6 MB (112571529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
