## `neo4j:community`

```console
$ docker pull neo4j@sha256:418d2168b6a275345ce748b5c7a2ff3ab5011c4687c1e31cdbde9e399fc664c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:9507716bec4ca7d48ab0037255c5419266033619ff8355c2e6a44fa1b3c8fe44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.5 MB (364537914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f5876b8aa043c64234bb02803ecb6aa6a518eee4d19a076b38df6b4e34fa9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 11:31:38 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 02 Sep 2022 11:31:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=869ecb89ce36fe457b4d4c4fcaa48fdf2f2d739c45323bd2c8ccdf09aa11abbf NEO4J_TARBALL=neo4j-community-4.4.10-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 02 Sep 2022 11:31:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
# Fri, 02 Sep 2022 11:31:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 02 Sep 2022 11:31:41 GMT
COPY multi:3374c8dc0747f37551a88a28b1d77a933ccfa81a6b8258bf2e495e2876116c57 in /startup/ 
# Fri, 02 Sep 2022 11:31:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.10-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 11:31:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 11:31:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 02 Sep 2022 11:31:55 GMT
VOLUME [/data /logs]
# Fri, 02 Sep 2022 11:31:55 GMT
EXPOSE 7473 7474 7687
# Fri, 02 Sep 2022 11:31:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 11:31:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c89c817336057daee61fcc5ec012333e1eb4322a14f22cbb1454a07b6e355b`  
		Last Modified: Fri, 02 Sep 2022 11:39:19 GMT  
		Size: 198.1 MB (198124885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f992a8f96b44906367e7df1757bb4d1efa17bb01c3ae2d72bc9cbde7b6750`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c343745c86d04ce9eb039476b43408a016a0d79525849c203fb90828ad656`  
		Last Modified: Fri, 02 Sep 2022 11:39:04 GMT  
		Size: 7.6 KB (7614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6e702c7c721e45a25e71ee1c6314bfe151cf63524beb784bc0fa536d7e00c5`  
		Last Modified: Fri, 02 Sep 2022 11:39:12 GMT  
		Size: 135.0 MB (135020071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:6e23f8985f37c5f73a181ef08b97dc6f91a30dbff41169330464ff452a9818ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.7 MB (359689153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be5bece553e8afc0924244b8735d765220716c4e2847f7bcd37402a5e77dbce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:03:47 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Wed, 07 Sep 2022 18:40:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=28810daac5de4a5d5b77ce2da7d7c3da4c5ccf13288bad885b833c35b96100c8 NEO4J_TARBALL=neo4j-community-4.4.11-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 07 Sep 2022 18:40:16 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
# Wed, 07 Sep 2022 18:40:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 07 Sep 2022 18:40:19 GMT
COPY multi:8d06e2159cef389ad848accdd078d2b91b147b7708e8ebf82c3f2530c0cabbdf in /startup/ 
# Wed, 07 Sep 2022 18:40:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 07 Sep 2022 18:40:30 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Sep 2022 18:40:31 GMT
WORKDIR /var/lib/neo4j
# Wed, 07 Sep 2022 18:40:32 GMT
VOLUME [/data /logs]
# Wed, 07 Sep 2022 18:40:33 GMT
EXPOSE 7473 7474 7687
# Wed, 07 Sep 2022 18:40:34 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 07 Sep 2022 18:40:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf0f19121849fff7b9de1a3bc603d164cb1b1f319434b16b849eb8536c40b7`  
		Last Modified: Fri, 02 Sep 2022 09:08:39 GMT  
		Size: 194.9 MB (194867809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a31b9357381bc63974a52b519130fc7be72ecfbaa7aa63afd7168d3b6304703`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e906c0279c826c5d1292427d9465b014b03fa4a076c06253729b6994b743bfd`  
		Last Modified: Wed, 07 Sep 2022 18:42:07 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de213bd8dd684e20b128be0c029a9fabf773a7950c2a4a1c376b56d046689bb5`  
		Last Modified: Wed, 07 Sep 2022 18:42:16 GMT  
		Size: 134.7 MB (134746137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
