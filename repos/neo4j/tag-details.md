<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.20`](#neo4j4420)
-	[`neo4j:4.4.20-community`](#neo4j4420-community)
-	[`neo4j:4.4.20-enterprise`](#neo4j4420-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5.8`](#neo4j58)
-	[`neo4j:5.8-community`](#neo4j58-community)
-	[`neo4j:5.8-enterprise`](#neo4j58-enterprise)
-	[`neo4j:5.8.0`](#neo4j580)
-	[`neo4j:5.8.0-community`](#neo4j580-community)
-	[`neo4j:5.8.0-enterprise`](#neo4j580-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:d61f1b55569938e3809448ba916204d4a0c5eaf25d1a8809192b152dd133a2b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:6a6b044a9bcfcf5471d2e6de18fd12f30c4a7d9524cba11d67a472b7f61cd236
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.4 MB (349352799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9e0cc69fa89529b81f9cf8a5018c4cdc0c4d1b159522416b281dc2649366a4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:19:27 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Tue, 23 May 2023 04:19:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9d0a96d724615f08934474687707a01afc454dfc09afc3e0ce99d741296d8cbf NEO4J_TARBALL=neo4j-community-4.4.20-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:19:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
# Tue, 23 May 2023 04:19:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:19:29 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 23 May 2023 04:19:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:19:40 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:19:40 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:19:40 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:19:40 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:19:40 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:19:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e80ece7b5d59b8f713850fc7b510f037c2d5884cbead449774454a259f42de`  
		Last Modified: Tue, 23 May 2023 04:21:29 GMT  
		Size: 198.5 MB (198549524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267d55670465870b4ed7e55422bc8d1f860406f6c721565762235803c9213fbf`  
		Last Modified: Tue, 23 May 2023 04:21:15 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c944f9e30d8972620dc456eefd69097d7d849c96b9be7ff0162a8287915f4205`  
		Last Modified: Tue, 23 May 2023 04:21:16 GMT  
		Size: 8.7 KB (8707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ea06cd4d09fe43e59d5aa732cdd882be111e1abba2590e660dbbf546cf06c9`  
		Last Modified: Tue, 23 May 2023 04:21:21 GMT  
		Size: 119.4 MB (119387122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:2d40881fe3ef39538595f3f453d57d7ebea09a143e5d3df1907bf4b684921e1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.6 MB (344633450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe233903eaead3cbcb38fe3cac6c52ea831042611b133da2323a8add4015b81c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Fri, 05 May 2023 18:54:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9d0a96d724615f08934474687707a01afc454dfc09afc3e0ce99d741296d8cbf NEO4J_TARBALL=neo4j-community-4.4.20-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 05 May 2023 18:54:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
# Fri, 05 May 2023 18:54:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 05 May 2023 18:54:54 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Fri, 05 May 2023 18:55:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 05 May 2023 18:55:04 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 May 2023 18:55:04 GMT
WORKDIR /var/lib/neo4j
# Fri, 05 May 2023 18:55:05 GMT
VOLUME [/data /logs]
# Fri, 05 May 2023 18:55:05 GMT
EXPOSE 7473 7474 7687
# Fri, 05 May 2023 18:55:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 05 May 2023 18:55:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0aa3476c1a9b5d9dca9b0f0758094b3ac19d32c73b84d54aff3fac3c7bec504`  
		Last Modified: Fri, 05 May 2023 18:55:37 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5cfa49c626a3633555164de938e107b78241081aac16df792096779feb2efb`  
		Last Modified: Fri, 05 May 2023 18:55:37 GMT  
		Size: 8.7 KB (8704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f9cbbfae074869c2dee87914fd1be657a8e842fd8bc1823fe4e87ea5bb195`  
		Last Modified: Fri, 05 May 2023 18:55:42 GMT  
		Size: 119.2 MB (119243920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:d61f1b55569938e3809448ba916204d4a0c5eaf25d1a8809192b152dd133a2b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:6a6b044a9bcfcf5471d2e6de18fd12f30c4a7d9524cba11d67a472b7f61cd236
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.4 MB (349352799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9e0cc69fa89529b81f9cf8a5018c4cdc0c4d1b159522416b281dc2649366a4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:19:27 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Tue, 23 May 2023 04:19:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9d0a96d724615f08934474687707a01afc454dfc09afc3e0ce99d741296d8cbf NEO4J_TARBALL=neo4j-community-4.4.20-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:19:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
# Tue, 23 May 2023 04:19:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:19:29 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 23 May 2023 04:19:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:19:40 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:19:40 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:19:40 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:19:40 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:19:40 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:19:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e80ece7b5d59b8f713850fc7b510f037c2d5884cbead449774454a259f42de`  
		Last Modified: Tue, 23 May 2023 04:21:29 GMT  
		Size: 198.5 MB (198549524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267d55670465870b4ed7e55422bc8d1f860406f6c721565762235803c9213fbf`  
		Last Modified: Tue, 23 May 2023 04:21:15 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c944f9e30d8972620dc456eefd69097d7d849c96b9be7ff0162a8287915f4205`  
		Last Modified: Tue, 23 May 2023 04:21:16 GMT  
		Size: 8.7 KB (8707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ea06cd4d09fe43e59d5aa732cdd882be111e1abba2590e660dbbf546cf06c9`  
		Last Modified: Tue, 23 May 2023 04:21:21 GMT  
		Size: 119.4 MB (119387122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:2d40881fe3ef39538595f3f453d57d7ebea09a143e5d3df1907bf4b684921e1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.6 MB (344633450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe233903eaead3cbcb38fe3cac6c52ea831042611b133da2323a8add4015b81c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Fri, 05 May 2023 18:54:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9d0a96d724615f08934474687707a01afc454dfc09afc3e0ce99d741296d8cbf NEO4J_TARBALL=neo4j-community-4.4.20-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 05 May 2023 18:54:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
# Fri, 05 May 2023 18:54:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 05 May 2023 18:54:54 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Fri, 05 May 2023 18:55:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 05 May 2023 18:55:04 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 May 2023 18:55:04 GMT
WORKDIR /var/lib/neo4j
# Fri, 05 May 2023 18:55:05 GMT
VOLUME [/data /logs]
# Fri, 05 May 2023 18:55:05 GMT
EXPOSE 7473 7474 7687
# Fri, 05 May 2023 18:55:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 05 May 2023 18:55:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0aa3476c1a9b5d9dca9b0f0758094b3ac19d32c73b84d54aff3fac3c7bec504`  
		Last Modified: Fri, 05 May 2023 18:55:37 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5cfa49c626a3633555164de938e107b78241081aac16df792096779feb2efb`  
		Last Modified: Fri, 05 May 2023 18:55:37 GMT  
		Size: 8.7 KB (8704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f9cbbfae074869c2dee87914fd1be657a8e842fd8bc1823fe4e87ea5bb195`  
		Last Modified: Fri, 05 May 2023 18:55:42 GMT  
		Size: 119.2 MB (119243920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:0b929c714cbe5c496cc6ea0c37a38102ad9616077099eeb7e8984ee5110fe121
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:1f923d5a2065ef0724f7d8879f7f8a859d1c1f356a62476b0124079706d8e51c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.7 MB (446655244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c4b1434625e0c234388b31b8a5415a44db07801663a571fea64e543f432c95`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:19:27 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Tue, 23 May 2023 04:19:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d25329edbbf8a75e9e32d4d0c38fb817f155e171d4cf8b7509a7b50d35bb2549 NEO4J_TARBALL=neo4j-enterprise-4.4.20-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:19:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
# Tue, 23 May 2023 04:19:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:19:44 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 23 May 2023 04:20:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:20:04 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:20:04 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:20:04 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:20:05 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:20:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:20:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e80ece7b5d59b8f713850fc7b510f037c2d5884cbead449774454a259f42de`  
		Last Modified: Tue, 23 May 2023 04:21:29 GMT  
		Size: 198.5 MB (198549524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91edb1f24e0fa5c54f5300b585704a4d401da13dadc7447121997849fd67342f`  
		Last Modified: Tue, 23 May 2023 04:21:40 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e0188044204c2900cc08bfb19fadd149e0066eb88101a348a62949de27a7f6`  
		Last Modified: Tue, 23 May 2023 04:21:40 GMT  
		Size: 8.7 KB (8707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeed45053abf132b8a87e6a48b3b3ae1e7407e8a5412fe47eb18529ca784cb7`  
		Last Modified: Tue, 23 May 2023 04:21:49 GMT  
		Size: 216.7 MB (216689569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fe5bd2b339c8b81777657fa0753db09fe45d1652269092523235ce338ebaa765
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.9 MB (441933203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d9e131e06753b9de820ed28ea2b8bca82a461bad0be453df7aa347da7500b5`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Fri, 05 May 2023 18:55:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d25329edbbf8a75e9e32d4d0c38fb817f155e171d4cf8b7509a7b50d35bb2549 NEO4J_TARBALL=neo4j-enterprise-4.4.20-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 05 May 2023 18:55:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
# Fri, 05 May 2023 18:55:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 05 May 2023 18:55:08 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Fri, 05 May 2023 18:55:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 05 May 2023 18:55:20 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 May 2023 18:55:20 GMT
WORKDIR /var/lib/neo4j
# Fri, 05 May 2023 18:55:20 GMT
VOLUME [/data /logs]
# Fri, 05 May 2023 18:55:20 GMT
EXPOSE 7473 7474 7687
# Fri, 05 May 2023 18:55:20 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 05 May 2023 18:55:20 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be1c502952730214e6c290ee9b13f0018911d40e0a72c05535507b79a9ca642`  
		Last Modified: Fri, 05 May 2023 18:55:54 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfd4d5af0b7ce2cbabacd65efb6a6edc53adf348b69e3bd5cd2172e313f519f`  
		Last Modified: Fri, 05 May 2023 18:55:54 GMT  
		Size: 8.7 KB (8706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f690115508090a789a2e096bfd38c34bc6c7bcb78c033ca20a4d4dc9f2425213`  
		Last Modified: Fri, 05 May 2023 18:56:03 GMT  
		Size: 216.5 MB (216543668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.20`

```console
$ docker pull neo4j@sha256:d61f1b55569938e3809448ba916204d4a0c5eaf25d1a8809192b152dd133a2b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.20` - linux; amd64

```console
$ docker pull neo4j@sha256:6a6b044a9bcfcf5471d2e6de18fd12f30c4a7d9524cba11d67a472b7f61cd236
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.4 MB (349352799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9e0cc69fa89529b81f9cf8a5018c4cdc0c4d1b159522416b281dc2649366a4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:19:27 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Tue, 23 May 2023 04:19:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9d0a96d724615f08934474687707a01afc454dfc09afc3e0ce99d741296d8cbf NEO4J_TARBALL=neo4j-community-4.4.20-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:19:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
# Tue, 23 May 2023 04:19:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:19:29 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 23 May 2023 04:19:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:19:40 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:19:40 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:19:40 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:19:40 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:19:40 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:19:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e80ece7b5d59b8f713850fc7b510f037c2d5884cbead449774454a259f42de`  
		Last Modified: Tue, 23 May 2023 04:21:29 GMT  
		Size: 198.5 MB (198549524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267d55670465870b4ed7e55422bc8d1f860406f6c721565762235803c9213fbf`  
		Last Modified: Tue, 23 May 2023 04:21:15 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c944f9e30d8972620dc456eefd69097d7d849c96b9be7ff0162a8287915f4205`  
		Last Modified: Tue, 23 May 2023 04:21:16 GMT  
		Size: 8.7 KB (8707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ea06cd4d09fe43e59d5aa732cdd882be111e1abba2590e660dbbf546cf06c9`  
		Last Modified: Tue, 23 May 2023 04:21:21 GMT  
		Size: 119.4 MB (119387122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.20` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:2d40881fe3ef39538595f3f453d57d7ebea09a143e5d3df1907bf4b684921e1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.6 MB (344633450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe233903eaead3cbcb38fe3cac6c52ea831042611b133da2323a8add4015b81c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Fri, 05 May 2023 18:54:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9d0a96d724615f08934474687707a01afc454dfc09afc3e0ce99d741296d8cbf NEO4J_TARBALL=neo4j-community-4.4.20-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 05 May 2023 18:54:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
# Fri, 05 May 2023 18:54:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 05 May 2023 18:54:54 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Fri, 05 May 2023 18:55:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 05 May 2023 18:55:04 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 May 2023 18:55:04 GMT
WORKDIR /var/lib/neo4j
# Fri, 05 May 2023 18:55:05 GMT
VOLUME [/data /logs]
# Fri, 05 May 2023 18:55:05 GMT
EXPOSE 7473 7474 7687
# Fri, 05 May 2023 18:55:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 05 May 2023 18:55:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0aa3476c1a9b5d9dca9b0f0758094b3ac19d32c73b84d54aff3fac3c7bec504`  
		Last Modified: Fri, 05 May 2023 18:55:37 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5cfa49c626a3633555164de938e107b78241081aac16df792096779feb2efb`  
		Last Modified: Fri, 05 May 2023 18:55:37 GMT  
		Size: 8.7 KB (8704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f9cbbfae074869c2dee87914fd1be657a8e842fd8bc1823fe4e87ea5bb195`  
		Last Modified: Fri, 05 May 2023 18:55:42 GMT  
		Size: 119.2 MB (119243920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.20-community`

```console
$ docker pull neo4j@sha256:d61f1b55569938e3809448ba916204d4a0c5eaf25d1a8809192b152dd133a2b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.20-community` - linux; amd64

```console
$ docker pull neo4j@sha256:6a6b044a9bcfcf5471d2e6de18fd12f30c4a7d9524cba11d67a472b7f61cd236
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.4 MB (349352799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9e0cc69fa89529b81f9cf8a5018c4cdc0c4d1b159522416b281dc2649366a4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:19:27 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Tue, 23 May 2023 04:19:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9d0a96d724615f08934474687707a01afc454dfc09afc3e0ce99d741296d8cbf NEO4J_TARBALL=neo4j-community-4.4.20-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:19:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
# Tue, 23 May 2023 04:19:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:19:29 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 23 May 2023 04:19:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:19:40 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:19:40 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:19:40 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:19:40 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:19:40 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:19:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e80ece7b5d59b8f713850fc7b510f037c2d5884cbead449774454a259f42de`  
		Last Modified: Tue, 23 May 2023 04:21:29 GMT  
		Size: 198.5 MB (198549524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267d55670465870b4ed7e55422bc8d1f860406f6c721565762235803c9213fbf`  
		Last Modified: Tue, 23 May 2023 04:21:15 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c944f9e30d8972620dc456eefd69097d7d849c96b9be7ff0162a8287915f4205`  
		Last Modified: Tue, 23 May 2023 04:21:16 GMT  
		Size: 8.7 KB (8707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ea06cd4d09fe43e59d5aa732cdd882be111e1abba2590e660dbbf546cf06c9`  
		Last Modified: Tue, 23 May 2023 04:21:21 GMT  
		Size: 119.4 MB (119387122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.20-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:2d40881fe3ef39538595f3f453d57d7ebea09a143e5d3df1907bf4b684921e1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.6 MB (344633450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe233903eaead3cbcb38fe3cac6c52ea831042611b133da2323a8add4015b81c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Fri, 05 May 2023 18:54:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=9d0a96d724615f08934474687707a01afc454dfc09afc3e0ce99d741296d8cbf NEO4J_TARBALL=neo4j-community-4.4.20-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 05 May 2023 18:54:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
# Fri, 05 May 2023 18:54:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 05 May 2023 18:54:54 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Fri, 05 May 2023 18:55:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 05 May 2023 18:55:04 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 May 2023 18:55:04 GMT
WORKDIR /var/lib/neo4j
# Fri, 05 May 2023 18:55:05 GMT
VOLUME [/data /logs]
# Fri, 05 May 2023 18:55:05 GMT
EXPOSE 7473 7474 7687
# Fri, 05 May 2023 18:55:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 05 May 2023 18:55:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0aa3476c1a9b5d9dca9b0f0758094b3ac19d32c73b84d54aff3fac3c7bec504`  
		Last Modified: Fri, 05 May 2023 18:55:37 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5cfa49c626a3633555164de938e107b78241081aac16df792096779feb2efb`  
		Last Modified: Fri, 05 May 2023 18:55:37 GMT  
		Size: 8.7 KB (8704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f9cbbfae074869c2dee87914fd1be657a8e842fd8bc1823fe4e87ea5bb195`  
		Last Modified: Fri, 05 May 2023 18:55:42 GMT  
		Size: 119.2 MB (119243920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.20-enterprise`

```console
$ docker pull neo4j@sha256:0b929c714cbe5c496cc6ea0c37a38102ad9616077099eeb7e8984ee5110fe121
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.20-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:1f923d5a2065ef0724f7d8879f7f8a859d1c1f356a62476b0124079706d8e51c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.7 MB (446655244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c4b1434625e0c234388b31b8a5415a44db07801663a571fea64e543f432c95`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:19:27 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Tue, 23 May 2023 04:19:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d25329edbbf8a75e9e32d4d0c38fb817f155e171d4cf8b7509a7b50d35bb2549 NEO4J_TARBALL=neo4j-enterprise-4.4.20-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:19:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
# Tue, 23 May 2023 04:19:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:19:44 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 23 May 2023 04:20:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:20:04 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:20:04 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:20:04 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:20:05 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:20:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:20:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e80ece7b5d59b8f713850fc7b510f037c2d5884cbead449774454a259f42de`  
		Last Modified: Tue, 23 May 2023 04:21:29 GMT  
		Size: 198.5 MB (198549524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91edb1f24e0fa5c54f5300b585704a4d401da13dadc7447121997849fd67342f`  
		Last Modified: Tue, 23 May 2023 04:21:40 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e0188044204c2900cc08bfb19fadd149e0066eb88101a348a62949de27a7f6`  
		Last Modified: Tue, 23 May 2023 04:21:40 GMT  
		Size: 8.7 KB (8707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeed45053abf132b8a87e6a48b3b3ae1e7407e8a5412fe47eb18529ca784cb7`  
		Last Modified: Tue, 23 May 2023 04:21:49 GMT  
		Size: 216.7 MB (216689569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.20-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fe5bd2b339c8b81777657fa0753db09fe45d1652269092523235ce338ebaa765
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.9 MB (441933203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d9e131e06753b9de820ed28ea2b8bca82a461bad0be453df7aa347da7500b5`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:10:37 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Fri, 05 May 2023 18:55:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d25329edbbf8a75e9e32d4d0c38fb817f155e171d4cf8b7509a7b50d35bb2549 NEO4J_TARBALL=neo4j-enterprise-4.4.20-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 05 May 2023 18:55:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
# Fri, 05 May 2023 18:55:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 05 May 2023 18:55:08 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Fri, 05 May 2023 18:55:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.20-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 05 May 2023 18:55:20 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 May 2023 18:55:20 GMT
WORKDIR /var/lib/neo4j
# Fri, 05 May 2023 18:55:20 GMT
VOLUME [/data /logs]
# Fri, 05 May 2023 18:55:20 GMT
EXPOSE 7473 7474 7687
# Fri, 05 May 2023 18:55:20 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 05 May 2023 18:55:20 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8372f00ab12bb739ea85b3b21db2dbe4809c7c3bd11102276ddbe52e3a864e`  
		Last Modified: Thu, 04 May 2023 10:20:09 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be1c502952730214e6c290ee9b13f0018911d40e0a72c05535507b79a9ca642`  
		Last Modified: Fri, 05 May 2023 18:55:54 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfd4d5af0b7ce2cbabacd65efb6a6edc53adf348b69e3bd5cd2172e313f519f`  
		Last Modified: Fri, 05 May 2023 18:55:54 GMT  
		Size: 8.7 KB (8706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f690115508090a789a2e096bfd38c34bc6c7bcb78c033ca20a4d4dc9f2425213`  
		Last Modified: Fri, 05 May 2023 18:56:03 GMT  
		Size: 216.5 MB (216543668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:894ef57b9074bebdc1fa75f448370665320b99bac4f29d6711624ef353fd515b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:3546a3130e80a51d420e7a07e925aa6465d2af87b77add87cb35f43c7a14caeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338685282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7856754509efc0504255ca580c2f4308504989facbbc2f883e5be0eb8553b71a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:18:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:18:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:18:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:18:42 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:18:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:18:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:18:54 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:18:54 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:18:54 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:18:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:18:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0787c8d764ee0036e5e76c521001f9628f82954d6c48640bdcc21b5242c109b`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f729f64977b963f46455a8c8eac4f2d66517b11d7bfc809833c1ded8562aef`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73577e5c94088cfb6c46a1b5b7842a84de0cfa9f0a77db52f267a2effe3bc56b`  
		Last Modified: Tue, 23 May 2023 04:20:24 GMT  
		Size: 114.7 MB (114688687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4d6f8f10da6ea588793a3624a53e9a95ff5ab0b1b902a43dc07b47f62f390a38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335998044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118fc18b61f9247dbf45ab43c8583dd5ce00bf5a2dde0a466716979be6c18743`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:40 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:41:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:41:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:41:52 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:41:53 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:41:53 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:41:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:41:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b24c0af0966f52b39ffed749fcc7ac480385ca848c515602292cf21b6ab5c57`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4a72bb959c2fe7d17c8e12b8227f7c4f3e46bb8cef32b8873f9fea23020eef`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3627f314bc804b661f816d55e262a6896e8cc46a7eb0c712589103882b0ac`  
		Last Modified: Mon, 22 May 2023 20:42:37 GMT  
		Size: 114.5 MB (114545018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:894ef57b9074bebdc1fa75f448370665320b99bac4f29d6711624ef353fd515b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:3546a3130e80a51d420e7a07e925aa6465d2af87b77add87cb35f43c7a14caeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338685282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7856754509efc0504255ca580c2f4308504989facbbc2f883e5be0eb8553b71a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:18:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:18:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:18:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:18:42 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:18:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:18:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:18:54 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:18:54 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:18:54 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:18:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:18:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0787c8d764ee0036e5e76c521001f9628f82954d6c48640bdcc21b5242c109b`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f729f64977b963f46455a8c8eac4f2d66517b11d7bfc809833c1ded8562aef`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73577e5c94088cfb6c46a1b5b7842a84de0cfa9f0a77db52f267a2effe3bc56b`  
		Last Modified: Tue, 23 May 2023 04:20:24 GMT  
		Size: 114.7 MB (114688687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4d6f8f10da6ea588793a3624a53e9a95ff5ab0b1b902a43dc07b47f62f390a38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335998044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118fc18b61f9247dbf45ab43c8583dd5ce00bf5a2dde0a466716979be6c18743`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:40 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:41:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:41:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:41:52 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:41:53 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:41:53 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:41:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:41:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b24c0af0966f52b39ffed749fcc7ac480385ca848c515602292cf21b6ab5c57`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4a72bb959c2fe7d17c8e12b8227f7c4f3e46bb8cef32b8873f9fea23020eef`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3627f314bc804b661f816d55e262a6896e8cc46a7eb0c712589103882b0ac`  
		Last Modified: Mon, 22 May 2023 20:42:37 GMT  
		Size: 114.5 MB (114545018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:b95a45aac610acc8b2494aac7d6fa377895bef5881f7d372b99eaafd4ebab064
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:e89709d490cfe4ad4f7a49e9690a1d4397b18f251acf68f8b6f4f0e847f84032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **603.7 MB (603679730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b1df17c9a9394414568590a6e11207fe6489768a304faa439ed658aab1f353`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:19:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:19:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:19:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:19:01 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:19:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:19:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:19:18 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:19:18 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:19:18 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:19:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:19:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5011326b12928bcd6584016f6aea605e8a53b9a1d6ac9a647ce032b78f52fad`  
		Last Modified: Tue, 23 May 2023 04:20:50 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b348a8efca0e9ac27d6a133a3ac8ae18412cac16ac1971201175e18477aee`  
		Last Modified: Tue, 23 May 2023 04:20:49 GMT  
		Size: 8.8 KB (8767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c95b5adb6f2b7ba27e4fd29866e1a9e6af175a955727d5983fa7352d7e09a`  
		Last Modified: Tue, 23 May 2023 04:21:04 GMT  
		Size: 379.7 MB (379683148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:42ca8fe6b98045d5dc3b59c5d9c86472e5f16b6fefa886beb3831aae222b7164
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.0 MB (600994101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a22ce0b872f728daecdabba3c63197159ae65a527218cad450964f7533a06e7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:56 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:42:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:42:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:42:12 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:42:13 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:42:13 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:42:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:42:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a6cfeb8c521df684b8271ff58c0bfe0f59f607c604302cc73f02e1176de805`  
		Last Modified: Mon, 22 May 2023 20:42:57 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da7fc38501e198ef67781844a1edb68b49581a33db12bccd6164c014ef48cfe`  
		Last Modified: Mon, 22 May 2023 20:42:57 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850ea76f6227ff05c47e82a52d3561c2f1d5adadd6525cba8479903aeab75794`  
		Last Modified: Mon, 22 May 2023 20:43:09 GMT  
		Size: 379.5 MB (379541072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.8`

```console
$ docker pull neo4j@sha256:894ef57b9074bebdc1fa75f448370665320b99bac4f29d6711624ef353fd515b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.8` - linux; amd64

```console
$ docker pull neo4j@sha256:3546a3130e80a51d420e7a07e925aa6465d2af87b77add87cb35f43c7a14caeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338685282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7856754509efc0504255ca580c2f4308504989facbbc2f883e5be0eb8553b71a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:18:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:18:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:18:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:18:42 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:18:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:18:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:18:54 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:18:54 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:18:54 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:18:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:18:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0787c8d764ee0036e5e76c521001f9628f82954d6c48640bdcc21b5242c109b`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f729f64977b963f46455a8c8eac4f2d66517b11d7bfc809833c1ded8562aef`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73577e5c94088cfb6c46a1b5b7842a84de0cfa9f0a77db52f267a2effe3bc56b`  
		Last Modified: Tue, 23 May 2023 04:20:24 GMT  
		Size: 114.7 MB (114688687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4d6f8f10da6ea588793a3624a53e9a95ff5ab0b1b902a43dc07b47f62f390a38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335998044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118fc18b61f9247dbf45ab43c8583dd5ce00bf5a2dde0a466716979be6c18743`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:40 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:41:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:41:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:41:52 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:41:53 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:41:53 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:41:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:41:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b24c0af0966f52b39ffed749fcc7ac480385ca848c515602292cf21b6ab5c57`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4a72bb959c2fe7d17c8e12b8227f7c4f3e46bb8cef32b8873f9fea23020eef`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3627f314bc804b661f816d55e262a6896e8cc46a7eb0c712589103882b0ac`  
		Last Modified: Mon, 22 May 2023 20:42:37 GMT  
		Size: 114.5 MB (114545018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.8-community`

```console
$ docker pull neo4j@sha256:894ef57b9074bebdc1fa75f448370665320b99bac4f29d6711624ef353fd515b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.8-community` - linux; amd64

```console
$ docker pull neo4j@sha256:3546a3130e80a51d420e7a07e925aa6465d2af87b77add87cb35f43c7a14caeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338685282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7856754509efc0504255ca580c2f4308504989facbbc2f883e5be0eb8553b71a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:18:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:18:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:18:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:18:42 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:18:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:18:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:18:54 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:18:54 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:18:54 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:18:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:18:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0787c8d764ee0036e5e76c521001f9628f82954d6c48640bdcc21b5242c109b`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f729f64977b963f46455a8c8eac4f2d66517b11d7bfc809833c1ded8562aef`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73577e5c94088cfb6c46a1b5b7842a84de0cfa9f0a77db52f267a2effe3bc56b`  
		Last Modified: Tue, 23 May 2023 04:20:24 GMT  
		Size: 114.7 MB (114688687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.8-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4d6f8f10da6ea588793a3624a53e9a95ff5ab0b1b902a43dc07b47f62f390a38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335998044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118fc18b61f9247dbf45ab43c8583dd5ce00bf5a2dde0a466716979be6c18743`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:40 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:41:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:41:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:41:52 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:41:53 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:41:53 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:41:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:41:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b24c0af0966f52b39ffed749fcc7ac480385ca848c515602292cf21b6ab5c57`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4a72bb959c2fe7d17c8e12b8227f7c4f3e46bb8cef32b8873f9fea23020eef`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3627f314bc804b661f816d55e262a6896e8cc46a7eb0c712589103882b0ac`  
		Last Modified: Mon, 22 May 2023 20:42:37 GMT  
		Size: 114.5 MB (114545018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.8-enterprise`

```console
$ docker pull neo4j@sha256:b95a45aac610acc8b2494aac7d6fa377895bef5881f7d372b99eaafd4ebab064
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.8-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:e89709d490cfe4ad4f7a49e9690a1d4397b18f251acf68f8b6f4f0e847f84032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **603.7 MB (603679730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b1df17c9a9394414568590a6e11207fe6489768a304faa439ed658aab1f353`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:19:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:19:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:19:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:19:01 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:19:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:19:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:19:18 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:19:18 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:19:18 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:19:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:19:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5011326b12928bcd6584016f6aea605e8a53b9a1d6ac9a647ce032b78f52fad`  
		Last Modified: Tue, 23 May 2023 04:20:50 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b348a8efca0e9ac27d6a133a3ac8ae18412cac16ac1971201175e18477aee`  
		Last Modified: Tue, 23 May 2023 04:20:49 GMT  
		Size: 8.8 KB (8767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c95b5adb6f2b7ba27e4fd29866e1a9e6af175a955727d5983fa7352d7e09a`  
		Last Modified: Tue, 23 May 2023 04:21:04 GMT  
		Size: 379.7 MB (379683148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.8-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:42ca8fe6b98045d5dc3b59c5d9c86472e5f16b6fefa886beb3831aae222b7164
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.0 MB (600994101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a22ce0b872f728daecdabba3c63197159ae65a527218cad450964f7533a06e7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:56 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:42:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:42:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:42:12 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:42:13 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:42:13 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:42:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:42:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a6cfeb8c521df684b8271ff58c0bfe0f59f607c604302cc73f02e1176de805`  
		Last Modified: Mon, 22 May 2023 20:42:57 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da7fc38501e198ef67781844a1edb68b49581a33db12bccd6164c014ef48cfe`  
		Last Modified: Mon, 22 May 2023 20:42:57 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850ea76f6227ff05c47e82a52d3561c2f1d5adadd6525cba8479903aeab75794`  
		Last Modified: Mon, 22 May 2023 20:43:09 GMT  
		Size: 379.5 MB (379541072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.8.0`

```console
$ docker pull neo4j@sha256:894ef57b9074bebdc1fa75f448370665320b99bac4f29d6711624ef353fd515b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.8.0` - linux; amd64

```console
$ docker pull neo4j@sha256:3546a3130e80a51d420e7a07e925aa6465d2af87b77add87cb35f43c7a14caeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338685282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7856754509efc0504255ca580c2f4308504989facbbc2f883e5be0eb8553b71a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:18:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:18:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:18:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:18:42 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:18:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:18:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:18:54 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:18:54 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:18:54 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:18:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:18:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0787c8d764ee0036e5e76c521001f9628f82954d6c48640bdcc21b5242c109b`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f729f64977b963f46455a8c8eac4f2d66517b11d7bfc809833c1ded8562aef`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73577e5c94088cfb6c46a1b5b7842a84de0cfa9f0a77db52f267a2effe3bc56b`  
		Last Modified: Tue, 23 May 2023 04:20:24 GMT  
		Size: 114.7 MB (114688687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.8.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4d6f8f10da6ea588793a3624a53e9a95ff5ab0b1b902a43dc07b47f62f390a38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335998044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118fc18b61f9247dbf45ab43c8583dd5ce00bf5a2dde0a466716979be6c18743`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:40 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:41:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:41:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:41:52 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:41:53 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:41:53 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:41:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:41:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b24c0af0966f52b39ffed749fcc7ac480385ca848c515602292cf21b6ab5c57`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4a72bb959c2fe7d17c8e12b8227f7c4f3e46bb8cef32b8873f9fea23020eef`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3627f314bc804b661f816d55e262a6896e8cc46a7eb0c712589103882b0ac`  
		Last Modified: Mon, 22 May 2023 20:42:37 GMT  
		Size: 114.5 MB (114545018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.8.0-community`

```console
$ docker pull neo4j@sha256:894ef57b9074bebdc1fa75f448370665320b99bac4f29d6711624ef353fd515b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.8.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:3546a3130e80a51d420e7a07e925aa6465d2af87b77add87cb35f43c7a14caeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338685282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7856754509efc0504255ca580c2f4308504989facbbc2f883e5be0eb8553b71a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:18:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:18:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:18:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:18:42 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:18:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:18:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:18:54 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:18:54 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:18:54 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:18:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:18:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0787c8d764ee0036e5e76c521001f9628f82954d6c48640bdcc21b5242c109b`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f729f64977b963f46455a8c8eac4f2d66517b11d7bfc809833c1ded8562aef`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73577e5c94088cfb6c46a1b5b7842a84de0cfa9f0a77db52f267a2effe3bc56b`  
		Last Modified: Tue, 23 May 2023 04:20:24 GMT  
		Size: 114.7 MB (114688687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.8.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4d6f8f10da6ea588793a3624a53e9a95ff5ab0b1b902a43dc07b47f62f390a38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335998044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118fc18b61f9247dbf45ab43c8583dd5ce00bf5a2dde0a466716979be6c18743`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:40 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:41:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:41:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:41:52 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:41:53 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:41:53 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:41:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:41:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b24c0af0966f52b39ffed749fcc7ac480385ca848c515602292cf21b6ab5c57`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4a72bb959c2fe7d17c8e12b8227f7c4f3e46bb8cef32b8873f9fea23020eef`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3627f314bc804b661f816d55e262a6896e8cc46a7eb0c712589103882b0ac`  
		Last Modified: Mon, 22 May 2023 20:42:37 GMT  
		Size: 114.5 MB (114545018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.8.0-enterprise`

```console
$ docker pull neo4j@sha256:b95a45aac610acc8b2494aac7d6fa377895bef5881f7d372b99eaafd4ebab064
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.8.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:e89709d490cfe4ad4f7a49e9690a1d4397b18f251acf68f8b6f4f0e847f84032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **603.7 MB (603679730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b1df17c9a9394414568590a6e11207fe6489768a304faa439ed658aab1f353`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:19:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:19:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:19:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:19:01 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:19:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:19:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:19:18 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:19:18 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:19:18 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:19:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:19:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5011326b12928bcd6584016f6aea605e8a53b9a1d6ac9a647ce032b78f52fad`  
		Last Modified: Tue, 23 May 2023 04:20:50 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b348a8efca0e9ac27d6a133a3ac8ae18412cac16ac1971201175e18477aee`  
		Last Modified: Tue, 23 May 2023 04:20:49 GMT  
		Size: 8.8 KB (8767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c95b5adb6f2b7ba27e4fd29866e1a9e6af175a955727d5983fa7352d7e09a`  
		Last Modified: Tue, 23 May 2023 04:21:04 GMT  
		Size: 379.7 MB (379683148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.8.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:42ca8fe6b98045d5dc3b59c5d9c86472e5f16b6fefa886beb3831aae222b7164
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.0 MB (600994101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a22ce0b872f728daecdabba3c63197159ae65a527218cad450964f7533a06e7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:56 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:42:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:42:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:42:12 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:42:13 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:42:13 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:42:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:42:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a6cfeb8c521df684b8271ff58c0bfe0f59f607c604302cc73f02e1176de805`  
		Last Modified: Mon, 22 May 2023 20:42:57 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da7fc38501e198ef67781844a1edb68b49581a33db12bccd6164c014ef48cfe`  
		Last Modified: Mon, 22 May 2023 20:42:57 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850ea76f6227ff05c47e82a52d3561c2f1d5adadd6525cba8479903aeab75794`  
		Last Modified: Mon, 22 May 2023 20:43:09 GMT  
		Size: 379.5 MB (379541072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:894ef57b9074bebdc1fa75f448370665320b99bac4f29d6711624ef353fd515b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:3546a3130e80a51d420e7a07e925aa6465d2af87b77add87cb35f43c7a14caeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338685282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7856754509efc0504255ca580c2f4308504989facbbc2f883e5be0eb8553b71a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:18:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:18:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:18:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:18:42 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:18:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:18:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:18:54 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:18:54 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:18:54 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:18:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:18:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0787c8d764ee0036e5e76c521001f9628f82954d6c48640bdcc21b5242c109b`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f729f64977b963f46455a8c8eac4f2d66517b11d7bfc809833c1ded8562aef`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73577e5c94088cfb6c46a1b5b7842a84de0cfa9f0a77db52f267a2effe3bc56b`  
		Last Modified: Tue, 23 May 2023 04:20:24 GMT  
		Size: 114.7 MB (114688687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4d6f8f10da6ea588793a3624a53e9a95ff5ab0b1b902a43dc07b47f62f390a38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335998044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118fc18b61f9247dbf45ab43c8583dd5ce00bf5a2dde0a466716979be6c18743`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:40 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:41:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:41:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:41:52 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:41:53 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:41:53 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:41:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:41:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b24c0af0966f52b39ffed749fcc7ac480385ca848c515602292cf21b6ab5c57`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4a72bb959c2fe7d17c8e12b8227f7c4f3e46bb8cef32b8873f9fea23020eef`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3627f314bc804b661f816d55e262a6896e8cc46a7eb0c712589103882b0ac`  
		Last Modified: Mon, 22 May 2023 20:42:37 GMT  
		Size: 114.5 MB (114545018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:b95a45aac610acc8b2494aac7d6fa377895bef5881f7d372b99eaafd4ebab064
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:e89709d490cfe4ad4f7a49e9690a1d4397b18f251acf68f8b6f4f0e847f84032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **603.7 MB (603679730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b1df17c9a9394414568590a6e11207fe6489768a304faa439ed658aab1f353`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:19:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:19:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:19:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:19:01 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:19:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:19:18 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:19:18 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:19:18 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:19:18 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:19:19 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:19:19 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5011326b12928bcd6584016f6aea605e8a53b9a1d6ac9a647ce032b78f52fad`  
		Last Modified: Tue, 23 May 2023 04:20:50 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b348a8efca0e9ac27d6a133a3ac8ae18412cac16ac1971201175e18477aee`  
		Last Modified: Tue, 23 May 2023 04:20:49 GMT  
		Size: 8.8 KB (8767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c95b5adb6f2b7ba27e4fd29866e1a9e6af175a955727d5983fa7352d7e09a`  
		Last Modified: Tue, 23 May 2023 04:21:04 GMT  
		Size: 379.7 MB (379683148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:42ca8fe6b98045d5dc3b59c5d9c86472e5f16b6fefa886beb3831aae222b7164
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.0 MB (600994101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a22ce0b872f728daecdabba3c63197159ae65a527218cad450964f7533a06e7`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:56 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:42:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:42:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:42:12 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:42:13 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:42:13 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:42:13 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:42:13 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a6cfeb8c521df684b8271ff58c0bfe0f59f607c604302cc73f02e1176de805`  
		Last Modified: Mon, 22 May 2023 20:42:57 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da7fc38501e198ef67781844a1edb68b49581a33db12bccd6164c014ef48cfe`  
		Last Modified: Mon, 22 May 2023 20:42:57 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850ea76f6227ff05c47e82a52d3561c2f1d5adadd6525cba8479903aeab75794`  
		Last Modified: Mon, 22 May 2023 20:43:09 GMT  
		Size: 379.5 MB (379541072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:894ef57b9074bebdc1fa75f448370665320b99bac4f29d6711624ef353fd515b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:3546a3130e80a51d420e7a07e925aa6465d2af87b77add87cb35f43c7a14caeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338685282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7856754509efc0504255ca580c2f4308504989facbbc2f883e5be0eb8553b71a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:18:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 04:18:39 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Tue, 23 May 2023 04:18:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 23 May 2023 04:18:41 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 23 May 2023 04:18:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 23 May 2023 04:18:42 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Tue, 23 May 2023 04:18:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:18:54 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 04:18:54 GMT
WORKDIR /var/lib/neo4j
# Tue, 23 May 2023 04:18:54 GMT
VOLUME [/data /logs]
# Tue, 23 May 2023 04:18:54 GMT
EXPOSE 7473 7474 7687
# Tue, 23 May 2023 04:18:54 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 23 May 2023 04:18:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e304d0221eddeca3682794711387f6677072df1d6fd9df02ff4f7487148d1df`  
		Last Modified: Tue, 23 May 2023 04:20:31 GMT  
		Size: 192.6 MB (192580374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0787c8d764ee0036e5e76c521001f9628f82954d6c48640bdcc21b5242c109b`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f729f64977b963f46455a8c8eac4f2d66517b11d7bfc809833c1ded8562aef`  
		Last Modified: Tue, 23 May 2023 04:20:18 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73577e5c94088cfb6c46a1b5b7842a84de0cfa9f0a77db52f267a2effe3bc56b`  
		Last Modified: Tue, 23 May 2023 04:20:24 GMT  
		Size: 114.7 MB (114688687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:4d6f8f10da6ea588793a3624a53e9a95ff5ab0b1b902a43dc07b47f62f390a38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335998044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118fc18b61f9247dbf45ab43c8583dd5ce00bf5a2dde0a466716979be6c18743`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Mon, 22 May 2023 20:41:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Mon, 22 May 2023 20:41:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Mon, 22 May 2023 20:41:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Mon, 22 May 2023 20:41:40 GMT
COPY multi:b0adb110d92b4bcfe30cb0c0db43c522b6bd0c9497a88b7577c0c7f10bfdc932 in /startup/ 
# Mon, 22 May 2023 20:41:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Mon, 22 May 2023 20:41:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 May 2023 20:41:52 GMT
WORKDIR /var/lib/neo4j
# Mon, 22 May 2023 20:41:53 GMT
VOLUME [/data /logs]
# Mon, 22 May 2023 20:41:53 GMT
EXPOSE 7473 7474 7687
# Mon, 22 May 2023 20:41:53 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Mon, 22 May 2023 20:41:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b24c0af0966f52b39ffed749fcc7ac480385ca848c515602292cf21b6ab5c57`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4a72bb959c2fe7d17c8e12b8227f7c4f3e46bb8cef32b8873f9fea23020eef`  
		Last Modified: Mon, 22 May 2023 20:42:33 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3627f314bc804b661f816d55e262a6896e8cc46a7eb0c712589103882b0ac`  
		Last Modified: Mon, 22 May 2023 20:42:37 GMT  
		Size: 114.5 MB (114545018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
