<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.3`](#neo4j43)
-	[`neo4j:4.3-community`](#neo4j43-community)
-	[`neo4j:4.3-enterprise`](#neo4j43-enterprise)
-	[`neo4j:4.3.21`](#neo4j4321)
-	[`neo4j:4.3.21-community`](#neo4j4321-community)
-	[`neo4j:4.3.21-enterprise`](#neo4j4321-enterprise)
-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.14`](#neo4j4414)
-	[`neo4j:4.4.14-community`](#neo4j4414-community)
-	[`neo4j:4.4.14-enterprise`](#neo4j4414-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5.1`](#neo4j51)
-	[`neo4j:5.1-enterprise`](#neo4j51-enterprise)
-	[`neo4j:5.1.0`](#neo4j510)
-	[`neo4j:5.1.0-community`](#neo4j510-community)
-	[`neo4j:5.1.0-enterprise`](#neo4j510-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.3`

```console
$ docker pull neo4j@sha256:6396689ea6a263a3cc8af0c031251d88d290491c40e6b86464e2183ee3a3fab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3` - linux; amd64

```console
$ docker pull neo4j@sha256:26c46bd979a2ee8bc0359897a006beffa4b3fc18e47091d1dcbdb44fb52c08e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.3 MB (360298415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc77dcae38c0626b5ddccda11f2c47521c3278c17fbe6b5869240968777b268`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:03:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=39ec4c909fe4c51ae1936922aafe0d649d438faff838f65489e9b25ea76a69de NEO4J_TARBALL=neo4j-community-4.3.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:03:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
# Thu, 10 Nov 2022 21:03:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:03:40 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Thu, 10 Nov 2022 21:03:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:03:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:03:57 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:03:57 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:03:57 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:03:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:03:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf6ddb7032ebd3a6d23712826706b444ca58fe8df7ede3706b24bc8206dcebd`  
		Last Modified: Thu, 10 Nov 2022 21:05:35 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b7afb7db4ee9798d33716e286a579742a90f56cd440e7e6df913e3ae6760a1`  
		Last Modified: Thu, 10 Nov 2022 21:05:35 GMT  
		Size: 7.6 KB (7627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e017a9d6ff9d18764d300d7d547abed58a70ec712d8d1c762787e796d282ed`  
		Last Modified: Thu, 10 Nov 2022 21:05:42 GMT  
		Size: 130.4 MB (130411046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3-community`

```console
$ docker pull neo4j@sha256:6396689ea6a263a3cc8af0c031251d88d290491c40e6b86464e2183ee3a3fab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3-community` - linux; amd64

```console
$ docker pull neo4j@sha256:26c46bd979a2ee8bc0359897a006beffa4b3fc18e47091d1dcbdb44fb52c08e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.3 MB (360298415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc77dcae38c0626b5ddccda11f2c47521c3278c17fbe6b5869240968777b268`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:03:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=39ec4c909fe4c51ae1936922aafe0d649d438faff838f65489e9b25ea76a69de NEO4J_TARBALL=neo4j-community-4.3.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:03:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
# Thu, 10 Nov 2022 21:03:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:03:40 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Thu, 10 Nov 2022 21:03:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:03:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:03:57 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:03:57 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:03:57 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:03:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:03:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf6ddb7032ebd3a6d23712826706b444ca58fe8df7ede3706b24bc8206dcebd`  
		Last Modified: Thu, 10 Nov 2022 21:05:35 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b7afb7db4ee9798d33716e286a579742a90f56cd440e7e6df913e3ae6760a1`  
		Last Modified: Thu, 10 Nov 2022 21:05:35 GMT  
		Size: 7.6 KB (7627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e017a9d6ff9d18764d300d7d547abed58a70ec712d8d1c762787e796d282ed`  
		Last Modified: Thu, 10 Nov 2022 21:05:42 GMT  
		Size: 130.4 MB (130411046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3-enterprise`

```console
$ docker pull neo4j@sha256:076e0a37b6c68caa95716a94fef05b7c39a6a3c5f3f828c4f62109c7275f8928
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:34e9f07e1e8b94e03e1deadc74e4c6a69fd3a822fbe45e3187008ccd41ccaf66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.8 MB (390789276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d1f85abca070b55f2ebb79ae9e4c9689e1c3a614e93689f3388df427005ee8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:04:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=73a8a9357081c0c62859672b21fb61a0352a1444d82b78cf226099c9a57adaa4 NEO4J_TARBALL=neo4j-enterprise-4.3.21-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:04:03 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.21-unix.tar.gz
# Thu, 10 Nov 2022 21:04:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:04:04 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Thu, 10 Nov 2022 21:04:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:04:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:04:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:04:23 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:04:23 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:04:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:04:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51579107ab52d85467ffa277d5324debbf5fa38102285913a8534fde34e6eb23`  
		Last Modified: Thu, 10 Nov 2022 21:05:55 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a66e8b9addedcf86e58eb952be5fce7974dae362ecd1cf36245166ed881921`  
		Last Modified: Thu, 10 Nov 2022 21:05:55 GMT  
		Size: 7.6 KB (7622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c4ffd471cae76c39df727e3c3e5e8c827f4108f5917a51d5f0c63ee00819c`  
		Last Modified: Thu, 10 Nov 2022 21:06:03 GMT  
		Size: 160.9 MB (160901911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.21`

```console
$ docker pull neo4j@sha256:6396689ea6a263a3cc8af0c031251d88d290491c40e6b86464e2183ee3a3fab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.21` - linux; amd64

```console
$ docker pull neo4j@sha256:26c46bd979a2ee8bc0359897a006beffa4b3fc18e47091d1dcbdb44fb52c08e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.3 MB (360298415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc77dcae38c0626b5ddccda11f2c47521c3278c17fbe6b5869240968777b268`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:03:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=39ec4c909fe4c51ae1936922aafe0d649d438faff838f65489e9b25ea76a69de NEO4J_TARBALL=neo4j-community-4.3.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:03:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
# Thu, 10 Nov 2022 21:03:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:03:40 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Thu, 10 Nov 2022 21:03:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:03:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:03:57 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:03:57 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:03:57 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:03:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:03:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf6ddb7032ebd3a6d23712826706b444ca58fe8df7ede3706b24bc8206dcebd`  
		Last Modified: Thu, 10 Nov 2022 21:05:35 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b7afb7db4ee9798d33716e286a579742a90f56cd440e7e6df913e3ae6760a1`  
		Last Modified: Thu, 10 Nov 2022 21:05:35 GMT  
		Size: 7.6 KB (7627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e017a9d6ff9d18764d300d7d547abed58a70ec712d8d1c762787e796d282ed`  
		Last Modified: Thu, 10 Nov 2022 21:05:42 GMT  
		Size: 130.4 MB (130411046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.21-community`

```console
$ docker pull neo4j@sha256:6396689ea6a263a3cc8af0c031251d88d290491c40e6b86464e2183ee3a3fab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.21-community` - linux; amd64

```console
$ docker pull neo4j@sha256:26c46bd979a2ee8bc0359897a006beffa4b3fc18e47091d1dcbdb44fb52c08e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.3 MB (360298415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc77dcae38c0626b5ddccda11f2c47521c3278c17fbe6b5869240968777b268`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:03:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=39ec4c909fe4c51ae1936922aafe0d649d438faff838f65489e9b25ea76a69de NEO4J_TARBALL=neo4j-community-4.3.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:03:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
# Thu, 10 Nov 2022 21:03:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:03:40 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Thu, 10 Nov 2022 21:03:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.3.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:03:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:03:57 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:03:57 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:03:57 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:03:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:03:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf6ddb7032ebd3a6d23712826706b444ca58fe8df7ede3706b24bc8206dcebd`  
		Last Modified: Thu, 10 Nov 2022 21:05:35 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b7afb7db4ee9798d33716e286a579742a90f56cd440e7e6df913e3ae6760a1`  
		Last Modified: Thu, 10 Nov 2022 21:05:35 GMT  
		Size: 7.6 KB (7627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e017a9d6ff9d18764d300d7d547abed58a70ec712d8d1c762787e796d282ed`  
		Last Modified: Thu, 10 Nov 2022 21:05:42 GMT  
		Size: 130.4 MB (130411046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.3.21-enterprise`

```console
$ docker pull neo4j@sha256:076e0a37b6c68caa95716a94fef05b7c39a6a3c5f3f828c4f62109c7275f8928
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.3.21-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:34e9f07e1e8b94e03e1deadc74e4c6a69fd3a822fbe45e3187008ccd41ccaf66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.8 MB (390789276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d1f85abca070b55f2ebb79ae9e4c9689e1c3a614e93689f3388df427005ee8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:04:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=73a8a9357081c0c62859672b21fb61a0352a1444d82b78cf226099c9a57adaa4 NEO4J_TARBALL=neo4j-enterprise-4.3.21-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:04:03 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.21-unix.tar.gz
# Thu, 10 Nov 2022 21:04:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:04:04 GMT
COPY multi:3b4704be041416e3fa83bc67a4b7f99c008afd7bda5553bae3b5e35844061a0a in /startup/ 
# Thu, 10 Nov 2022 21:04:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.3.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:04:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:04:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:04:23 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:04:23 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:04:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:04:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51579107ab52d85467ffa277d5324debbf5fa38102285913a8534fde34e6eb23`  
		Last Modified: Thu, 10 Nov 2022 21:05:55 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a66e8b9addedcf86e58eb952be5fce7974dae362ecd1cf36245166ed881921`  
		Last Modified: Thu, 10 Nov 2022 21:05:55 GMT  
		Size: 7.6 KB (7622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c4ffd471cae76c39df727e3c3e5e8c827f4108f5917a51d5f0c63ee00819c`  
		Last Modified: Thu, 10 Nov 2022 21:06:03 GMT  
		Size: 160.9 MB (160901911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:2e5503f82a3321a8a4bfbb288812723def5bd039dc87018f1fc6f4edbdb8e0b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:fcfcbb026e0e538bf66f5fe5c4b2db3dd4931c3aae07f13a5a8c10e979596256
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.2 MB (365191080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3fb3d78a8ca59e43a4befeb544851be71adab616ce9540853f6b6cf197cff9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:02:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=339cb1c9e885f27efb7d284239cae76423be3389d631420917330da97af79e90 NEO4J_TARBALL=neo4j-community-4.4.14-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:02:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:02:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:02:48 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:03:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:03:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:03:07 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:03:07 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:03:07 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:03:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:03:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc595c5d513cb7bf4ee1d3fd5ca4d27784e05e4c073586c8cb85bf5705e45d`  
		Last Modified: Thu, 10 Nov 2022 21:04:53 GMT  
		Size: 3.9 KB (3871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b82b3fc5465cfd76e8c27259cddffded8a2df10688a9d181516cea3d018ffc7`  
		Last Modified: Thu, 10 Nov 2022 21:04:53 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69899c801f1cfc707562d190478566f46e1cfc4debf9093792edca3af71d4`  
		Last Modified: Thu, 10 Nov 2022 21:05:00 GMT  
		Size: 135.3 MB (135303153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:dac8ab67f63f43a645081495b4b685d32eda3738a727b58d522af076e25b72e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.4 MB (360439130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797ab4079ea3a57e17e92682bab94fc206687d92418268dd8e550af4ce9bf53d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 04 Nov 2022 23:12:49 GMT
COPY dir:5aa0292cc524fb250468b6c5a859d971d75bcb0dd4bed7cfb9f10423858de6d6 in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:04:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=339cb1c9e885f27efb7d284239cae76423be3389d631420917330da97af79e90 NEO4J_TARBALL=neo4j-community-4.4.14-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:04:23 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:04:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:04:24 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:04:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:04:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:04:35 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:04:35 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:04:35 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:04:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:04:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb106e6b88c840d8bc916d39cbd7e76282f34fad97623abb4a385dbc33404ce`  
		Last Modified: Fri, 04 Nov 2022 23:23:35 GMT  
		Size: 195.2 MB (195201089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b4bf102e6f8e35396c8e1b04242522f6d5c4863be2591b44c254675c390ce0`  
		Last Modified: Thu, 10 Nov 2022 21:05:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04e0476a2f72bb9a8d28c34f59317e9d56b73f2badd8f1719e2a513c9c037c6`  
		Last Modified: Thu, 10 Nov 2022 21:05:21 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f779ff185eb3a2356fef0b0afdaa30073e003d54748bbbe3d12d770dcc8f55`  
		Last Modified: Thu, 10 Nov 2022 21:05:27 GMT  
		Size: 135.2 MB (135162074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:2e5503f82a3321a8a4bfbb288812723def5bd039dc87018f1fc6f4edbdb8e0b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:fcfcbb026e0e538bf66f5fe5c4b2db3dd4931c3aae07f13a5a8c10e979596256
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.2 MB (365191080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3fb3d78a8ca59e43a4befeb544851be71adab616ce9540853f6b6cf197cff9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:02:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=339cb1c9e885f27efb7d284239cae76423be3389d631420917330da97af79e90 NEO4J_TARBALL=neo4j-community-4.4.14-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:02:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:02:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:02:48 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:03:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:03:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:03:07 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:03:07 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:03:07 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:03:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:03:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc595c5d513cb7bf4ee1d3fd5ca4d27784e05e4c073586c8cb85bf5705e45d`  
		Last Modified: Thu, 10 Nov 2022 21:04:53 GMT  
		Size: 3.9 KB (3871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b82b3fc5465cfd76e8c27259cddffded8a2df10688a9d181516cea3d018ffc7`  
		Last Modified: Thu, 10 Nov 2022 21:04:53 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69899c801f1cfc707562d190478566f46e1cfc4debf9093792edca3af71d4`  
		Last Modified: Thu, 10 Nov 2022 21:05:00 GMT  
		Size: 135.3 MB (135303153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:dac8ab67f63f43a645081495b4b685d32eda3738a727b58d522af076e25b72e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.4 MB (360439130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797ab4079ea3a57e17e92682bab94fc206687d92418268dd8e550af4ce9bf53d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 04 Nov 2022 23:12:49 GMT
COPY dir:5aa0292cc524fb250468b6c5a859d971d75bcb0dd4bed7cfb9f10423858de6d6 in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:04:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=339cb1c9e885f27efb7d284239cae76423be3389d631420917330da97af79e90 NEO4J_TARBALL=neo4j-community-4.4.14-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:04:23 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:04:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:04:24 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:04:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:04:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:04:35 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:04:35 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:04:35 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:04:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:04:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb106e6b88c840d8bc916d39cbd7e76282f34fad97623abb4a385dbc33404ce`  
		Last Modified: Fri, 04 Nov 2022 23:23:35 GMT  
		Size: 195.2 MB (195201089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b4bf102e6f8e35396c8e1b04242522f6d5c4863be2591b44c254675c390ce0`  
		Last Modified: Thu, 10 Nov 2022 21:05:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04e0476a2f72bb9a8d28c34f59317e9d56b73f2badd8f1719e2a513c9c037c6`  
		Last Modified: Thu, 10 Nov 2022 21:05:21 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f779ff185eb3a2356fef0b0afdaa30073e003d54748bbbe3d12d770dcc8f55`  
		Last Modified: Thu, 10 Nov 2022 21:05:27 GMT  
		Size: 135.2 MB (135162074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:79e5b3a43af1f8f921ba68cd2530b1a410aff1377dbe39ef5b0e1adaae7f6a46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:3bf575b323d20ff90773153c6f66d7962d58e04d434ddbc6d1a8ccac30e26d00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.4 MB (460382376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1c0a2f95649528ca83d1b44e68fa35cf73ade9fd1038310bbbe85822b5b1cf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:03:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa50a54d7d460391051b03f12f49718969ee45912fb7fa3bb9e4bcb49001286e NEO4J_TARBALL=neo4j-enterprise-4.4.14-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:03:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:03:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:03:12 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:03:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:03:34 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:03:34 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:03:34 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:03:35 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:03:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:03:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b0a761311b7b72cb8b5c626f81b3da5a6a0b1c9cfdcf1497b14bb6e4fff2a`  
		Last Modified: Thu, 10 Nov 2022 21:05:14 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d8ad4151283c9d791cf5ae3ffe42910383d66de9ae419655c8f42025138441`  
		Last Modified: Thu, 10 Nov 2022 21:05:15 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafec535186ef01d59fe66a33ccd7f7fc43189571137fbffccb1655306c0d216`  
		Last Modified: Thu, 10 Nov 2022 21:05:26 GMT  
		Size: 230.5 MB (230494461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4cbc20fc10ff0bfac99b7449fcc53f2ba4eb7246eb585faa0cd25d653fa2a8d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.6 MB (455629502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e4926ebb0fd5d3123ccff364e040a6f4787afec512672b8fcb75d7fce429621`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 04 Nov 2022 23:12:49 GMT
COPY dir:5aa0292cc524fb250468b6c5a859d971d75bcb0dd4bed7cfb9f10423858de6d6 in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:04:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa50a54d7d460391051b03f12f49718969ee45912fb7fa3bb9e4bcb49001286e NEO4J_TARBALL=neo4j-enterprise-4.4.14-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:04:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:04:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:04:40 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:04:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:04:53 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:04:53 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:04:53 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:04:54 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:04:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:04:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb106e6b88c840d8bc916d39cbd7e76282f34fad97623abb4a385dbc33404ce`  
		Last Modified: Fri, 04 Nov 2022 23:23:35 GMT  
		Size: 195.2 MB (195201089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a92425963287d349a8c9a853dd5d4fa96b7626668e1b6ca4e2b432d006b0f1`  
		Last Modified: Thu, 10 Nov 2022 21:05:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d471490bcd6873f3259786e8022776d2c26ba561fe407846bfba6b6aee2f2067`  
		Last Modified: Thu, 10 Nov 2022 21:05:41 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e34af0824504f43515080f40887e6a367eac89509e1c2d3acdf3668619025c`  
		Last Modified: Thu, 10 Nov 2022 21:05:50 GMT  
		Size: 230.4 MB (230352442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.14`

```console
$ docker pull neo4j@sha256:2e5503f82a3321a8a4bfbb288812723def5bd039dc87018f1fc6f4edbdb8e0b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.14` - linux; amd64

```console
$ docker pull neo4j@sha256:fcfcbb026e0e538bf66f5fe5c4b2db3dd4931c3aae07f13a5a8c10e979596256
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.2 MB (365191080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3fb3d78a8ca59e43a4befeb544851be71adab616ce9540853f6b6cf197cff9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:02:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=339cb1c9e885f27efb7d284239cae76423be3389d631420917330da97af79e90 NEO4J_TARBALL=neo4j-community-4.4.14-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:02:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:02:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:02:48 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:03:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:03:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:03:07 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:03:07 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:03:07 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:03:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:03:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc595c5d513cb7bf4ee1d3fd5ca4d27784e05e4c073586c8cb85bf5705e45d`  
		Last Modified: Thu, 10 Nov 2022 21:04:53 GMT  
		Size: 3.9 KB (3871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b82b3fc5465cfd76e8c27259cddffded8a2df10688a9d181516cea3d018ffc7`  
		Last Modified: Thu, 10 Nov 2022 21:04:53 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69899c801f1cfc707562d190478566f46e1cfc4debf9093792edca3af71d4`  
		Last Modified: Thu, 10 Nov 2022 21:05:00 GMT  
		Size: 135.3 MB (135303153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.14` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:dac8ab67f63f43a645081495b4b685d32eda3738a727b58d522af076e25b72e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.4 MB (360439130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797ab4079ea3a57e17e92682bab94fc206687d92418268dd8e550af4ce9bf53d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 04 Nov 2022 23:12:49 GMT
COPY dir:5aa0292cc524fb250468b6c5a859d971d75bcb0dd4bed7cfb9f10423858de6d6 in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:04:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=339cb1c9e885f27efb7d284239cae76423be3389d631420917330da97af79e90 NEO4J_TARBALL=neo4j-community-4.4.14-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:04:23 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:04:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:04:24 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:04:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:04:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:04:35 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:04:35 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:04:35 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:04:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:04:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb106e6b88c840d8bc916d39cbd7e76282f34fad97623abb4a385dbc33404ce`  
		Last Modified: Fri, 04 Nov 2022 23:23:35 GMT  
		Size: 195.2 MB (195201089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b4bf102e6f8e35396c8e1b04242522f6d5c4863be2591b44c254675c390ce0`  
		Last Modified: Thu, 10 Nov 2022 21:05:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04e0476a2f72bb9a8d28c34f59317e9d56b73f2badd8f1719e2a513c9c037c6`  
		Last Modified: Thu, 10 Nov 2022 21:05:21 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f779ff185eb3a2356fef0b0afdaa30073e003d54748bbbe3d12d770dcc8f55`  
		Last Modified: Thu, 10 Nov 2022 21:05:27 GMT  
		Size: 135.2 MB (135162074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.14-community`

```console
$ docker pull neo4j@sha256:2e5503f82a3321a8a4bfbb288812723def5bd039dc87018f1fc6f4edbdb8e0b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.14-community` - linux; amd64

```console
$ docker pull neo4j@sha256:fcfcbb026e0e538bf66f5fe5c4b2db3dd4931c3aae07f13a5a8c10e979596256
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.2 MB (365191080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3fb3d78a8ca59e43a4befeb544851be71adab616ce9540853f6b6cf197cff9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:02:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=339cb1c9e885f27efb7d284239cae76423be3389d631420917330da97af79e90 NEO4J_TARBALL=neo4j-community-4.4.14-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:02:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:02:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:02:48 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:03:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:03:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:03:07 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:03:07 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:03:07 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:03:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:03:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc595c5d513cb7bf4ee1d3fd5ca4d27784e05e4c073586c8cb85bf5705e45d`  
		Last Modified: Thu, 10 Nov 2022 21:04:53 GMT  
		Size: 3.9 KB (3871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b82b3fc5465cfd76e8c27259cddffded8a2df10688a9d181516cea3d018ffc7`  
		Last Modified: Thu, 10 Nov 2022 21:04:53 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69899c801f1cfc707562d190478566f46e1cfc4debf9093792edca3af71d4`  
		Last Modified: Thu, 10 Nov 2022 21:05:00 GMT  
		Size: 135.3 MB (135303153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.14-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:dac8ab67f63f43a645081495b4b685d32eda3738a727b58d522af076e25b72e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.4 MB (360439130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797ab4079ea3a57e17e92682bab94fc206687d92418268dd8e550af4ce9bf53d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 04 Nov 2022 23:12:49 GMT
COPY dir:5aa0292cc524fb250468b6c5a859d971d75bcb0dd4bed7cfb9f10423858de6d6 in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:04:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=339cb1c9e885f27efb7d284239cae76423be3389d631420917330da97af79e90 NEO4J_TARBALL=neo4j-community-4.4.14-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:04:23 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:04:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:04:24 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:04:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:04:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:04:35 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:04:35 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:04:35 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:04:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:04:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb106e6b88c840d8bc916d39cbd7e76282f34fad97623abb4a385dbc33404ce`  
		Last Modified: Fri, 04 Nov 2022 23:23:35 GMT  
		Size: 195.2 MB (195201089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b4bf102e6f8e35396c8e1b04242522f6d5c4863be2591b44c254675c390ce0`  
		Last Modified: Thu, 10 Nov 2022 21:05:21 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04e0476a2f72bb9a8d28c34f59317e9d56b73f2badd8f1719e2a513c9c037c6`  
		Last Modified: Thu, 10 Nov 2022 21:05:21 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f779ff185eb3a2356fef0b0afdaa30073e003d54748bbbe3d12d770dcc8f55`  
		Last Modified: Thu, 10 Nov 2022 21:05:27 GMT  
		Size: 135.2 MB (135162074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.14-enterprise`

```console
$ docker pull neo4j@sha256:79e5b3a43af1f8f921ba68cd2530b1a410aff1377dbe39ef5b0e1adaae7f6a46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.14-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:3bf575b323d20ff90773153c6f66d7962d58e04d434ddbc6d1a8ccac30e26d00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.4 MB (460382376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1c0a2f95649528ca83d1b44e68fa35cf73ade9fd1038310bbbe85822b5b1cf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 05 Nov 2022 00:29:05 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:03:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa50a54d7d460391051b03f12f49718969ee45912fb7fa3bb9e4bcb49001286e NEO4J_TARBALL=neo4j-enterprise-4.4.14-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:03:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:03:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:03:12 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:03:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:03:34 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:03:34 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:03:34 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:03:35 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:03:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:03:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eeac167d177f8e3f122f752a133299e5053ba524e678b50f631ee9e5c6e940`  
		Last Modified: Sat, 05 Nov 2022 00:31:16 GMT  
		Size: 198.5 MB (198455845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b0a761311b7b72cb8b5c626f81b3da5a6a0b1c9cfdcf1497b14bb6e4fff2a`  
		Last Modified: Thu, 10 Nov 2022 21:05:14 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d8ad4151283c9d791cf5ae3ffe42910383d66de9ae419655c8f42025138441`  
		Last Modified: Thu, 10 Nov 2022 21:05:15 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafec535186ef01d59fe66a33ccd7f7fc43189571137fbffccb1655306c0d216`  
		Last Modified: Thu, 10 Nov 2022 21:05:26 GMT  
		Size: 230.5 MB (230494461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.14-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4cbc20fc10ff0bfac99b7449fcc53f2ba4eb7246eb585faa0cd25d653fa2a8d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.6 MB (455629502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e4926ebb0fd5d3123ccff364e040a6f4787afec512672b8fcb75d7fce429621`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 04 Nov 2022 23:12:49 GMT
COPY dir:5aa0292cc524fb250468b6c5a859d971d75bcb0dd4bed7cfb9f10423858de6d6 in /opt/java/openjdk 
# Thu, 10 Nov 2022 21:04:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa50a54d7d460391051b03f12f49718969ee45912fb7fa3bb9e4bcb49001286e NEO4J_TARBALL=neo4j-enterprise-4.4.14-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 10 Nov 2022 21:04:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
# Thu, 10 Nov 2022 21:04:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 10 Nov 2022 21:04:40 GMT
COPY multi:d79a5b7ba73da37dcfa9335950c203f23710473d4bdc3c12de4d0b0c62fbd733 in /startup/ 
# Thu, 10 Nov 2022 21:04:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Nov 2022 21:04:53 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 21:04:53 GMT
WORKDIR /var/lib/neo4j
# Thu, 10 Nov 2022 21:04:53 GMT
VOLUME [/data /logs]
# Thu, 10 Nov 2022 21:04:54 GMT
EXPOSE 7473 7474 7687
# Thu, 10 Nov 2022 21:04:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:04:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb106e6b88c840d8bc916d39cbd7e76282f34fad97623abb4a385dbc33404ce`  
		Last Modified: Fri, 04 Nov 2022 23:23:35 GMT  
		Size: 195.2 MB (195201089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a92425963287d349a8c9a853dd5d4fa96b7626668e1b6ca4e2b432d006b0f1`  
		Last Modified: Thu, 10 Nov 2022 21:05:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d471490bcd6873f3259786e8022776d2c26ba561fe407846bfba6b6aee2f2067`  
		Last Modified: Thu, 10 Nov 2022 21:05:41 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e34af0824504f43515080f40887e6a367eac89509e1c2d3acdf3668619025c`  
		Last Modified: Thu, 10 Nov 2022 21:05:50 GMT  
		Size: 230.4 MB (230352442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:589f6b099edcab2848f30899317af61547c2bc36777a66ecf4513ab8a258b4df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:3ad88ceb9cced6dc2bb686e060eb2fc68c580a5c82943f1c361ef6a23c099018
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.6 MB (334571402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e8fabaef285bc934b646db7981529d3257b2dbd071d0efc166a764f0a05e9a7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:03 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:04 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:16 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:16 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:16 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca65b8a2c6678ed5001a523f60b53a78d05bdeafa47afb4159afb57a753d06bc`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79ac708f0d7f66d87f165b4cbab59bf15f1e0a9331b05fa459a174e54deb409`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbba578ea91813db3207c2be4512eb25b066646974c23a7f6ffb52ec6d0f57e`  
		Last Modified: Mon, 07 Nov 2022 21:43:20 GMT  
		Size: 110.7 MB (110708609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:db984633260a4dcebd2a947b897486e106a59219a926e1edef3ca02f39ce459d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331856654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ae93e09f723d1ce12b8b30075ec388bdd475c3cc75a32ceb3100855e3bd8d5`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:21 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:22 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:31 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:31 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:31 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:31 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:31 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:31 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78489ea6d327966723e32b2c92b0a25b093bf7fc19d40d6ed0ccba9df1671e59`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7fa9e5679baf03c909f45e99134562a0043cdac2d992a0f15f75752052263e`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 7.6 KB (7628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624eb837b81cf0ad6c6b061765b8aec39fb37d7492c2f91d999d6d8fa39931f5`  
		Last Modified: Mon, 07 Nov 2022 21:40:27 GMT  
		Size: 110.6 MB (110566002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:589f6b099edcab2848f30899317af61547c2bc36777a66ecf4513ab8a258b4df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:3ad88ceb9cced6dc2bb686e060eb2fc68c580a5c82943f1c361ef6a23c099018
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.6 MB (334571402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e8fabaef285bc934b646db7981529d3257b2dbd071d0efc166a764f0a05e9a7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:03 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:04 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:16 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:16 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:16 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca65b8a2c6678ed5001a523f60b53a78d05bdeafa47afb4159afb57a753d06bc`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79ac708f0d7f66d87f165b4cbab59bf15f1e0a9331b05fa459a174e54deb409`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbba578ea91813db3207c2be4512eb25b066646974c23a7f6ffb52ec6d0f57e`  
		Last Modified: Mon, 07 Nov 2022 21:43:20 GMT  
		Size: 110.7 MB (110708609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:db984633260a4dcebd2a947b897486e106a59219a926e1edef3ca02f39ce459d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331856654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ae93e09f723d1ce12b8b30075ec388bdd475c3cc75a32ceb3100855e3bd8d5`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:21 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:22 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:31 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:31 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:31 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:31 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:31 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:31 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78489ea6d327966723e32b2c92b0a25b093bf7fc19d40d6ed0ccba9df1671e59`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7fa9e5679baf03c909f45e99134562a0043cdac2d992a0f15f75752052263e`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 7.6 KB (7628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624eb837b81cf0ad6c6b061765b8aec39fb37d7492c2f91d999d6d8fa39931f5`  
		Last Modified: Mon, 07 Nov 2022 21:40:27 GMT  
		Size: 110.6 MB (110566002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:9a4bcf00ee9014a9ff0b708a3c1030ecb09bb23d8d7522b5fe6f2b88a05fb7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:20b7411918a707659786a1a770d5c8c275565d85d0cada635fade57cf575ab83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.2 MB (430159743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75672eebe80dbbdaeaff4717d949e0277218793afaf2d8c655fc59634edb3c70`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:21 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:36 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:36 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:36 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e8565cfe49966c982867a5621e5eaf2dacc4051ede76f2d5fa1c05cc4663e8`  
		Last Modified: Mon, 07 Nov 2022 21:43:45 GMT  
		Size: 3.9 KB (3861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a8f35af07dcaed5768cc7f8c4ef833434b4cf18877f9b9b2b829dd76db0a6e`  
		Last Modified: Mon, 07 Nov 2022 21:43:45 GMT  
		Size: 7.6 KB (7631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bef8af0d744b267d17da627ab840c060bc69874505af56002b0e06e1e65abe`  
		Last Modified: Mon, 07 Nov 2022 21:43:55 GMT  
		Size: 206.3 MB (206296947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:63b00a9e963c031cad10716e42ac91ba44aa05241d49480b00ad6a9ee3b9c1c6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.4 MB (427444123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e58c75c545a73f3f586b558acda7045154e84771fd0182d6754c6440d00d025`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:36 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:54 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:54 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:54 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a178c84172e1ce76780f08f6343145c0bcdc38eec775c69b6637fcb0be1d393`  
		Last Modified: Mon, 07 Nov 2022 21:40:49 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61a5e1cbd196598c089048696990a1e5f2c180f24cb8c95a97eecfbfc538831`  
		Last Modified: Mon, 07 Nov 2022 21:40:49 GMT  
		Size: 7.6 KB (7629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084b6431edc5985ae0e1d28b4a14112bd2c2b910312a545f0e41991d94b9ab06`  
		Last Modified: Mon, 07 Nov 2022 21:40:57 GMT  
		Size: 206.2 MB (206153470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.1`

```console
$ docker pull neo4j@sha256:589f6b099edcab2848f30899317af61547c2bc36777a66ecf4513ab8a258b4df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.1` - linux; amd64

```console
$ docker pull neo4j@sha256:3ad88ceb9cced6dc2bb686e060eb2fc68c580a5c82943f1c361ef6a23c099018
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.6 MB (334571402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e8fabaef285bc934b646db7981529d3257b2dbd071d0efc166a764f0a05e9a7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:03 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:04 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:16 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:16 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:16 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca65b8a2c6678ed5001a523f60b53a78d05bdeafa47afb4159afb57a753d06bc`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79ac708f0d7f66d87f165b4cbab59bf15f1e0a9331b05fa459a174e54deb409`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbba578ea91813db3207c2be4512eb25b066646974c23a7f6ffb52ec6d0f57e`  
		Last Modified: Mon, 07 Nov 2022 21:43:20 GMT  
		Size: 110.7 MB (110708609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.1` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:db984633260a4dcebd2a947b897486e106a59219a926e1edef3ca02f39ce459d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331856654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ae93e09f723d1ce12b8b30075ec388bdd475c3cc75a32ceb3100855e3bd8d5`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:21 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:22 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:31 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:31 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:31 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:31 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:31 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:31 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78489ea6d327966723e32b2c92b0a25b093bf7fc19d40d6ed0ccba9df1671e59`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7fa9e5679baf03c909f45e99134562a0043cdac2d992a0f15f75752052263e`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 7.6 KB (7628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624eb837b81cf0ad6c6b061765b8aec39fb37d7492c2f91d999d6d8fa39931f5`  
		Last Modified: Mon, 07 Nov 2022 21:40:27 GMT  
		Size: 110.6 MB (110566002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.1-enterprise`

```console
$ docker pull neo4j@sha256:9a4bcf00ee9014a9ff0b708a3c1030ecb09bb23d8d7522b5fe6f2b88a05fb7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.1-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:20b7411918a707659786a1a770d5c8c275565d85d0cada635fade57cf575ab83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.2 MB (430159743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75672eebe80dbbdaeaff4717d949e0277218793afaf2d8c655fc59634edb3c70`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:21 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:36 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:36 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:36 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e8565cfe49966c982867a5621e5eaf2dacc4051ede76f2d5fa1c05cc4663e8`  
		Last Modified: Mon, 07 Nov 2022 21:43:45 GMT  
		Size: 3.9 KB (3861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a8f35af07dcaed5768cc7f8c4ef833434b4cf18877f9b9b2b829dd76db0a6e`  
		Last Modified: Mon, 07 Nov 2022 21:43:45 GMT  
		Size: 7.6 KB (7631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bef8af0d744b267d17da627ab840c060bc69874505af56002b0e06e1e65abe`  
		Last Modified: Mon, 07 Nov 2022 21:43:55 GMT  
		Size: 206.3 MB (206296947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.1-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:63b00a9e963c031cad10716e42ac91ba44aa05241d49480b00ad6a9ee3b9c1c6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.4 MB (427444123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e58c75c545a73f3f586b558acda7045154e84771fd0182d6754c6440d00d025`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:36 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:54 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:54 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:54 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a178c84172e1ce76780f08f6343145c0bcdc38eec775c69b6637fcb0be1d393`  
		Last Modified: Mon, 07 Nov 2022 21:40:49 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61a5e1cbd196598c089048696990a1e5f2c180f24cb8c95a97eecfbfc538831`  
		Last Modified: Mon, 07 Nov 2022 21:40:49 GMT  
		Size: 7.6 KB (7629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084b6431edc5985ae0e1d28b4a14112bd2c2b910312a545f0e41991d94b9ab06`  
		Last Modified: Mon, 07 Nov 2022 21:40:57 GMT  
		Size: 206.2 MB (206153470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.1.0`

```console
$ docker pull neo4j@sha256:589f6b099edcab2848f30899317af61547c2bc36777a66ecf4513ab8a258b4df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.1.0` - linux; amd64

```console
$ docker pull neo4j@sha256:3ad88ceb9cced6dc2bb686e060eb2fc68c580a5c82943f1c361ef6a23c099018
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.6 MB (334571402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e8fabaef285bc934b646db7981529d3257b2dbd071d0efc166a764f0a05e9a7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:03 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:04 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:16 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:16 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:16 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca65b8a2c6678ed5001a523f60b53a78d05bdeafa47afb4159afb57a753d06bc`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79ac708f0d7f66d87f165b4cbab59bf15f1e0a9331b05fa459a174e54deb409`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbba578ea91813db3207c2be4512eb25b066646974c23a7f6ffb52ec6d0f57e`  
		Last Modified: Mon, 07 Nov 2022 21:43:20 GMT  
		Size: 110.7 MB (110708609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.1.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:db984633260a4dcebd2a947b897486e106a59219a926e1edef3ca02f39ce459d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331856654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ae93e09f723d1ce12b8b30075ec388bdd475c3cc75a32ceb3100855e3bd8d5`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:21 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:22 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:31 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:31 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:31 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:31 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:31 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:31 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78489ea6d327966723e32b2c92b0a25b093bf7fc19d40d6ed0ccba9df1671e59`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7fa9e5679baf03c909f45e99134562a0043cdac2d992a0f15f75752052263e`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 7.6 KB (7628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624eb837b81cf0ad6c6b061765b8aec39fb37d7492c2f91d999d6d8fa39931f5`  
		Last Modified: Mon, 07 Nov 2022 21:40:27 GMT  
		Size: 110.6 MB (110566002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.1.0-community`

```console
$ docker pull neo4j@sha256:589f6b099edcab2848f30899317af61547c2bc36777a66ecf4513ab8a258b4df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.1.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:3ad88ceb9cced6dc2bb686e060eb2fc68c580a5c82943f1c361ef6a23c099018
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.6 MB (334571402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e8fabaef285bc934b646db7981529d3257b2dbd071d0efc166a764f0a05e9a7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:03 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:04 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:16 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:16 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:16 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca65b8a2c6678ed5001a523f60b53a78d05bdeafa47afb4159afb57a753d06bc`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79ac708f0d7f66d87f165b4cbab59bf15f1e0a9331b05fa459a174e54deb409`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbba578ea91813db3207c2be4512eb25b066646974c23a7f6ffb52ec6d0f57e`  
		Last Modified: Mon, 07 Nov 2022 21:43:20 GMT  
		Size: 110.7 MB (110708609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.1.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:db984633260a4dcebd2a947b897486e106a59219a926e1edef3ca02f39ce459d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331856654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ae93e09f723d1ce12b8b30075ec388bdd475c3cc75a32ceb3100855e3bd8d5`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:21 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:22 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:31 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:31 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:31 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:31 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:31 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:31 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78489ea6d327966723e32b2c92b0a25b093bf7fc19d40d6ed0ccba9df1671e59`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7fa9e5679baf03c909f45e99134562a0043cdac2d992a0f15f75752052263e`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 7.6 KB (7628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624eb837b81cf0ad6c6b061765b8aec39fb37d7492c2f91d999d6d8fa39931f5`  
		Last Modified: Mon, 07 Nov 2022 21:40:27 GMT  
		Size: 110.6 MB (110566002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.1.0-enterprise`

```console
$ docker pull neo4j@sha256:9a4bcf00ee9014a9ff0b708a3c1030ecb09bb23d8d7522b5fe6f2b88a05fb7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.1.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:20b7411918a707659786a1a770d5c8c275565d85d0cada635fade57cf575ab83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.2 MB (430159743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75672eebe80dbbdaeaff4717d949e0277218793afaf2d8c655fc59634edb3c70`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:21 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:36 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:36 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:36 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e8565cfe49966c982867a5621e5eaf2dacc4051ede76f2d5fa1c05cc4663e8`  
		Last Modified: Mon, 07 Nov 2022 21:43:45 GMT  
		Size: 3.9 KB (3861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a8f35af07dcaed5768cc7f8c4ef833434b4cf18877f9b9b2b829dd76db0a6e`  
		Last Modified: Mon, 07 Nov 2022 21:43:45 GMT  
		Size: 7.6 KB (7631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bef8af0d744b267d17da627ab840c060bc69874505af56002b0e06e1e65abe`  
		Last Modified: Mon, 07 Nov 2022 21:43:55 GMT  
		Size: 206.3 MB (206296947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.1.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:63b00a9e963c031cad10716e42ac91ba44aa05241d49480b00ad6a9ee3b9c1c6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.4 MB (427444123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e58c75c545a73f3f586b558acda7045154e84771fd0182d6754c6440d00d025`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:36 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:54 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:54 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:54 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a178c84172e1ce76780f08f6343145c0bcdc38eec775c69b6637fcb0be1d393`  
		Last Modified: Mon, 07 Nov 2022 21:40:49 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61a5e1cbd196598c089048696990a1e5f2c180f24cb8c95a97eecfbfc538831`  
		Last Modified: Mon, 07 Nov 2022 21:40:49 GMT  
		Size: 7.6 KB (7629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084b6431edc5985ae0e1d28b4a14112bd2c2b910312a545f0e41991d94b9ab06`  
		Last Modified: Mon, 07 Nov 2022 21:40:57 GMT  
		Size: 206.2 MB (206153470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:589f6b099edcab2848f30899317af61547c2bc36777a66ecf4513ab8a258b4df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:3ad88ceb9cced6dc2bb686e060eb2fc68c580a5c82943f1c361ef6a23c099018
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.6 MB (334571402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e8fabaef285bc934b646db7981529d3257b2dbd071d0efc166a764f0a05e9a7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:03 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:04 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:16 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:16 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:16 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca65b8a2c6678ed5001a523f60b53a78d05bdeafa47afb4159afb57a753d06bc`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79ac708f0d7f66d87f165b4cbab59bf15f1e0a9331b05fa459a174e54deb409`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbba578ea91813db3207c2be4512eb25b066646974c23a7f6ffb52ec6d0f57e`  
		Last Modified: Mon, 07 Nov 2022 21:43:20 GMT  
		Size: 110.7 MB (110708609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:db984633260a4dcebd2a947b897486e106a59219a926e1edef3ca02f39ce459d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331856654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ae93e09f723d1ce12b8b30075ec388bdd475c3cc75a32ceb3100855e3bd8d5`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:21 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:22 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:31 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:31 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:31 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:31 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:31 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:31 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78489ea6d327966723e32b2c92b0a25b093bf7fc19d40d6ed0ccba9df1671e59`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7fa9e5679baf03c909f45e99134562a0043cdac2d992a0f15f75752052263e`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 7.6 KB (7628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624eb837b81cf0ad6c6b061765b8aec39fb37d7492c2f91d999d6d8fa39931f5`  
		Last Modified: Mon, 07 Nov 2022 21:40:27 GMT  
		Size: 110.6 MB (110566002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:9a4bcf00ee9014a9ff0b708a3c1030ecb09bb23d8d7522b5fe6f2b88a05fb7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:20b7411918a707659786a1a770d5c8c275565d85d0cada635fade57cf575ab83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.2 MB (430159743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75672eebe80dbbdaeaff4717d949e0277218793afaf2d8c655fc59634edb3c70`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:21 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:36 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:36 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:36 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e8565cfe49966c982867a5621e5eaf2dacc4051ede76f2d5fa1c05cc4663e8`  
		Last Modified: Mon, 07 Nov 2022 21:43:45 GMT  
		Size: 3.9 KB (3861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a8f35af07dcaed5768cc7f8c4ef833434b4cf18877f9b9b2b829dd76db0a6e`  
		Last Modified: Mon, 07 Nov 2022 21:43:45 GMT  
		Size: 7.6 KB (7631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bef8af0d744b267d17da627ab840c060bc69874505af56002b0e06e1e65abe`  
		Last Modified: Mon, 07 Nov 2022 21:43:55 GMT  
		Size: 206.3 MB (206296947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:63b00a9e963c031cad10716e42ac91ba44aa05241d49480b00ad6a9ee3b9c1c6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.4 MB (427444123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e58c75c545a73f3f586b558acda7045154e84771fd0182d6754c6440d00d025`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f9b6b6ec624932ed4611e8fadac3f8198853e53b3318cc9a588f1f9ff9a1fb1 NEO4J_TARBALL=neo4j-enterprise-5.1.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:35 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:36 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:36 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:54 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:54 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:54 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a178c84172e1ce76780f08f6343145c0bcdc38eec775c69b6637fcb0be1d393`  
		Last Modified: Mon, 07 Nov 2022 21:40:49 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61a5e1cbd196598c089048696990a1e5f2c180f24cb8c95a97eecfbfc538831`  
		Last Modified: Mon, 07 Nov 2022 21:40:49 GMT  
		Size: 7.6 KB (7629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084b6431edc5985ae0e1d28b4a14112bd2c2b910312a545f0e41991d94b9ab06`  
		Last Modified: Mon, 07 Nov 2022 21:40:57 GMT  
		Size: 206.2 MB (206153470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:589f6b099edcab2848f30899317af61547c2bc36777a66ecf4513ab8a258b4df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:3ad88ceb9cced6dc2bb686e060eb2fc68c580a5c82943f1c361ef6a23c099018
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.6 MB (334571402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e8fabaef285bc934b646db7981529d3257b2dbd071d0efc166a764f0a05e9a7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 20:48:08 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:42:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:42:03 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:42:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:42:04 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:42:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:42:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:42:16 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:42:16 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:42:16 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:42:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:42:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d9967bfe9b338d34c1d6b115d688a7c4c9b111a5ea71ceb27421142a7f12b`  
		Last Modified: Mon, 07 Nov 2022 20:57:59 GMT  
		Size: 192.4 MB (192431266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca65b8a2c6678ed5001a523f60b53a78d05bdeafa47afb4159afb57a753d06bc`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79ac708f0d7f66d87f165b4cbab59bf15f1e0a9331b05fa459a174e54deb409`  
		Last Modified: Mon, 07 Nov 2022 21:43:14 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbba578ea91813db3207c2be4512eb25b066646974c23a7f6ffb52ec6d0f57e`  
		Last Modified: Mon, 07 Nov 2022 21:43:20 GMT  
		Size: 110.7 MB (110708609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:db984633260a4dcebd2a947b897486e106a59219a926e1edef3ca02f39ce459d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331856654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ae93e09f723d1ce12b8b30075ec388bdd475c3cc75a32ceb3100855e3bd8d5`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 07 Nov 2022 21:03:54 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Mon, 07 Nov 2022 21:39:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 07 Nov 2022 21:39:21 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Mon, 07 Nov 2022 21:39:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 07 Nov 2022 21:39:22 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Mon, 07 Nov 2022 21:39:31 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:31 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:39:31 GMT
WORKDIR /var/lib/neo4j
# Mon, 07 Nov 2022 21:39:31 GMT
VOLUME [/data /logs]
# Mon, 07 Nov 2022 21:39:31 GMT
EXPOSE 7473 7474 7687
# Mon, 07 Nov 2022 21:39:31 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 07 Nov 2022 21:39:31 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da08ea5cf75b951398d57ee8bc9c95f4a6a9ffdd4548e791b7ac3a9ea4c9900a`  
		Last Modified: Mon, 07 Nov 2022 21:12:03 GMT  
		Size: 191.2 MB (191215226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78489ea6d327966723e32b2c92b0a25b093bf7fc19d40d6ed0ccba9df1671e59`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7fa9e5679baf03c909f45e99134562a0043cdac2d992a0f15f75752052263e`  
		Last Modified: Mon, 07 Nov 2022 21:40:22 GMT  
		Size: 7.6 KB (7628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624eb837b81cf0ad6c6b061765b8aec39fb37d7492c2f91d999d6d8fa39931f5`  
		Last Modified: Mon, 07 Nov 2022 21:40:27 GMT  
		Size: 110.6 MB (110566002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
