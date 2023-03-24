## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:81ef7aa43a1fb07bf90d1759d5fcd4be1378284cfbafdd398530b6de8e2e63c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:0bdfac10c6cf85f39245526db306978b4bd8fc5221213f2345d458a7dae0c8a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339535267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f270818e4e86dd95357d6e40dc6bec49d937d57506ab65f35ea42a6ca1d31564`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:23:11 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Fri, 24 Mar 2023 22:19:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=16cc236a08fd99acea9b08dc9b19c016dc693bb97fa4f4ca81c2c90cf9452292 NEO4J_TARBALL=neo4j-community-5.6.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Mar 2023 22:19:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.6.0-unix.tar.gz
# Fri, 24 Mar 2023 22:19:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.6.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Mar 2023 22:19:45 GMT
COPY multi:a0d7d5f1f7f5a76cb0c8925dfafbe8943f9d1b1a76afc1b0ac964f6eb93156be in /startup/ 
# Fri, 24 Mar 2023 22:19:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.6.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 22:19:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 22:19:57 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Mar 2023 22:19:57 GMT
VOLUME [/data /logs]
# Fri, 24 Mar 2023 22:19:57 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Mar 2023 22:19:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 22:19:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f5c96fe943f36d4d8aa8ab4df9c0bd26f8cd6280632e002706fc7d61a975aa`  
		Last Modified: Thu, 23 Mar 2023 06:32:52 GMT  
		Size: 192.4 MB (192438234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f43c670dbde27898598509ec1b583b9f7effb76884e823603070ffa0be9bd08`  
		Last Modified: Fri, 24 Mar 2023 22:20:36 GMT  
		Size: 3.9 KB (3853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab0797c19058ae57b5132cd37e1a2cee660e7d9ec12848145dfb7ba5f573429`  
		Last Modified: Fri, 24 Mar 2023 22:20:36 GMT  
		Size: 8.6 KB (8625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed80d8fc6458c1c4a250defc7f4109d3da12fcf904944ec29ac67c23a6af2f7`  
		Last Modified: Fri, 24 Mar 2023 22:20:41 GMT  
		Size: 115.7 MB (115673150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:e0d5c90a53158a563c66ecc5cccf708cdfb5f4fb8c3ad26d7d2ceff1aac1f1a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336866734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bdee3d203ae3538bbb68570149fdd25c9994029ba2333a69d470c4dfdd82e6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:57:23 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Fri, 24 Mar 2023 21:39:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=16cc236a08fd99acea9b08dc9b19c016dc693bb97fa4f4ca81c2c90cf9452292 NEO4J_TARBALL=neo4j-community-5.6.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Mar 2023 21:39:38 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.6.0-unix.tar.gz
# Fri, 24 Mar 2023 21:39:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.6.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Mar 2023 21:39:39 GMT
COPY multi:a0d7d5f1f7f5a76cb0c8925dfafbe8943f9d1b1a76afc1b0ac964f6eb93156be in /startup/ 
# Fri, 24 Mar 2023 21:39:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.6.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 21:39:49 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 21:39:49 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Mar 2023 21:39:49 GMT
VOLUME [/data /logs]
# Fri, 24 Mar 2023 21:39:49 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Mar 2023 21:39:49 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 21:39:50 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46c3fded23542cb5a993d929bb8b2dfc32a31d4c9928588d2da3bc91d84fec`  
		Last Modified: Thu, 23 Mar 2023 07:06:00 GMT  
		Size: 191.3 MB (191260416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737154f6de69f9045e142a8da3146a9fc0a41ca310383db0f39f146dd86b41d2`  
		Last Modified: Fri, 24 Mar 2023 21:40:32 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d896bdd286f69e68772ea9c57d9727341d9de89164bac6a792ced55572f9b8f9`  
		Last Modified: Fri, 24 Mar 2023 21:40:32 GMT  
		Size: 8.6 KB (8631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd237490ceadc3ee24d992583d9ddd699ce3ab62961aa576393d7aa125b928c`  
		Last Modified: Fri, 24 Mar 2023 21:40:37 GMT  
		Size: 115.5 MB (115531104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
