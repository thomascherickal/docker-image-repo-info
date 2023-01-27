## `neo4j:community`

```console
$ docker pull neo4j@sha256:4da73555d51ae5a40b698bc9654c9d629e3a972040be0bb7c22d4e04865c5342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:79c2a5802ac0684fbce0d85421d0cb994967f4f57c7b9d8152ee26890b45aa60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338568057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801d7a542ed2c02db9b9a2984cf97d5b2a298b56bf1b36e27735a380934afc83`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Fri, 27 Jan 2023 20:19:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 20:19:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 20:19:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 20:19:52 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 20:20:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 20:20:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 20:20:06 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 20:20:06 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 20:20:06 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 20:20:06 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 20:20:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d46b5ccec1c38088acc371a620c831f87e7954f5274fe56194ad0fc35d51`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d912719189eb3a824e515e108b0e1eb5067c9ccc1b821183ec5aef7fe64db`  
		Last Modified: Fri, 27 Jan 2023 20:20:54 GMT  
		Size: 8.3 KB (8338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beaef1edc03f7eca9434fbd08ebc846f5ebde22524306bd963c7390affea6a72`  
		Last Modified: Fri, 27 Jan 2023 20:21:00 GMT  
		Size: 114.7 MB (114720741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:fa8d67f81f72551bf4f03be555e4ad3a2a262f33b1e3c31de06040b3e69d02a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7389ff6917629855abdeaa437e2becdc1b14b80af326e21533f40c4cb241a3bd`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 24 Jan 2023 21:04:04 GMT
COPY dir:6138ae24df63cd8b909473221414960a006ae73d2e2f1e88f48051984c7a0e00 in /opt/java/openjdk 
# Fri, 27 Jan 2023 21:17:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 27 Jan 2023 21:17:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Fri, 27 Jan 2023 21:17:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 27 Jan 2023 21:17:10 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Fri, 27 Jan 2023 21:17:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2023 21:17:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 21:17:21 GMT
WORKDIR /var/lib/neo4j
# Fri, 27 Jan 2023 21:17:21 GMT
VOLUME [/data /logs]
# Fri, 27 Jan 2023 21:17:21 GMT
EXPOSE 7473 7474 7687
# Fri, 27 Jan 2023 21:17:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 27 Jan 2023 21:17:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f35e12b4b859554fa3c720b691ca2e6d60e7e2e24c6332157caccf058052ab7`  
		Last Modified: Tue, 24 Jan 2023 21:14:03 GMT  
		Size: 191.3 MB (191260429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db6ad68d5043079adfe47bcd5eea82a6b923a893c3d56c82b7655371f544280`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398d73d2bf5d1dba7105ca31b65ad4d44e4c0bab7a6a627b4427d20e8dc5954d`  
		Last Modified: Fri, 27 Jan 2023 21:18:07 GMT  
		Size: 8.3 KB (8342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7bb5b9140f835f1d3638d645d54df4ce5f594068484b4d5ce7ff3474318ebb`  
		Last Modified: Fri, 27 Jan 2023 21:18:12 GMT  
		Size: 114.6 MB (114579133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
