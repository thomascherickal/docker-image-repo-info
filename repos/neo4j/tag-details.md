<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.3`](#neo4j43)
-	[`neo4j:4.3-community`](#neo4j43-community)
-	[`neo4j:4.3-enterprise`](#neo4j43-enterprise)
-	[`neo4j:4.3.19`](#neo4j4319)
-	[`neo4j:4.3.19-community`](#neo4j4319-community)
-	[`neo4j:4.3.19-enterprise`](#neo4j4319-enterprise)
-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.12`](#neo4j4412)
-	[`neo4j:4.4.12-community`](#neo4j4412-community)
-	[`neo4j:4.4.12-enterprise`](#neo4j4412-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5.1.0`](#neo4j510)
-	[`neo4j:5.1.0-community`](#neo4j510-community)
-	[`neo4j:5.1.0-enterprise`](#neo4j510-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.3`

```console
$ docker pull neo4j@sha256:9f91999433ef87bfac2f9362ec53ecdc90ed784639a306386306fea543a54aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3` - linux; amd64

```console
$ docker pull neo4j@sha256:f4abd08307390cb08ace358a3f743fc23bf814e5035e53d19a14088e5ea76be8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.8 MB (359834403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b8e1ad387463539d92050192276fb25d0f8a8a8a36bfac4cb2695b46998540`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:55:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=55e4dec03a4424933d753387913a38ac2a6100dbfbb1cd976b3958fb8489e3a7 NEO4J_TARBALL=neo4j-community-4.3.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:55:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
# Wed, 02 Nov 2022 20:55:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:55:05 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Wed, 02 Nov 2022 20:55:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:55:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:55:22 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:55:22 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:55:22 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:55:22 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:55:22 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7b69f2c348a39b6cd8688220c9ba99a68d9086cba745b4310e43e17b013bf2`  
		Last Modified: Wed, 02 Nov 2022 20:57:47 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ffa5c86e6a34c74a79eeaef72e14384e7c06e7466ac3d3c89860a1aeba0fa5`  
		Last Modified: Wed, 02 Nov 2022 20:57:46 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9309efad43c990a1d4cffa805307b58fb6b24c2efc0cdc9be16e08ac13fd12e`  
		Last Modified: Wed, 02 Nov 2022 20:57:53 GMT  
		Size: 130.3 MB (130278130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3-community`

```console
$ docker pull neo4j@sha256:9f91999433ef87bfac2f9362ec53ecdc90ed784639a306386306fea543a54aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3-community` - linux; amd64

```console
$ docker pull neo4j@sha256:f4abd08307390cb08ace358a3f743fc23bf814e5035e53d19a14088e5ea76be8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.8 MB (359834403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b8e1ad387463539d92050192276fb25d0f8a8a8a36bfac4cb2695b46998540`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:55:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=55e4dec03a4424933d753387913a38ac2a6100dbfbb1cd976b3958fb8489e3a7 NEO4J_TARBALL=neo4j-community-4.3.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:55:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
# Wed, 02 Nov 2022 20:55:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:55:05 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Wed, 02 Nov 2022 20:55:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:55:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:55:22 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:55:22 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:55:22 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:55:22 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:55:22 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7b69f2c348a39b6cd8688220c9ba99a68d9086cba745b4310e43e17b013bf2`  
		Last Modified: Wed, 02 Nov 2022 20:57:47 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ffa5c86e6a34c74a79eeaef72e14384e7c06e7466ac3d3c89860a1aeba0fa5`  
		Last Modified: Wed, 02 Nov 2022 20:57:46 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9309efad43c990a1d4cffa805307b58fb6b24c2efc0cdc9be16e08ac13fd12e`  
		Last Modified: Wed, 02 Nov 2022 20:57:53 GMT  
		Size: 130.3 MB (130278130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3-enterprise`

```console
$ docker pull neo4j@sha256:18526d06f284409f956a168f98fe7c5910fd660978d08a6e7dab2f6caf6e2f55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:87e0f077a929f3cd88de6829e62e8143e76c82d414a6021734a5d649aa7ea63d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.3 MB (390318593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:495e995fbb7513be28cb94bdde18feec8227ccbbbaa5a3ffb15191bf95bf038f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:55:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4f574dc264853263b865d9c696b389c6dd3e4c9bf7adb84d2f6ac87f907a561c NEO4J_TARBALL=neo4j-enterprise-4.3.19-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:55:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.19-unix.tar.gz
# Wed, 02 Nov 2022 20:55:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:55:29 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Wed, 02 Nov 2022 20:55:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:55:42 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:55:42 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:55:42 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:55:42 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:55:42 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:55:43 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae489abc6a9b6911e5e1bb590a50f7c5a6b3c482b4f910b1a4f956f7777ce55`  
		Last Modified: Wed, 02 Nov 2022 20:58:08 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1843a4ead7d40713414a31a910b7f8e2b379e64c33d618cb566901d55378e0d0`  
		Last Modified: Wed, 02 Nov 2022 20:58:08 GMT  
		Size: 7.6 KB (7629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22de54a9c7471b16fe8b22bccbf6fadc1c80e4404fb52a32ff75ffefdaae4bda`  
		Last Modified: Wed, 02 Nov 2022 20:58:16 GMT  
		Size: 160.8 MB (160762319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.19`

```console
$ docker pull neo4j@sha256:9f91999433ef87bfac2f9362ec53ecdc90ed784639a306386306fea543a54aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.19` - linux; amd64

```console
$ docker pull neo4j@sha256:f4abd08307390cb08ace358a3f743fc23bf814e5035e53d19a14088e5ea76be8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.8 MB (359834403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b8e1ad387463539d92050192276fb25d0f8a8a8a36bfac4cb2695b46998540`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:55:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=55e4dec03a4424933d753387913a38ac2a6100dbfbb1cd976b3958fb8489e3a7 NEO4J_TARBALL=neo4j-community-4.3.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:55:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
# Wed, 02 Nov 2022 20:55:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:55:05 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Wed, 02 Nov 2022 20:55:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:55:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:55:22 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:55:22 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:55:22 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:55:22 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:55:22 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7b69f2c348a39b6cd8688220c9ba99a68d9086cba745b4310e43e17b013bf2`  
		Last Modified: Wed, 02 Nov 2022 20:57:47 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ffa5c86e6a34c74a79eeaef72e14384e7c06e7466ac3d3c89860a1aeba0fa5`  
		Last Modified: Wed, 02 Nov 2022 20:57:46 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9309efad43c990a1d4cffa805307b58fb6b24c2efc0cdc9be16e08ac13fd12e`  
		Last Modified: Wed, 02 Nov 2022 20:57:53 GMT  
		Size: 130.3 MB (130278130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.19-community`

```console
$ docker pull neo4j@sha256:9f91999433ef87bfac2f9362ec53ecdc90ed784639a306386306fea543a54aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.19-community` - linux; amd64

```console
$ docker pull neo4j@sha256:f4abd08307390cb08ace358a3f743fc23bf814e5035e53d19a14088e5ea76be8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.8 MB (359834403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b8e1ad387463539d92050192276fb25d0f8a8a8a36bfac4cb2695b46998540`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:55:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=55e4dec03a4424933d753387913a38ac2a6100dbfbb1cd976b3958fb8489e3a7 NEO4J_TARBALL=neo4j-community-4.3.19-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:55:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
# Wed, 02 Nov 2022 20:55:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:55:05 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Wed, 02 Nov 2022 20:55:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:55:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:55:22 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:55:22 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:55:22 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:55:22 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:55:22 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7b69f2c348a39b6cd8688220c9ba99a68d9086cba745b4310e43e17b013bf2`  
		Last Modified: Wed, 02 Nov 2022 20:57:47 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ffa5c86e6a34c74a79eeaef72e14384e7c06e7466ac3d3c89860a1aeba0fa5`  
		Last Modified: Wed, 02 Nov 2022 20:57:46 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9309efad43c990a1d4cffa805307b58fb6b24c2efc0cdc9be16e08ac13fd12e`  
		Last Modified: Wed, 02 Nov 2022 20:57:53 GMT  
		Size: 130.3 MB (130278130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.19-enterprise`

```console
$ docker pull neo4j@sha256:18526d06f284409f956a168f98fe7c5910fd660978d08a6e7dab2f6caf6e2f55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.19-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:87e0f077a929f3cd88de6829e62e8143e76c82d414a6021734a5d649aa7ea63d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.3 MB (390318593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:495e995fbb7513be28cb94bdde18feec8227ccbbbaa5a3ffb15191bf95bf038f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:55:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4f574dc264853263b865d9c696b389c6dd3e4c9bf7adb84d2f6ac87f907a561c NEO4J_TARBALL=neo4j-enterprise-4.3.19-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:55:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.19-unix.tar.gz
# Wed, 02 Nov 2022 20:55:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.19-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:55:29 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Wed, 02 Nov 2022 20:55:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.19-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:55:42 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:55:42 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:55:42 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:55:42 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:55:42 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:55:43 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae489abc6a9b6911e5e1bb590a50f7c5a6b3c482b4f910b1a4f956f7777ce55`  
		Last Modified: Wed, 02 Nov 2022 20:58:08 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1843a4ead7d40713414a31a910b7f8e2b379e64c33d618cb566901d55378e0d0`  
		Last Modified: Wed, 02 Nov 2022 20:58:08 GMT  
		Size: 7.6 KB (7629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22de54a9c7471b16fe8b22bccbf6fadc1c80e4404fb52a32ff75ffefdaae4bda`  
		Last Modified: Wed, 02 Nov 2022 20:58:16 GMT  
		Size: 160.8 MB (160762319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:35bcc85de971e7e5ef69105912acef1a4a1013630553fac4120ea7ec0f30f11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:661830bcca4c12796f8ca6e24df9f43809fd2ecc0b1ca00d55781b553bc51bcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.7 MB (364702679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a61b292b3ce58c0760f07386656a04dc1dd910b9a4a222386f0cd1f51531adaa`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:54:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=58f2ab847b1898c3f33731dc247784459223185307a4c89757f43ea94eb2a491 NEO4J_TARBALL=neo4j-community-4.4.12-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:54:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 20:54:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:54:21 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 20:54:37 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:54:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:54:38 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:54:38 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:54:38 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:54:38 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:54:38 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116ceae6b055c970f673fef07d088ee976990457f2c744e7f8fa0b79b8a596e8`  
		Last Modified: Wed, 02 Nov 2022 20:56:59 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a45966de65b14bd02ebe7bfb0285a8312cf1925ebd7984ca747ca6864f90c89`  
		Last Modified: Wed, 02 Nov 2022 20:56:58 GMT  
		Size: 7.6 KB (7613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a34a6c86cca952ef18ca7f04c0404c9c3be65e430a0f77884faf729a564f14`  
		Last Modified: Wed, 02 Nov 2022 20:57:10 GMT  
		Size: 135.1 MB (135146421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9ac1b5690f2222edfee31ec722e7dd08c771c05ebe665a87426254fd6767cf24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.9 MB (359947552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b9b994acfdd187c1ab081ab0dc3e74cdb2c5cf0f3bbc011cfccdcae908246bc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:47:12 GMT
COPY dir:e48336735658172388295f760b71f5f10a9b7d3f960c6e4546718a38dd6452e7 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=58f2ab847b1898c3f33731dc247784459223185307a4c89757f43ea94eb2a491 NEO4J_TARBALL=neo4j-community-4.4.12-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 21:26:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:51 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 21:27:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:27:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:27:00 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:27:00 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:27:00 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:27:00 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:27:00 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc966be4bd15170671412b817450394760b037c8e5e3587768bfc3bbd123d53`  
		Last Modified: Wed, 02 Nov 2022 20:58:36 GMT  
		Size: 194.9 MB (194867681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2e7f91c7899cd4df2d383a124d0ade2c0d3c7a1ef389825f0286fef0bdb60`  
		Last Modified: Wed, 02 Nov 2022 21:28:28 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d344aacc94f4c5a28ab3c041385c2a926979091528d2f03c5c2f65da61bed42`  
		Last Modified: Wed, 02 Nov 2022 21:28:28 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1093ac340afa5ad140a5f82ed94ed0769ac95062b13224af1f73065920fa2b`  
		Last Modified: Wed, 02 Nov 2022 21:28:34 GMT  
		Size: 135.0 MB (135004463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:35bcc85de971e7e5ef69105912acef1a4a1013630553fac4120ea7ec0f30f11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:661830bcca4c12796f8ca6e24df9f43809fd2ecc0b1ca00d55781b553bc51bcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.7 MB (364702679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a61b292b3ce58c0760f07386656a04dc1dd910b9a4a222386f0cd1f51531adaa`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:54:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=58f2ab847b1898c3f33731dc247784459223185307a4c89757f43ea94eb2a491 NEO4J_TARBALL=neo4j-community-4.4.12-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:54:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 20:54:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:54:21 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 20:54:37 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:54:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:54:38 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:54:38 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:54:38 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:54:38 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:54:38 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116ceae6b055c970f673fef07d088ee976990457f2c744e7f8fa0b79b8a596e8`  
		Last Modified: Wed, 02 Nov 2022 20:56:59 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a45966de65b14bd02ebe7bfb0285a8312cf1925ebd7984ca747ca6864f90c89`  
		Last Modified: Wed, 02 Nov 2022 20:56:58 GMT  
		Size: 7.6 KB (7613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a34a6c86cca952ef18ca7f04c0404c9c3be65e430a0f77884faf729a564f14`  
		Last Modified: Wed, 02 Nov 2022 20:57:10 GMT  
		Size: 135.1 MB (135146421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9ac1b5690f2222edfee31ec722e7dd08c771c05ebe665a87426254fd6767cf24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.9 MB (359947552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b9b994acfdd187c1ab081ab0dc3e74cdb2c5cf0f3bbc011cfccdcae908246bc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:47:12 GMT
COPY dir:e48336735658172388295f760b71f5f10a9b7d3f960c6e4546718a38dd6452e7 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=58f2ab847b1898c3f33731dc247784459223185307a4c89757f43ea94eb2a491 NEO4J_TARBALL=neo4j-community-4.4.12-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 21:26:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:51 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 21:27:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:27:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:27:00 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:27:00 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:27:00 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:27:00 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:27:00 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc966be4bd15170671412b817450394760b037c8e5e3587768bfc3bbd123d53`  
		Last Modified: Wed, 02 Nov 2022 20:58:36 GMT  
		Size: 194.9 MB (194867681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2e7f91c7899cd4df2d383a124d0ade2c0d3c7a1ef389825f0286fef0bdb60`  
		Last Modified: Wed, 02 Nov 2022 21:28:28 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d344aacc94f4c5a28ab3c041385c2a926979091528d2f03c5c2f65da61bed42`  
		Last Modified: Wed, 02 Nov 2022 21:28:28 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1093ac340afa5ad140a5f82ed94ed0769ac95062b13224af1f73065920fa2b`  
		Last Modified: Wed, 02 Nov 2022 21:28:34 GMT  
		Size: 135.0 MB (135004463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:9b9ea03c553171b3b450290528b62475aae3c7905702aabebdd494f2da97c1da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:faf4b4a423de2ad44cf30f377f46bc3a8737ec2a455d96e0b18e288739d0c9e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459553729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cde5e0d360a7e70cff749a34259d020562e11165c784f3bf2fcd34fdb27a1ef1`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:54:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=f0eff8c70ec5666169803d3d29363b770cd767f5737c8495e2daa3808c87836f NEO4J_TARBALL=neo4j-enterprise-4.4.12-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:54:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 20:54:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:54:45 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 20:55:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:55:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:55:01 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:55:01 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:55:01 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:55:01 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:55:01 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0eb192209530b2472e775a2ec5c48be42f6404c71df93ad355aaa13599ca4f`  
		Last Modified: Wed, 02 Nov 2022 20:57:25 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a6a3eb604cfdcf73b5189168a05d0addad62d0799ce59ac4d8711f8452f18b`  
		Last Modified: Wed, 02 Nov 2022 20:57:25 GMT  
		Size: 7.6 KB (7611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322c35fe82e5c501fdf24bc4d0ea5130b90d22c3d779a331ab31b8ffd52e5360`  
		Last Modified: Wed, 02 Nov 2022 20:57:37 GMT  
		Size: 230.0 MB (229997470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:bbcee1a96f2d47be11e2acd64c7d7423c30acb0f744ef2ef4accb485c168ea95
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.8 MB (454799686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d36f01f86d4b7b230e1807f00e6075ab7f394e5b0322fca09e92c5ef31c47d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:47:12 GMT
COPY dir:e48336735658172388295f760b71f5f10a9b7d3f960c6e4546718a38dd6452e7 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:27:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=f0eff8c70ec5666169803d3d29363b770cd767f5737c8495e2daa3808c87836f NEO4J_TARBALL=neo4j-enterprise-4.4.12-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:27:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 21:27:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:27:05 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 21:27:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:27:20 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:27:20 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:27:20 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:27:20 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:27:20 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:27:20 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc966be4bd15170671412b817450394760b037c8e5e3587768bfc3bbd123d53`  
		Last Modified: Wed, 02 Nov 2022 20:58:36 GMT  
		Size: 194.9 MB (194867681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ded0e4793c2fb9fc8bc921cf2dd6e25c0459db77446175b77e8a6452def8a48`  
		Last Modified: Wed, 02 Nov 2022 21:28:48 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475f174dc382df1ce0fa288c28cd7b70b044f1a13d06d1100c46eb938df55fdd`  
		Last Modified: Wed, 02 Nov 2022 21:28:48 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce3d3d1adcad9de8efb1e631f777f9b886852ab6689068f8c8364199c6799bb`  
		Last Modified: Wed, 02 Nov 2022 21:28:58 GMT  
		Size: 229.9 MB (229856589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.12`

```console
$ docker pull neo4j@sha256:35bcc85de971e7e5ef69105912acef1a4a1013630553fac4120ea7ec0f30f11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.12` - linux; amd64

```console
$ docker pull neo4j@sha256:661830bcca4c12796f8ca6e24df9f43809fd2ecc0b1ca00d55781b553bc51bcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.7 MB (364702679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a61b292b3ce58c0760f07386656a04dc1dd910b9a4a222386f0cd1f51531adaa`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:54:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=58f2ab847b1898c3f33731dc247784459223185307a4c89757f43ea94eb2a491 NEO4J_TARBALL=neo4j-community-4.4.12-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:54:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 20:54:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:54:21 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 20:54:37 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:54:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:54:38 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:54:38 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:54:38 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:54:38 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:54:38 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116ceae6b055c970f673fef07d088ee976990457f2c744e7f8fa0b79b8a596e8`  
		Last Modified: Wed, 02 Nov 2022 20:56:59 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a45966de65b14bd02ebe7bfb0285a8312cf1925ebd7984ca747ca6864f90c89`  
		Last Modified: Wed, 02 Nov 2022 20:56:58 GMT  
		Size: 7.6 KB (7613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a34a6c86cca952ef18ca7f04c0404c9c3be65e430a0f77884faf729a564f14`  
		Last Modified: Wed, 02 Nov 2022 20:57:10 GMT  
		Size: 135.1 MB (135146421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.12` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9ac1b5690f2222edfee31ec722e7dd08c771c05ebe665a87426254fd6767cf24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.9 MB (359947552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b9b994acfdd187c1ab081ab0dc3e74cdb2c5cf0f3bbc011cfccdcae908246bc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:47:12 GMT
COPY dir:e48336735658172388295f760b71f5f10a9b7d3f960c6e4546718a38dd6452e7 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=58f2ab847b1898c3f33731dc247784459223185307a4c89757f43ea94eb2a491 NEO4J_TARBALL=neo4j-community-4.4.12-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 21:26:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:51 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 21:27:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:27:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:27:00 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:27:00 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:27:00 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:27:00 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:27:00 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc966be4bd15170671412b817450394760b037c8e5e3587768bfc3bbd123d53`  
		Last Modified: Wed, 02 Nov 2022 20:58:36 GMT  
		Size: 194.9 MB (194867681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2e7f91c7899cd4df2d383a124d0ade2c0d3c7a1ef389825f0286fef0bdb60`  
		Last Modified: Wed, 02 Nov 2022 21:28:28 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d344aacc94f4c5a28ab3c041385c2a926979091528d2f03c5c2f65da61bed42`  
		Last Modified: Wed, 02 Nov 2022 21:28:28 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1093ac340afa5ad140a5f82ed94ed0769ac95062b13224af1f73065920fa2b`  
		Last Modified: Wed, 02 Nov 2022 21:28:34 GMT  
		Size: 135.0 MB (135004463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.12-community`

```console
$ docker pull neo4j@sha256:35bcc85de971e7e5ef69105912acef1a4a1013630553fac4120ea7ec0f30f11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.12-community` - linux; amd64

```console
$ docker pull neo4j@sha256:661830bcca4c12796f8ca6e24df9f43809fd2ecc0b1ca00d55781b553bc51bcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.7 MB (364702679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a61b292b3ce58c0760f07386656a04dc1dd910b9a4a222386f0cd1f51531adaa`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:54:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=58f2ab847b1898c3f33731dc247784459223185307a4c89757f43ea94eb2a491 NEO4J_TARBALL=neo4j-community-4.4.12-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:54:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 20:54:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:54:21 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 20:54:37 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:54:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:54:38 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:54:38 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:54:38 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:54:38 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:54:38 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116ceae6b055c970f673fef07d088ee976990457f2c744e7f8fa0b79b8a596e8`  
		Last Modified: Wed, 02 Nov 2022 20:56:59 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a45966de65b14bd02ebe7bfb0285a8312cf1925ebd7984ca747ca6864f90c89`  
		Last Modified: Wed, 02 Nov 2022 20:56:58 GMT  
		Size: 7.6 KB (7613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a34a6c86cca952ef18ca7f04c0404c9c3be65e430a0f77884faf729a564f14`  
		Last Modified: Wed, 02 Nov 2022 20:57:10 GMT  
		Size: 135.1 MB (135146421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.12-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:9ac1b5690f2222edfee31ec722e7dd08c771c05ebe665a87426254fd6767cf24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.9 MB (359947552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b9b994acfdd187c1ab081ab0dc3e74cdb2c5cf0f3bbc011cfccdcae908246bc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:47:12 GMT
COPY dir:e48336735658172388295f760b71f5f10a9b7d3f960c6e4546718a38dd6452e7 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=58f2ab847b1898c3f33731dc247784459223185307a4c89757f43ea94eb2a491 NEO4J_TARBALL=neo4j-community-4.4.12-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 21:26:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:51 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 21:27:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:27:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:27:00 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:27:00 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:27:00 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:27:00 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:27:00 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc966be4bd15170671412b817450394760b037c8e5e3587768bfc3bbd123d53`  
		Last Modified: Wed, 02 Nov 2022 20:58:36 GMT  
		Size: 194.9 MB (194867681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2e7f91c7899cd4df2d383a124d0ade2c0d3c7a1ef389825f0286fef0bdb60`  
		Last Modified: Wed, 02 Nov 2022 21:28:28 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d344aacc94f4c5a28ab3c041385c2a926979091528d2f03c5c2f65da61bed42`  
		Last Modified: Wed, 02 Nov 2022 21:28:28 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1093ac340afa5ad140a5f82ed94ed0769ac95062b13224af1f73065920fa2b`  
		Last Modified: Wed, 02 Nov 2022 21:28:34 GMT  
		Size: 135.0 MB (135004463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.12-enterprise`

```console
$ docker pull neo4j@sha256:9b9ea03c553171b3b450290528b62475aae3c7905702aabebdd494f2da97c1da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.12-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:faf4b4a423de2ad44cf30f377f46bc3a8737ec2a455d96e0b18e288739d0c9e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459553729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cde5e0d360a7e70cff749a34259d020562e11165c784f3bf2fcd34fdb27a1ef1`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:54:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=f0eff8c70ec5666169803d3d29363b770cd767f5737c8495e2daa3808c87836f NEO4J_TARBALL=neo4j-enterprise-4.4.12-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:54:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 20:54:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:54:45 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 20:55:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:55:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:55:01 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:55:01 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:55:01 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:55:01 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:55:01 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0eb192209530b2472e775a2ec5c48be42f6404c71df93ad355aaa13599ca4f`  
		Last Modified: Wed, 02 Nov 2022 20:57:25 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a6a3eb604cfdcf73b5189168a05d0addad62d0799ce59ac4d8711f8452f18b`  
		Last Modified: Wed, 02 Nov 2022 20:57:25 GMT  
		Size: 7.6 KB (7611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322c35fe82e5c501fdf24bc4d0ea5130b90d22c3d779a331ab31b8ffd52e5360`  
		Last Modified: Wed, 02 Nov 2022 20:57:37 GMT  
		Size: 230.0 MB (229997470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.12-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:bbcee1a96f2d47be11e2acd64c7d7423c30acb0f744ef2ef4accb485c168ea95
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.8 MB (454799686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d36f01f86d4b7b230e1807f00e6075ab7f394e5b0322fca09e92c5ef31c47d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:47:12 GMT
COPY dir:e48336735658172388295f760b71f5f10a9b7d3f960c6e4546718a38dd6452e7 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:27:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=f0eff8c70ec5666169803d3d29363b770cd767f5737c8495e2daa3808c87836f NEO4J_TARBALL=neo4j-enterprise-4.4.12-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:27:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
# Wed, 02 Nov 2022 21:27:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:27:05 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 02 Nov 2022 21:27:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:27:20 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:27:20 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:27:20 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:27:20 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:27:20 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:27:20 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc966be4bd15170671412b817450394760b037c8e5e3587768bfc3bbd123d53`  
		Last Modified: Wed, 02 Nov 2022 20:58:36 GMT  
		Size: 194.9 MB (194867681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ded0e4793c2fb9fc8bc921cf2dd6e25c0459db77446175b77e8a6452def8a48`  
		Last Modified: Wed, 02 Nov 2022 21:28:48 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475f174dc382df1ce0fa288c28cd7b70b044f1a13d06d1100c46eb938df55fdd`  
		Last Modified: Wed, 02 Nov 2022 21:28:48 GMT  
		Size: 7.6 KB (7612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce3d3d1adcad9de8efb1e631f777f9b886852ab6689068f8c8364199c6799bb`  
		Last Modified: Wed, 02 Nov 2022 21:28:58 GMT  
		Size: 229.9 MB (229856589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:fc99f5721a0badff3376526670a25a71f524dabb48f19ca383c1d2ff5db3c9b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:b780c8381e7f1ab5ca8fe737276dbefbe7525bbd31cdc009b5d3810938dcba26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334277794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b92f0b7f95023408457dd46c1832f690f17828af1ec34a4a2b5328f2f2e0ce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:15:23 GMT
COPY dir:58adc2a0817e042696a68e5783ea1d9db89b18bd838f66f2ddc3c99acbc84106 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:53:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:53:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 20:53:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:53:41 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 20:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:53:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:53:55 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:53:55 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:53:55 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:53:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:53:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b9477aacca86981c880c8ed7c4dbb56574cdcda91a39effa9c2332b96765`  
		Last Modified: Wed, 02 Nov 2022 20:27:47 GMT  
		Size: 192.1 MB (192137557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3112b4ae6e1a6961c3b59de4b733095baef2a2ac136c1fad7d9c2ae6c42492d`  
		Last Modified: Wed, 02 Nov 2022 20:56:11 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c89cfb52d22682f78babb4c91e0091ab16e91e38a29acbcc8a924c6e0a2059`  
		Last Modified: Wed, 02 Nov 2022 20:56:12 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129efcacc87bccae32585727944036d41362d927953efc157220609baa63f6ec`  
		Last Modified: Wed, 02 Nov 2022 20:56:18 GMT  
		Size: 110.7 MB (110708707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:26c2bac6ae0667ebbae325805848a20b6037c7ed6d450190d97db28091be20b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331545745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86073f4afd276e313eac90b043f954f932c77e8eb1a843a26bfdc24206cbcb9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:50:40 GMT
COPY dir:527d7e3a362e3a52ce4ecffbf599fb9423f60f5fcdccc64d800fcfec8666f5b8 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 21:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 21:26:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:26:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:26:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:26:29 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:26:30 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:26:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:26:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c78a656ff98cd4a277e3c01f4d0eb067085f7d111e0f4a4c913c75ed384c0`  
		Last Modified: Wed, 02 Nov 2022 21:01:35 GMT  
		Size: 190.9 MB (190904092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449edc3d08e467ce37d14ad7fa99aac6b03a0517ba1199eff5c63e54cf7add1c`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b0f871a10e6921abeb9ee66ec6092c30fca9379c1f7f428047eb46ff850cf`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c44bbd671eb7f05a3596c9a2ed39098a38c3b7ec17520fcd09550a3cec5fd`  
		Last Modified: Wed, 02 Nov 2022 21:27:47 GMT  
		Size: 110.6 MB (110566224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:fc99f5721a0badff3376526670a25a71f524dabb48f19ca383c1d2ff5db3c9b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:b780c8381e7f1ab5ca8fe737276dbefbe7525bbd31cdc009b5d3810938dcba26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334277794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b92f0b7f95023408457dd46c1832f690f17828af1ec34a4a2b5328f2f2e0ce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:15:23 GMT
COPY dir:58adc2a0817e042696a68e5783ea1d9db89b18bd838f66f2ddc3c99acbc84106 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:53:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:53:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 20:53:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:53:41 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 20:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:53:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:53:55 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:53:55 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:53:55 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:53:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:53:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b9477aacca86981c880c8ed7c4dbb56574cdcda91a39effa9c2332b96765`  
		Last Modified: Wed, 02 Nov 2022 20:27:47 GMT  
		Size: 192.1 MB (192137557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3112b4ae6e1a6961c3b59de4b733095baef2a2ac136c1fad7d9c2ae6c42492d`  
		Last Modified: Wed, 02 Nov 2022 20:56:11 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c89cfb52d22682f78babb4c91e0091ab16e91e38a29acbcc8a924c6e0a2059`  
		Last Modified: Wed, 02 Nov 2022 20:56:12 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129efcacc87bccae32585727944036d41362d927953efc157220609baa63f6ec`  
		Last Modified: Wed, 02 Nov 2022 20:56:18 GMT  
		Size: 110.7 MB (110708707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:26c2bac6ae0667ebbae325805848a20b6037c7ed6d450190d97db28091be20b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331545745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86073f4afd276e313eac90b043f954f932c77e8eb1a843a26bfdc24206cbcb9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:50:40 GMT
COPY dir:527d7e3a362e3a52ce4ecffbf599fb9423f60f5fcdccc64d800fcfec8666f5b8 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 21:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 21:26:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:26:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:26:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:26:29 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:26:30 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:26:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:26:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c78a656ff98cd4a277e3c01f4d0eb067085f7d111e0f4a4c913c75ed384c0`  
		Last Modified: Wed, 02 Nov 2022 21:01:35 GMT  
		Size: 190.9 MB (190904092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449edc3d08e467ce37d14ad7fa99aac6b03a0517ba1199eff5c63e54cf7add1c`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b0f871a10e6921abeb9ee66ec6092c30fca9379c1f7f428047eb46ff850cf`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c44bbd671eb7f05a3596c9a2ed39098a38c3b7ec17520fcd09550a3cec5fd`  
		Last Modified: Wed, 02 Nov 2022 21:27:47 GMT  
		Size: 110.6 MB (110566224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:e021c6e0e7534db9b8190feebc1d5dc26d6f7283ac590cdc44cfc8ab86431df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b34e1e719be447231403dd94cfd345a05c8a392d41151e9793b982e6592f0000
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.9 MB (429865976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f220f6cd2b3afd2d99fa59ceaa3fc9b76744d78c90be6021ecd5e5948b5f4243`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:15:23 GMT
COPY dir:58adc2a0817e042696a68e5783ea1d9db89b18bd838f66f2ddc3c99acbc84106 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:54:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:54:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 20:54:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:54:01 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 20:54:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:54:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:54:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:54:17 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:54:17 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:54:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:54:17 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b9477aacca86981c880c8ed7c4dbb56574cdcda91a39effa9c2332b96765`  
		Last Modified: Wed, 02 Nov 2022 20:27:47 GMT  
		Size: 192.1 MB (192137557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ddfe1fdeacf2ea67e79bc3abace5904dfd7dcd636be30d00a78f9ba919503`  
		Last Modified: Wed, 02 Nov 2022 20:56:36 GMT  
		Size: 3.9 KB (3868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe1ea32a9edbccfd04f44d1138b64863fd3af16c0ab459d6419d3deef9f92b1`  
		Last Modified: Wed, 02 Nov 2022 20:56:36 GMT  
		Size: 7.6 KB (7627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a228a3b945ff6c7b8b12c705b99f868be49a7b05748b4d73cde910ab6dbb2907`  
		Last Modified: Wed, 02 Nov 2022 20:56:46 GMT  
		Size: 206.3 MB (206296886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e3119bcd62fcef09e8864f6517b712b5296de5f58fe177e627a6698200cf7d74
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.1 MB (427132945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e695ccc82a44afd052c6eda03ebac0950167bdfc0e110c6b40f1528a146c85a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:50:40 GMT
COPY dir:527d7e3a362e3a52ce4ecffbf599fb9423f60f5fcdccc64d800fcfec8666f5b8 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 21:26:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:34 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 21:26:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:26:46 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:26:46 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:26:46 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c78a656ff98cd4a277e3c01f4d0eb067085f7d111e0f4a4c913c75ed384c0`  
		Last Modified: Wed, 02 Nov 2022 21:01:35 GMT  
		Size: 190.9 MB (190904092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1593c15c9163d2ee4a4e2391f77ac55b9c01f8f67f9c93dd104d15c108b16`  
		Last Modified: Wed, 02 Nov 2022 21:28:07 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33595905568863e78756e67cc0a78b42d4c5b7a0a84f6be00a47fa1ed511c2f`  
		Last Modified: Wed, 02 Nov 2022 21:28:07 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8773f8e2c7db03b2d9ded50475c64fc817c364574216c5f4c96a68dd02557a95`  
		Last Modified: Wed, 02 Nov 2022 21:28:15 GMT  
		Size: 206.2 MB (206153423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.1.0`

```console
$ docker pull neo4j@sha256:fc99f5721a0badff3376526670a25a71f524dabb48f19ca383c1d2ff5db3c9b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.1.0` - linux; amd64

```console
$ docker pull neo4j@sha256:b780c8381e7f1ab5ca8fe737276dbefbe7525bbd31cdc009b5d3810938dcba26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334277794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b92f0b7f95023408457dd46c1832f690f17828af1ec34a4a2b5328f2f2e0ce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:15:23 GMT
COPY dir:58adc2a0817e042696a68e5783ea1d9db89b18bd838f66f2ddc3c99acbc84106 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:53:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:53:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 20:53:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:53:41 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 20:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:53:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:53:55 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:53:55 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:53:55 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:53:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:53:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b9477aacca86981c880c8ed7c4dbb56574cdcda91a39effa9c2332b96765`  
		Last Modified: Wed, 02 Nov 2022 20:27:47 GMT  
		Size: 192.1 MB (192137557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3112b4ae6e1a6961c3b59de4b733095baef2a2ac136c1fad7d9c2ae6c42492d`  
		Last Modified: Wed, 02 Nov 2022 20:56:11 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c89cfb52d22682f78babb4c91e0091ab16e91e38a29acbcc8a924c6e0a2059`  
		Last Modified: Wed, 02 Nov 2022 20:56:12 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129efcacc87bccae32585727944036d41362d927953efc157220609baa63f6ec`  
		Last Modified: Wed, 02 Nov 2022 20:56:18 GMT  
		Size: 110.7 MB (110708707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.1.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:26c2bac6ae0667ebbae325805848a20b6037c7ed6d450190d97db28091be20b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331545745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86073f4afd276e313eac90b043f954f932c77e8eb1a843a26bfdc24206cbcb9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:50:40 GMT
COPY dir:527d7e3a362e3a52ce4ecffbf599fb9423f60f5fcdccc64d800fcfec8666f5b8 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 21:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 21:26:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:26:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:26:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:26:29 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:26:30 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:26:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:26:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c78a656ff98cd4a277e3c01f4d0eb067085f7d111e0f4a4c913c75ed384c0`  
		Last Modified: Wed, 02 Nov 2022 21:01:35 GMT  
		Size: 190.9 MB (190904092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449edc3d08e467ce37d14ad7fa99aac6b03a0517ba1199eff5c63e54cf7add1c`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b0f871a10e6921abeb9ee66ec6092c30fca9379c1f7f428047eb46ff850cf`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c44bbd671eb7f05a3596c9a2ed39098a38c3b7ec17520fcd09550a3cec5fd`  
		Last Modified: Wed, 02 Nov 2022 21:27:47 GMT  
		Size: 110.6 MB (110566224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.1.0-community`

```console
$ docker pull neo4j@sha256:fc99f5721a0badff3376526670a25a71f524dabb48f19ca383c1d2ff5db3c9b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.1.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:b780c8381e7f1ab5ca8fe737276dbefbe7525bbd31cdc009b5d3810938dcba26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334277794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b92f0b7f95023408457dd46c1832f690f17828af1ec34a4a2b5328f2f2e0ce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:15:23 GMT
COPY dir:58adc2a0817e042696a68e5783ea1d9db89b18bd838f66f2ddc3c99acbc84106 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:53:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:53:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 20:53:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:53:41 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 20:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:53:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:53:55 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:53:55 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:53:55 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:53:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:53:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b9477aacca86981c880c8ed7c4dbb56574cdcda91a39effa9c2332b96765`  
		Last Modified: Wed, 02 Nov 2022 20:27:47 GMT  
		Size: 192.1 MB (192137557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3112b4ae6e1a6961c3b59de4b733095baef2a2ac136c1fad7d9c2ae6c42492d`  
		Last Modified: Wed, 02 Nov 2022 20:56:11 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c89cfb52d22682f78babb4c91e0091ab16e91e38a29acbcc8a924c6e0a2059`  
		Last Modified: Wed, 02 Nov 2022 20:56:12 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129efcacc87bccae32585727944036d41362d927953efc157220609baa63f6ec`  
		Last Modified: Wed, 02 Nov 2022 20:56:18 GMT  
		Size: 110.7 MB (110708707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.1.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:26c2bac6ae0667ebbae325805848a20b6037c7ed6d450190d97db28091be20b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331545745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86073f4afd276e313eac90b043f954f932c77e8eb1a843a26bfdc24206cbcb9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:50:40 GMT
COPY dir:527d7e3a362e3a52ce4ecffbf599fb9423f60f5fcdccc64d800fcfec8666f5b8 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 21:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 21:26:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:26:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:26:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:26:29 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:26:30 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:26:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:26:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c78a656ff98cd4a277e3c01f4d0eb067085f7d111e0f4a4c913c75ed384c0`  
		Last Modified: Wed, 02 Nov 2022 21:01:35 GMT  
		Size: 190.9 MB (190904092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449edc3d08e467ce37d14ad7fa99aac6b03a0517ba1199eff5c63e54cf7add1c`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b0f871a10e6921abeb9ee66ec6092c30fca9379c1f7f428047eb46ff850cf`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c44bbd671eb7f05a3596c9a2ed39098a38c3b7ec17520fcd09550a3cec5fd`  
		Last Modified: Wed, 02 Nov 2022 21:27:47 GMT  
		Size: 110.6 MB (110566224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.1.0-enterprise`

```console
$ docker pull neo4j@sha256:e021c6e0e7534db9b8190feebc1d5dc26d6f7283ac590cdc44cfc8ab86431df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.1.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b34e1e719be447231403dd94cfd345a05c8a392d41151e9793b982e6592f0000
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.9 MB (429865976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f220f6cd2b3afd2d99fa59ceaa3fc9b76744d78c90be6021ecd5e5948b5f4243`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:15:23 GMT
COPY dir:58adc2a0817e042696a68e5783ea1d9db89b18bd838f66f2ddc3c99acbc84106 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:54:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:54:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 20:54:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:54:01 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 20:54:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:54:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:54:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:54:17 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:54:17 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:54:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:54:17 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b9477aacca86981c880c8ed7c4dbb56574cdcda91a39effa9c2332b96765`  
		Last Modified: Wed, 02 Nov 2022 20:27:47 GMT  
		Size: 192.1 MB (192137557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ddfe1fdeacf2ea67e79bc3abace5904dfd7dcd636be30d00a78f9ba919503`  
		Last Modified: Wed, 02 Nov 2022 20:56:36 GMT  
		Size: 3.9 KB (3868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe1ea32a9edbccfd04f44d1138b64863fd3af16c0ab459d6419d3deef9f92b1`  
		Last Modified: Wed, 02 Nov 2022 20:56:36 GMT  
		Size: 7.6 KB (7627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a228a3b945ff6c7b8b12c705b99f868be49a7b05748b4d73cde910ab6dbb2907`  
		Last Modified: Wed, 02 Nov 2022 20:56:46 GMT  
		Size: 206.3 MB (206296886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.1.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e3119bcd62fcef09e8864f6517b712b5296de5f58fe177e627a6698200cf7d74
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.1 MB (427132945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e695ccc82a44afd052c6eda03ebac0950167bdfc0e110c6b40f1528a146c85a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:50:40 GMT
COPY dir:527d7e3a362e3a52ce4ecffbf599fb9423f60f5fcdccc64d800fcfec8666f5b8 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 21:26:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:34 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 21:26:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:26:46 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:26:46 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:26:46 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c78a656ff98cd4a277e3c01f4d0eb067085f7d111e0f4a4c913c75ed384c0`  
		Last Modified: Wed, 02 Nov 2022 21:01:35 GMT  
		Size: 190.9 MB (190904092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1593c15c9163d2ee4a4e2391f77ac55b9c01f8f67f9c93dd104d15c108b16`  
		Last Modified: Wed, 02 Nov 2022 21:28:07 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33595905568863e78756e67cc0a78b42d4c5b7a0a84f6be00a47fa1ed511c2f`  
		Last Modified: Wed, 02 Nov 2022 21:28:07 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8773f8e2c7db03b2d9ded50475c64fc817c364574216c5f4c96a68dd02557a95`  
		Last Modified: Wed, 02 Nov 2022 21:28:15 GMT  
		Size: 206.2 MB (206153423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:fc99f5721a0badff3376526670a25a71f524dabb48f19ca383c1d2ff5db3c9b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:b780c8381e7f1ab5ca8fe737276dbefbe7525bbd31cdc009b5d3810938dcba26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334277794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b92f0b7f95023408457dd46c1832f690f17828af1ec34a4a2b5328f2f2e0ce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:15:23 GMT
COPY dir:58adc2a0817e042696a68e5783ea1d9db89b18bd838f66f2ddc3c99acbc84106 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:53:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:53:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 20:53:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:53:41 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 20:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:53:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:53:55 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:53:55 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:53:55 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:53:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:53:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b9477aacca86981c880c8ed7c4dbb56574cdcda91a39effa9c2332b96765`  
		Last Modified: Wed, 02 Nov 2022 20:27:47 GMT  
		Size: 192.1 MB (192137557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3112b4ae6e1a6961c3b59de4b733095baef2a2ac136c1fad7d9c2ae6c42492d`  
		Last Modified: Wed, 02 Nov 2022 20:56:11 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c89cfb52d22682f78babb4c91e0091ab16e91e38a29acbcc8a924c6e0a2059`  
		Last Modified: Wed, 02 Nov 2022 20:56:12 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129efcacc87bccae32585727944036d41362d927953efc157220609baa63f6ec`  
		Last Modified: Wed, 02 Nov 2022 20:56:18 GMT  
		Size: 110.7 MB (110708707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:26c2bac6ae0667ebbae325805848a20b6037c7ed6d450190d97db28091be20b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331545745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86073f4afd276e313eac90b043f954f932c77e8eb1a843a26bfdc24206cbcb9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:50:40 GMT
COPY dir:527d7e3a362e3a52ce4ecffbf599fb9423f60f5fcdccc64d800fcfec8666f5b8 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 21:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 21:26:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:26:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:26:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:26:29 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:26:30 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:26:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:26:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c78a656ff98cd4a277e3c01f4d0eb067085f7d111e0f4a4c913c75ed384c0`  
		Last Modified: Wed, 02 Nov 2022 21:01:35 GMT  
		Size: 190.9 MB (190904092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449edc3d08e467ce37d14ad7fa99aac6b03a0517ba1199eff5c63e54cf7add1c`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b0f871a10e6921abeb9ee66ec6092c30fca9379c1f7f428047eb46ff850cf`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c44bbd671eb7f05a3596c9a2ed39098a38c3b7ec17520fcd09550a3cec5fd`  
		Last Modified: Wed, 02 Nov 2022 21:27:47 GMT  
		Size: 110.6 MB (110566224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:e021c6e0e7534db9b8190feebc1d5dc26d6f7283ac590cdc44cfc8ab86431df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b34e1e719be447231403dd94cfd345a05c8a392d41151e9793b982e6592f0000
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.9 MB (429865976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f220f6cd2b3afd2d99fa59ceaa3fc9b76744d78c90be6021ecd5e5948b5f4243`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:15:23 GMT
COPY dir:58adc2a0817e042696a68e5783ea1d9db89b18bd838f66f2ddc3c99acbc84106 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:54:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:54:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 20:54:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:54:01 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 20:54:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:54:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:54:16 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:54:17 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:54:17 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:54:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:54:17 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b9477aacca86981c880c8ed7c4dbb56574cdcda91a39effa9c2332b96765`  
		Last Modified: Wed, 02 Nov 2022 20:27:47 GMT  
		Size: 192.1 MB (192137557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ddfe1fdeacf2ea67e79bc3abace5904dfd7dcd636be30d00a78f9ba919503`  
		Last Modified: Wed, 02 Nov 2022 20:56:36 GMT  
		Size: 3.9 KB (3868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe1ea32a9edbccfd04f44d1138b64863fd3af16c0ab459d6419d3deef9f92b1`  
		Last Modified: Wed, 02 Nov 2022 20:56:36 GMT  
		Size: 7.6 KB (7627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a228a3b945ff6c7b8b12c705b99f868be49a7b05748b4d73cde910ab6dbb2907`  
		Last Modified: Wed, 02 Nov 2022 20:56:46 GMT  
		Size: 206.3 MB (206296886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e3119bcd62fcef09e8864f6517b712b5296de5f58fe177e627a6698200cf7d74
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.1 MB (427132945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e695ccc82a44afd052c6eda03ebac0950167bdfc0e110c6b40f1528a146c85a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:50:40 GMT
COPY dir:527d7e3a362e3a52ce4ecffbf599fb9423f60f5fcdccc64d800fcfec8666f5b8 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 21:26:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:34 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 21:26:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:26:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:26:46 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:26:46 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:26:46 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:26:46 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:26:46 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c78a656ff98cd4a277e3c01f4d0eb067085f7d111e0f4a4c913c75ed384c0`  
		Last Modified: Wed, 02 Nov 2022 21:01:35 GMT  
		Size: 190.9 MB (190904092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1593c15c9163d2ee4a4e2391f77ac55b9c01f8f67f9c93dd104d15c108b16`  
		Last Modified: Wed, 02 Nov 2022 21:28:07 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33595905568863e78756e67cc0a78b42d4c5b7a0a84f6be00a47fa1ed511c2f`  
		Last Modified: Wed, 02 Nov 2022 21:28:07 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8773f8e2c7db03b2d9ded50475c64fc817c364574216c5f4c96a68dd02557a95`  
		Last Modified: Wed, 02 Nov 2022 21:28:15 GMT  
		Size: 206.2 MB (206153423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:fc99f5721a0badff3376526670a25a71f524dabb48f19ca383c1d2ff5db3c9b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:b780c8381e7f1ab5ca8fe737276dbefbe7525bbd31cdc009b5d3810938dcba26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334277794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b92f0b7f95023408457dd46c1832f690f17828af1ec34a4a2b5328f2f2e0ce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:15:23 GMT
COPY dir:58adc2a0817e042696a68e5783ea1d9db89b18bd838f66f2ddc3c99acbc84106 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:53:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:53:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 20:53:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:53:41 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 20:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:53:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:53:55 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:53:55 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:53:55 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:53:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:53:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b9477aacca86981c880c8ed7c4dbb56574cdcda91a39effa9c2332b96765`  
		Last Modified: Wed, 02 Nov 2022 20:27:47 GMT  
		Size: 192.1 MB (192137557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3112b4ae6e1a6961c3b59de4b733095baef2a2ac136c1fad7d9c2ae6c42492d`  
		Last Modified: Wed, 02 Nov 2022 20:56:11 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c89cfb52d22682f78babb4c91e0091ab16e91e38a29acbcc8a924c6e0a2059`  
		Last Modified: Wed, 02 Nov 2022 20:56:12 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129efcacc87bccae32585727944036d41362d927953efc157220609baa63f6ec`  
		Last Modified: Wed, 02 Nov 2022 20:56:18 GMT  
		Size: 110.7 MB (110708707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:26c2bac6ae0667ebbae325805848a20b6037c7ed6d450190d97db28091be20b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331545745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86073f4afd276e313eac90b043f954f932c77e8eb1a843a26bfdc24206cbcb9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:50:40 GMT
COPY dir:527d7e3a362e3a52ce4ecffbf599fb9423f60f5fcdccc64d800fcfec8666f5b8 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 21:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 21:26:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:26:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:26:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:26:29 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:26:30 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:26:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:26:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c78a656ff98cd4a277e3c01f4d0eb067085f7d111e0f4a4c913c75ed384c0`  
		Last Modified: Wed, 02 Nov 2022 21:01:35 GMT  
		Size: 190.9 MB (190904092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449edc3d08e467ce37d14ad7fa99aac6b03a0517ba1199eff5c63e54cf7add1c`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b0f871a10e6921abeb9ee66ec6092c30fca9379c1f7f428047eb46ff850cf`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c44bbd671eb7f05a3596c9a2ed39098a38c3b7ec17520fcd09550a3cec5fd`  
		Last Modified: Wed, 02 Nov 2022 21:27:47 GMT  
		Size: 110.6 MB (110566224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
