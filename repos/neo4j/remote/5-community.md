## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:b99ccc63b8b900a7c5fee373bdb4e5b22e9865326928e0502733004bcc7f9678
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:8c9f3e2012fbf49d33f29c3b0f2e5081e58c163f9f1296ee6091d390983ad0c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338568184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c141267db25cdcb805da3df6a8d070f8ef0ee5f2e0f17e98b7968af3f30740f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:06:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 14:12:04 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Sat, 04 Feb 2023 14:50:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:50:45 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Sat, 04 Feb 2023 14:50:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 07 Feb 2023 20:26:23 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Tue, 07 Feb 2023 20:26:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Feb 2023 20:26:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 20:26:39 GMT
WORKDIR /var/lib/neo4j
# Tue, 07 Feb 2023 20:26:39 GMT
VOLUME [/data /logs]
# Tue, 07 Feb 2023 20:26:39 GMT
EXPOSE 7473 7474 7687
# Tue, 07 Feb 2023 20:26:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 20:26:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87fb4ccb46beb33988288373afc1f2c97de5052711ef02009468a1bea691666`  
		Last Modified: Sat, 04 Feb 2023 14:24:01 GMT  
		Size: 192.4 MB (192438215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9d42968b209b3d117503b27b2266ebd63e1a04f05b0c36067f47094b3a8344`  
		Last Modified: Sat, 04 Feb 2023 14:52:18 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a991bff651eb0b0cbcddb8b0859f75d27095291db0b676e5ec8876979e9c0`  
		Last Modified: Tue, 07 Feb 2023 20:27:25 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a6831ab8c610b6c10f47d5f807f3a8cd49d73f7cb5540c9519d242514d40`  
		Last Modified: Tue, 07 Feb 2023 20:27:31 GMT  
		Size: 114.7 MB (114720771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:ad36e3fda92e436c4ba2b5cce4b130f2730e18c6ccf584d35357eb17ca24bc74
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335896503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f233089ca573444f72a5116a4bee69ce5d7e4a6a4bf23c0444f093501129b98b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:44:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 08:44:47 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Sat, 04 Feb 2023 08:44:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=aa985dd8298e2f82f744a0dc4693369aad26afff0338c14459fc3331e43ef143 NEO4J_TARBALL=neo4j-community-5.4.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:44:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
# Sat, 04 Feb 2023 08:44:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 07 Feb 2023 20:44:50 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Tue, 07 Feb 2023 20:45:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Feb 2023 20:45:00 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 20:45:00 GMT
WORKDIR /var/lib/neo4j
# Tue, 07 Feb 2023 20:45:00 GMT
VOLUME [/data /logs]
# Tue, 07 Feb 2023 20:45:00 GMT
EXPOSE 7473 7474 7687
# Tue, 07 Feb 2023 20:45:01 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 20:45:01 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3e25b707e39161f4cf1a28cf3bd4a0ec84bd0f2c93f699a34dc6dd1715cd62`  
		Last Modified: Sat, 04 Feb 2023 08:46:51 GMT  
		Size: 191.3 MB (191260441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46019c292e3e8d2f300738a84fd7c6aecabd7897468fb912bf208e09d1bbf17`  
		Last Modified: Sat, 04 Feb 2023 08:46:39 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded3a408642e4f2e3f0213aa7ac2bb5a141e29cd9749b01e22503f4ec81560a1`  
		Last Modified: Tue, 07 Feb 2023 20:45:43 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d4b1292d70c5468bae7b5782322665a0a4738fc1aa5e125e3aa17ac8fb61e`  
		Last Modified: Tue, 07 Feb 2023 20:45:48 GMT  
		Size: 114.6 MB (114578967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
