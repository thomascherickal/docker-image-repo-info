## `neo4j:latest`

```console
$ docker pull neo4j@sha256:ed6eb77058badabf0bcfda50da1f2dd5b53314f6afaacaed17eb1b65b64e3b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:135374c22967b8b028cfe0ec231e8faa28bb189dcb703f7c13487c6a43ae8722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339670142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc3aa6987130b610e932d5f648d9bcf34ba20f08f2ade3e01358ed68bdafcf`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:30:06 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 03 May 2023 21:09:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 03 May 2023 21:09:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Wed, 03 May 2023 21:10:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 03 May 2023 21:10:00 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Wed, 03 May 2023 21:10:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:10:11 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:10:11 GMT
WORKDIR /var/lib/neo4j
# Wed, 03 May 2023 21:10:11 GMT
VOLUME [/data /logs]
# Wed, 03 May 2023 21:10:11 GMT
EXPOSE 7473 7474 7687
# Wed, 03 May 2023 21:10:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 03 May 2023 21:10:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b479fcddcbb50b65db69b8812d87215c90a11a644267765f3dc0e7f19bde9`  
		Last Modified: Wed, 03 May 2023 20:38:39 GMT  
		Size: 192.6 MB (192580429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc29b8a0be2fdad2c0209669f62e4a52c8f1822951fd3606aee9871f291d458`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473676f5c4b0591fda9c3a2dc4d07de297f88ad552f76e8f8c149e35c2d1c5c2`  
		Last Modified: Wed, 03 May 2023 21:11:20 GMT  
		Size: 8.8 KB (8768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93765534ca788832bdfd3a07f7f80c9b8272a126028f2b2b9f44bce7399bf5d5`  
		Last Modified: Wed, 03 May 2023 21:11:25 GMT  
		Size: 115.7 MB (115673571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7aa4ae79e62f700964a424d6166309162ad421ea7241cdfef8782cb7b5abf210
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (336981794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6c0929c126c1a2abcd1b5af1ca7420955f76624ac87ea1d5e06f14b84b271`
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
# Thu, 04 May 2023 12:04:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=e13e94d8c8730f9525f30f98821ade79b349af1697d7ac94a8c3cc8b0273b734 NEO4J_TARBALL=neo4j-community-5.7.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 04 May 2023 12:04:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
# Thu, 04 May 2023 12:04:48 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 04 May 2023 12:04:48 GMT
COPY multi:231d2413caca967db6cb3937a1975c89c8f725750a4c6cb2893820fb868a6427 in /startup/ 
# Thu, 04 May 2023 12:05:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.7.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:01 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:05:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 04 May 2023 12:05:01 GMT
VOLUME [/data /logs]
# Thu, 04 May 2023 12:05:01 GMT
EXPOSE 7473 7474 7687
# Thu, 04 May 2023 12:05:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 04 May 2023 12:05:02 GMT
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
	-	`sha256:c93a8328b0b62b333b941f4f72d41fbe9f1cb67c1bdfd42ef100aa881314e839`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ce690ce0b7d3890d98ff9ccdded5c33f4227911f17a5595392105e27326e3`  
		Last Modified: Thu, 04 May 2023 12:06:09 GMT  
		Size: 8.8 KB (8773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b6be57bf03bc40983fbb0f78148f99a9c9fc273d643783cc2d9a6ed968b1a`  
		Last Modified: Thu, 04 May 2023 12:06:14 GMT  
		Size: 115.5 MB (115528758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
