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
