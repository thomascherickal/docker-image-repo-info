## `neo4j:latest`

```console
$ docker pull neo4j@sha256:176ed83343771264a78a7ef8ae802b95b9355ccfd00516fb3759d1e0a2bc6e94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:ee4b2d77cf3ffd5e6c4ae831c5bd058d9e2fa41ad0963e76a948b649e60a658c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.4 MB (338446767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0471a45f9a41007a1128b3cf918af56567051673f20d397c85b65421abd709b9`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:51:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:57:05 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Wed, 21 Dec 2022 11:52:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 21 Dec 2022 11:52:53 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Wed, 21 Dec 2022 11:52:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 21 Dec 2022 11:52:54 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Wed, 21 Dec 2022 11:53:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:53:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 11:53:07 GMT
WORKDIR /var/lib/neo4j
# Wed, 21 Dec 2022 11:53:07 GMT
VOLUME [/data /logs]
# Wed, 21 Dec 2022 11:53:07 GMT
EXPOSE 7473 7474 7687
# Wed, 21 Dec 2022 11:53:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:53:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3d6f042d4c187dc5ef35678240ad79b89963342d31898de3665a87a1568323`  
		Last Modified: Wed, 21 Dec 2022 02:09:14 GMT  
		Size: 192.4 MB (192431237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f42abb3f13626627d701ea540016be3c6d3ab0fb8a2f4a495a915d179de7f35`  
		Last Modified: Wed, 21 Dec 2022 11:56:34 GMT  
		Size: 3.9 KB (3866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68a0ef87b6ee5b98aedacfa770d3f51a791e062695811554e1fe0b901382ff1`  
		Last Modified: Wed, 21 Dec 2022 11:56:35 GMT  
		Size: 8.3 KB (8341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d367d623d9a4c6c38a4d94e3b962694ea2908d3e90023efd5be312715b13851`  
		Last Modified: Wed, 21 Dec 2022 11:56:40 GMT  
		Size: 114.6 MB (114606380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8f56ec3cd02d791f5fefe39c3212196be2632e69f156c97ee0fff805bf5da8ea
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.7 MB (335736302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28da406a1c57ad170bc4919c0817a4f9502b2b405fc4a415831ccf28a87429ba`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:43:55 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Wed, 11 Jan 2023 05:56:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=b20a3f253c42faccd1d2c37f9cc8bf6d557f0e645dced39e163da5ae12bb8d0a NEO4J_TARBALL=neo4j-community-5.3.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 11 Jan 2023 05:56:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
# Wed, 11 Jan 2023 05:56:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 11 Jan 2023 05:56:02 GMT
COPY multi:81f46e88e454671d24b1557a3a4cbb35163739c6808b91d7f90db70483d2b6ac in /startup/ 
# Wed, 11 Jan 2023 05:56:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.3.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 05:56:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 05:56:12 GMT
WORKDIR /var/lib/neo4j
# Wed, 11 Jan 2023 05:56:12 GMT
VOLUME [/data /logs]
# Wed, 11 Jan 2023 05:56:12 GMT
EXPOSE 7473 7474 7687
# Wed, 11 Jan 2023 05:56:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 05:56:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af213950f8cc63689dbc3db5e95e2955b9c5a24f79594f3d9716eec20e2bb23`  
		Last Modified: Wed, 11 Jan 2023 03:54:33 GMT  
		Size: 191.2 MB (191215202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a47ca77276b31855daf4c87303527ebd8feebcd0384fef04b80d1744403e28`  
		Last Modified: Wed, 11 Jan 2023 05:57:34 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fb7786289df3458aa260cbb826339383871873b32555e6de3fc77bfefaa4b9`  
		Last Modified: Wed, 11 Jan 2023 05:57:34 GMT  
		Size: 8.3 KB (8339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5e812311c598103458a64184acdcc233b248fe61521ca786b9efdabc5247db`  
		Last Modified: Wed, 11 Jan 2023 05:57:39 GMT  
		Size: 114.5 MB (114464059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
